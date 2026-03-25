# tarvalds仓库master内核分支

## 基本信息

```shell

root@armbian:~# uname -a
Linux armbian 7.0.0-rc5-kdev #1 SMP PREEMPT Wed Mar 25 09:57:37 UTC 2026 aarch64 GNU/Linux
root@armbian:~# free -w -h
               total        used        free      shared     buffers       cache   available
Mem:           1.9Gi       132Mi       1.5Gi       6.3Mi        13Mi       333Mi       1.8Gi
Swap:          983Mi          0B       983Mi
root@armbian:~# lsblk
NAME         MAJ:MIN RM   SIZE RO TYPE MOUNTPOINTS
mmcblk0      179:0    0  14.7G  0 disk 
├─mmcblk0p1  179:1    0     4M  0 part 
├─mmcblk0p2  179:2    0     4M  0 part 
├─mmcblk0p3  179:3    0   512M  0 part 
└─mmcblk0p4  179:4    0  14.2G  0 part /var/log.hdd
                                       /
mmcblk0boot0 179:32   0     4M  1 disk 
mmcblk0boot1 179:64   0     4M  1 disk 
zram0        254:0    0 983.4M  0 disk [SWAP]
zram1        254:1    0    50M  0 disk /var/log
root@armbian:~# inxi -Fxxxz
System:
  Kernel: 7.0.0-rc5-kdev arch: aarch64 bits: 64 compiler: gcc v: 11.4.0
    clocksource: arch_sys_counter
  Console: pty pts/0 Distro: Armbian GNU/Linux 13 (trixie)
Machine:
  Type: ARM System: Rockchip EMB3531 details: N/A
CPU:
  Info: 6-core model: N/A variant-1: cortex-a53 variant-2: cortex-a72 bits: 64 type: MCP
    smt: <unsupported> arch: ARMv8 rev: 4 cache: L1: 416 KiB L2: 1.5 MiB
  Speed: N/A min/max: N/A cores: No per core speed data found. bogomips: N/A
  Features: Use -f option to see features
Graphics:
  Device-1: display-subsystem driver: rockchip_drm v: N/A bus-ID: N/A
    chip-ID: rockchip:display-subsystem class-ID: display-subsystem
  Device-2: rk3399-dw-hdmi driver: dwhdmi_rockchip v: N/A bus-ID: N/A chip-ID: rockchip:ff940000
    class-ID: hdmi
  Device-3: rk3399-mali driver: N/A bus-ID: N/A chip-ID: rockchip:ff9a0000 class-ID: gpu
  Display: server: No display server data found. Headless machine? tty: 156x37
  API: N/A Message: No API data available in console. Headless machine?
  Info: Tools: No graphics tools found.
Audio:
  Device-1: simple-audio-card driver: asoc_simple_card bus-ID: N/A
    chip-ID: simple-audio-card:es8316-sound class-ID: es8316-sound
  Device-2: rk3399-dw-hdmi driver: dwhdmi_rockchip bus-ID: N/A chip-ID: rockchip:ff940000
    class-ID: hdmi
  Device-3: simple-audio-card driver: asoc_simple_card bus-ID: N/A
    chip-ID: simple-audio-card:hdmi-sound class-ID: hdmi-sound
  API: ALSA v: k7.0.0-rc5-kdev status: kernel-api
Network:
  Device-1: rk3399-gmac driver: rk_gmac_dwmac v: N/A port: N/A bus-ID: N/A
    chip-ID: rockchip:fe300000 class-ID: ethernet
  IF: eth0 state: up speed: 1000 Mbps duplex: full mac: <filter>
Drives:
  Local Storage: total: 14.68 GiB used: 1.88 GiB (12.8%)
  ID-1: /dev/mmcblk0 vendor: Hynix model: HAG4a2 size: 14.68 GiB type: Removable tech: SSD
    serial: <filter> fw-rev: 0x8 scheme: GPT
Partition:
  ID-1: / size: 13.87 GiB used: 1.88 GiB (13.6%) fs: ext4 dev: /dev/mmcblk0p4
  ID-2: /var/log size: 46.8 MiB used: 632 KiB (1.3%) fs: ext4 dev: /dev/zram1
Swap:
  ID-1: swap-1 type: zram size: 983.4 MiB used: 0 KiB (0.0%) priority: 5 dev: /dev/zram0
Sensors:
  Src: /sys System Temperatures: cpu: 36.9 C mobo: N/A
  Fan Speeds (rpm): N/A
Info:
  Memory: total: 2 GiB available: 1.92 GiB used: 180.4 MiB (9.2%)
  Processes: 142 Power: uptime: 9m states: freeze,mem suspend: deep wakeups: 0 Init: systemd
    v: 257 default: graphical
  Packages: pm: dpkg pkgs: 486 Compilers: gcc: 14.2.0 Shell: Bash v: 5.2.37
    running-in: pty pts/0 (SSH) inxi: 3.3.38


```