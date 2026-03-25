# rockchip-linux仓库develop-6.6内核

## 基本信息

```shell

root@armbian:~# uname -a
Linux armbian 6.6.89-kdev #1 SMP Wed Mar 25 04:56:28 UTC 2026 aarch64 GNU/Linux
root@armbian:~# 
root@armbian:~# lsusb -t
/:  Bus 001.Port 001: Dev 001, Class=root_hub, Driver=ehci-platform/1p, 480M
/:  Bus 002.Port 001: Dev 001, Class=root_hub, Driver=ehci-platform/1p, 480M
/:  Bus 003.Port 001: Dev 001, Class=root_hub, Driver=xhci-hcd/1p, 480M
/:  Bus 004.Port 001: Dev 001, Class=root_hub, Driver=ohci-platform/1p, 12M
/:  Bus 005.Port 001: Dev 001, Class=root_hub, Driver=ohci-platform/1p, 12M
    |__ Port 001: Dev 002, If 0, Class=Communications, Driver=cdc_acm, 12M
    |__ Port 001: Dev 002, If 1, Class=CDC Data, Driver=cdc_acm, 12M
    |__ Port 001: Dev 002, If 2, Class=Communications, Driver=cdc_acm, 12M
    |__ Port 001: Dev 002, If 3, Class=CDC Data, Driver=cdc_acm, 12M
    |__ Port 001: Dev 002, If 4, Class=Communications, Driver=cdc_acm, 12M
    |__ Port 001: Dev 002, If 5, Class=CDC Data, Driver=cdc_acm, 12M
    |__ Port 001: Dev 002, If 6, Class=Communications, Driver=cdc_acm, 12M
    |__ Port 001: Dev 002, If 7, Class=CDC Data, Driver=cdc_acm, 12M
/:  Bus 006.Port 001: Dev 001, Class=root_hub, Driver=xhci-hcd/1p, 5000M
/:  Bus 007.Port 001: Dev 001, Class=root_hub, Driver=xhci-hcd/1p, 480M
    |__ Port 001: Dev 002, If 0, Class=Hub, Driver=hub/4p, 480M
/:  Bus 008.Port 001: Dev 001, Class=root_hub, Driver=xhci-hcd/1p, 5000M
    |__ Port 001: Dev 002, If 0, Class=Hub, Driver=hub/4p, 5000M
root@armbian:~# 
root@armbian:~# lspci -nn
root@armbian:~# 
root@armbian:~# 


```