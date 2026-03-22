# uboot适配修改

```c
void rockchip_dnl_mode_check(void)
{
        if (rockchip_dnl_key_pressed()) {
                printf("download key pressed, entering download mode...\n");
                /* If failed, we fall back to bootrom download mode */
                cli_simple_run_command("rockusb 0 mmc 0", 0);
                set_back_to_bootrom_dnl_flag();
                do_reset(NULL, 0, 0, NULL);
        }
}


```

## 自定义maskrom命令，一键进入maskrom

```c
# cat cmd/maskrom.c 
/*
 * Copyright 2017 Rockchip Electronics Co., Ltd
 * Frank Wang <frank.wang@rock-chips.com>
 *
 * SPDX-License-Identifier:	GPL-2.0+
 */

#include <errno.h>
#include <common.h>
#include <command.h>
#include <console.h>
#include <g_dnl.h>
#include <part.h>
#include <usb.h>
#include <usb_mass_storage.h>
#include <rockusb.h>

void set_back_to_bootrom_dnl_flag(void);

static int do_maskrom(cmd_tbl_t *cmdtp, int flag, int argc, char *const argv[])
{
	set_back_to_bootrom_dnl_flag();
	do_reset(NULL, 0, 0, NULL);
	return 0;
}

U_BOOT_CMD(maskrom, 4, 1, do_maskrom,
	   "Just enter maskrom",
	   "Just enter maskrom\n"
);

```