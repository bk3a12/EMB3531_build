# 官方固件

## uboot

```text
bbe5181d5971e62b8eb4f371747f2e03  ./RK3399-EMB-3531-V2.2-Linux-General-debian_base-armhf_20200423/uboot/uboot.img
f66742b70950c8edba10bdc6c85abdfc  ./RK3399-EMB-3531-V2.2-Linux-General-ubuntu18.04_terminal-armhf_20200423/uboot/uboot.img

d74889f35bb5796dfe9db1f771775e6b  ./RK3399-EMB-3531-V2.2-Linux-General-debian_base-armhf_20200423/uboot/dtb-uboot.dtb
d74889f35bb5796dfe9db1f771775e6b  ./RK3399-EMB-3531-V2.2-Linux-General-ubuntu18.04_terminal-armhf_20200423/uboot/dtb-uboot.dtb

9e9a8eabb6f89a7cf5c10148d2809d09  ./RK3399-EMB-3531-V2.2-Linux-General-ubuntu18.04_terminal-armhf_20200423/uboot/dtb-uboot.dts
9e9a8eabb6f89a7cf5c10148d2809d09  ./RK3399-EMB-3531-V2.2-Linux-General-debian_base-armhf_20200423/uboot/dtb-uboot.dts
```

## trust

```text
83557680eeb5680a71354c326dd9226c  ./RK3399-EMB-3531-V2.2-Linux-General-ubuntu18.04_terminal-armhf_20200423/trust.img
83557680eeb5680a71354c326dd9226c  ./RK3399-EMB-3531-V2.2-Linux-General-debian_base-armhf_20200423/trust.img
```

## boot

```text
14092260121859644039166e1f84f3c4  ./RK3399-EMB-3531-V2.2-Linux-General-ubuntu18.04_terminal-armhf_20200423/boot/boot.img
14092260121859644039166e1f84f3c4  ./RK3399-EMB-3531-V2.2-Linux-General-debian_base-armhf_20200423/boot/boot.img

059daea9cf8d0c2f25a99551de7639aa  ./RK3399-EMB-3531-V2.2-Linux-General-ubuntu18.04_terminal-armhf_20200423/boot/dtb-kernel.dtb
059daea9cf8d0c2f25a99551de7639aa  ./RK3399-EMB-3531-V2.2-Linux-General-debian_base-armhf_20200423/boot/dtb-kernel.dtb

ebb573c8101592e5152532cc30555cb7  ./RK3399-EMB-3531-V2.2-Linux-General-ubuntu18.04_terminal-armhf_20200423/boot/dtb-kernel.dts
ebb573c8101592e5152532cc30555cb7  ./RK3399-EMB-3531-V2.2-Linux-General-debian_base-armhf_20200423/boot/dtb-kernel.dts

0fe134f488e883460232ee69f6419c7a  ./RK3399-EMB-3531-V2.2-Linux-General-ubuntu18.04_terminal-armhf_20200423/boot/Image
0fe134f488e883460232ee69f6419c7a  ./RK3399-EMB-3531-V2.2-Linux-General-debian_base-armhf_20200423/boot/Image
```



## 结论

* 公用同一套uboot dts
* 共用同一套kernel 和 dts

```text
ebb573c8101592e5152532cc30555cb7  dtb-kernel.dts
9e9a8eabb6f89a7cf5c10148d2809d09  dtb-uboot.dts
0fe134f488e883460232ee69f6419c7a  Image
```

