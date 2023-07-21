# UbuntuWorking

To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.

leo@leo-VirtualBox:~$ lshw
WARNING: you should run this program as super-user.
leo-virtualbox              
    description: Computer
    width: 64 bits
    capabilities: smp vsyscall32
  *-core
       description: Motherboard
       physical id: 0
     *-memory
          description: System memory
          physical id: 0
          size: 6016MiB
     *-cpu
          product: AMD Ryzen 5 2600 Six-Core Processor
          vendor: Advanced Micro Devices [AMD]
          physical id: 1
          bus info: cpu@0
          version: 23.8.2
          width: 64 bits
          capabilities: fpu fpu_exception wp vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt rdtscp x86-64 constant_tsc rep_good nopl nonstop_tsc cpuid extd_apicid pni pclmulqdq ssse3 cx16 sse4_1 sse4_2 x2apic movbe popcnt aes xsave avx rdrand hypervisor lahf_lm cmp_legacy cr8_legacy abm sse4a misalignsse 3dnowprefetch ssbd vmmcall fsgsbase bmi1 avx2 bmi2 rdseed clflushopt arat
     *-pci
          description: Host bridge
          product: 440FX - 82441FX PMC [Natoma]
          vendor: Intel Corporation
          physical id: 100
          bus info: pci@0000:00:00.0
          version: 02
          width: 32 bits
          clock: 33MHz
        *-isa
             description: ISA bridge
             product: 82371SB PIIX3 ISA [Natoma/Triton II]
             vendor: Intel Corporation
             physical id: 1
             bus info: pci@0000:00:01.0
             version: 00
             width: 32 bits
             clock: 33MHz
             capabilities: isa bus_master
             configuration: latency=0
           *-pnp00:00
                product: PnP device PNP0303
                physical id: 0
                capabilities: pnp
                configuration: driver=i8042 kbd
           *-pnp00:01
                product: PnP device PNP0f03
                physical id: 1
                capabilities: pnp
                configuration: driver=i8042 aux
        *-ide
             description: IDE interface
             product: 82371AB/EB/MB PIIX4 IDE
             vendor: Intel Corporation
             physical id: 1.1
             bus info: pci@0000:00:01.1
             logical name: scsi1
             version: 01
             width: 32 bits
             clock: 33MHz
             capabilities: ide isa_compat_mode pci_native_mode bus_master emulated
             configuration: driver=ata_piix latency=64
             resources: irq:0 ioport:1f0(size=8) ioport:3f6 ioport:170(size=8) ioport:376 ioport:d000(size=16)
           *-cdrom
                description: DVD reader
                product: CD-ROM
                vendor: VBOX
                physical id: 0.0.0
                bus info: scsi@1:0.0.0
                logical name: /dev/cdrom
                logical name: /dev/sr0
                version: 1.0
                capabilities: removable audio dvd
                configuration: ansiversion=5 status=nodisc
        *-display
             description: VGA compatible controller
             product: SVGA II Adapter
             vendor: VMware
             physical id: 2
             bus info: pci@0000:00:02.0
             logical name: /dev/fb0
             version: 00
             width: 32 bits
             clock: 33MHz
             capabilities: vga_controller bus_master rom fb
             configuration: depth=32 driver=vmwgfx latency=64 resolution=2048,2048
             resources: irq:18 ioport:d010(size=16) memory:e0000000-e0ffffff memory:f0000000-f01fffff memory:c0000-dffff
        *-network
             description: Ethernet interface
             product: 82540EM Gigabit Ethernet Controller
             vendor: Intel Corporation
             physical id: 3
             bus info: pci@0000:00:03.0
             logical name: enp0s3
             version: 02
             serial: 08:00:27:fd:0e:ed
             size: 1Gbit/s
             capacity: 1Gbit/s
             width: 32 bits
             clock: 66MHz
             capabilities: bus_master cap_list ethernet physical tp 10bt 10bt-fd 100bt 100bt-fd 1000bt-fd autonegotiation
             configuration: autonegotiation=on broadcast=yes driver=e1000 driverversion=5.19.0-46-generic duplex=full ip=10.0.2.15 latency=64 link=yes mingnt=255 multicast=yes port=twisted pair speed=1Gbit/s
             resources: irq:19 memory:f0200000-f021ffff ioport:d020(size=8)
        *-generic
             description: System peripheral
             product: VirtualBox mouse integration
             vendor: InnoTek Systemberatung GmbH
             physical id: 4
             bus info: pci@0000:00:04.0
             logical name: input7
             logical name: /dev/input/event6
             logical name: /dev/input/js1
             logical name: /dev/input/mouse2
             version: 00
             width: 32 bits
             clock: 33MHz
             capabilities: pci
             configuration: driver=vboxguest latency=0
             resources: irq:20 ioport:d040(size=32) memory:f0400000-f07fffff memory:f0800000-f0803fff
        *-multimedia
             description: Multimedia audio controller
             product: 82801AA AC'97 Audio Controller
             vendor: Intel Corporation
             physical id: 5
             bus info: pci@0000:00:05.0
             logical name: card0
             logical name: /dev/snd/controlC0
             logical name: /dev/snd/pcmC0D0c
             logical name: /dev/snd/pcmC0D0p
             logical name: /dev/snd/pcmC0D1c
             version: 01
             width: 32 bits
             clock: 33MHz
             capabilities: bus_master
             configuration: driver=snd_intel8x0 latency=64
             resources: irq:21 ioport:d100(size=256) ioport:d200(size=64)
        *-usb:0
             description: USB controller
             product: KeyLargo/Intrepid USB
             vendor: Apple Inc.
             physical id: 6
             bus info: pci@0000:00:06.0
             version: 00
             width: 32 bits
             clock: 33MHz
             capabilities: ohci bus_master cap_list
             configuration: driver=ohci-pci latency=64
             resources: irq:22 memory:f0804000-f0804fff
        *-bridge
             description: Bridge
             product: 82371AB/EB/MB PIIX4 ACPI
             vendor: Intel Corporation
             physical id: 7
             bus info: pci@0000:00:07.0
             version: 08
             width: 32 bits
             clock: 33MHz
             capabilities: bridge
             configuration: driver=piix4_smbus latency=0
             resources: irq:9
        *-usb:1
             description: USB controller
             product: 82801FB/FBM/FR/FW/FRW (ICH6 Family) USB2 EHCI Controller
             vendor: Intel Corporation
             physical id: b
             bus info: pci@0000:00:0b.0
             version: 00
             width: 32 bits
             clock: 33MHz
             capabilities: ehci bus_master cap_list
             configuration: driver=ehci-pci latency=64
             resources: irq:19 memory:f0805000-f0805fff
        *-sata
             description: SATA controller
             product: 82801HM/HEM (ICH8M/ICH8M-E) SATA Controller [AHCI mode]
             vendor: Intel Corporation
             physical id: d
             bus info: pci@0000:00:0d.0
             version: 02
             width: 32 bits
             clock: 33MHz
             capabilities: sata ahci_1.0 bus_master cap_list
             configuration: driver=ahci latency=64
             resources: irq:21 ioport:d240(size=8) ioport:d248(size=4) ioport:d250(size=8) ioport:d258(size=4) ioport:d260(size=16) memory:f0806000-f0807fff
  *-input:0
       product: Power Button
       physical id: 1
       logical name: input0
       logical name: /dev/input/event0
       capabilities: platform
  *-input:1
       product: Sleep Button
       physical id: 2
       logical name: input1
       logical name: /dev/input/event1
       capabilities: platform
  *-input:2
       product: AT Translated Set 2 keyboard
       physical id: 3
       logical name: input2
       logical name: /dev/input/event2
       logical name: input2::capslock
       logical name: input2::numlock
       logical name: input2::scrolllock
       capabilities: i8042
  *-input:3
       product: Video Bus
       physical id: 4
       logical name: input4
       logical name: /dev/input/event3
       capabilities: platform
  *-input:4
       product: ImExPS/2 Generic Explorer Mouse
       physical id: 5
       logical name: input5
       logical name: /dev/input/event4
       logical name: /dev/input/mouse0
       capabilities: i8042
  *-input:5
       product: VirtualBox USB Tablet
       physical id: 6
       logical name: input6
       logical name: /dev/input/event5
       logical name: /dev/input/js0
       logical name: /dev/input/mouse1
       capabilities: usb
WARNING: output may be incomplete or inaccurate, you should run this program as super-user.
leo@leo-VirtualBox:~$ uname -a
Linux leo-VirtualBox 5.19.0-46-generic #47~22.04.1-Ubuntu SMP PREEMPT_DYNAMIC Wed Jun 21 15:35:31 UTC 2 x86_64 x86_64 x86_64 GNU/Linux
leo@leo-VirtualBox:~$ /cpuinfo
bash: /cpuinfo: No such file or directory
leo@leo-VirtualBox:~$ cat /proc/cpuinfo
processor	: 0
vendor_id	: AuthenticAMD
cpu family	: 23
model		: 8
model name	: AMD Ryzen 5 2600 Six-Core Processor
stepping	: 2
cpu MHz		: 3393.638
cache size	: 512 KB
physical id	: 0
siblings	: 6
core id		: 0
cpu cores	: 6
apicid		: 0
initial apicid	: 0
fpu		: yes
fpu_exception	: yes
cpuid level	: 13
wp		: yes
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt rdtscp lm constant_tsc rep_good nopl nonstop_tsc cpuid extd_apicid pni pclmulqdq ssse3 cx16 sse4_1 sse4_2 x2apic movbe popcnt aes xsave avx rdrand hypervisor lahf_lm cmp_legacy cr8_legacy abm sse4a misalignsse 3dnowprefetch ssbd vmmcall fsgsbase bmi1 avx2 bmi2 rdseed clflushopt arat
bugs		: fxsave_leak sysret_ss_attrs null_seg spectre_v1 spectre_v2 retbleed smt_rsb
bogomips	: 6787.27
TLB size	: 2560 4K pages
clflush size	: 64
cache_alignment	: 64
address sizes	: 48 bits physical, 48 bits virtual
power management:

processor	: 1
vendor_id	: AuthenticAMD
cpu family	: 23
model		: 8
model name	: AMD Ryzen 5 2600 Six-Core Processor
stepping	: 2
cpu MHz		: 3393.638
cache size	: 512 KB
physical id	: 0
siblings	: 6
core id		: 1
cpu cores	: 6
apicid		: 1
initial apicid	: 1
fpu		: yes
fpu_exception	: yes
cpuid level	: 13
wp		: yes
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt rdtscp lm constant_tsc rep_good nopl nonstop_tsc cpuid extd_apicid pni pclmulqdq ssse3 cx16 sse4_1 sse4_2 x2apic movbe popcnt aes xsave avx rdrand hypervisor lahf_lm cmp_legacy cr8_legacy abm sse4a misalignsse 3dnowprefetch ssbd vmmcall fsgsbase bmi1 avx2 bmi2 rdseed clflushopt arat
bugs		: fxsave_leak sysret_ss_attrs null_seg spectre_v1 spectre_v2 retbleed smt_rsb
bogomips	: 6787.27
TLB size	: 2560 4K pages
clflush size	: 64
cache_alignment	: 64
address sizes	: 48 bits physical, 48 bits virtual
power management:

processor	: 2
vendor_id	: AuthenticAMD
cpu family	: 23
model		: 8
model name	: AMD Ryzen 5 2600 Six-Core Processor
stepping	: 2
cpu MHz		: 3393.638
cache size	: 512 KB
physical id	: 0
siblings	: 6
core id		: 2
cpu cores	: 6
apicid		: 2
initial apicid	: 2
fpu		: yes
fpu_exception	: yes
cpuid level	: 13
wp		: yes
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt rdtscp lm constant_tsc rep_good nopl nonstop_tsc cpuid extd_apicid pni pclmulqdq ssse3 cx16 sse4_1 sse4_2 x2apic movbe popcnt aes xsave avx rdrand hypervisor lahf_lm cmp_legacy cr8_legacy abm sse4a misalignsse 3dnowprefetch ssbd vmmcall fsgsbase bmi1 avx2 bmi2 rdseed clflushopt arat
bugs		: fxsave_leak sysret_ss_attrs null_seg spectre_v1 spectre_v2 retbleed smt_rsb
bogomips	: 6787.27
TLB size	: 2560 4K pages
clflush size	: 64
cache_alignment	: 64
address sizes	: 48 bits physical, 48 bits virtual
power management:

processor	: 3
vendor_id	: AuthenticAMD
cpu family	: 23
model		: 8
model name	: AMD Ryzen 5 2600 Six-Core Processor
stepping	: 2
cpu MHz		: 3393.638
cache size	: 512 KB
physical id	: 0
siblings	: 6
core id		: 3
cpu cores	: 6
apicid		: 3
initial apicid	: 3
fpu		: yes
fpu_exception	: yes
cpuid level	: 13
wp		: yes
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt rdtscp lm constant_tsc rep_good nopl nonstop_tsc cpuid extd_apicid pni pclmulqdq ssse3 cx16 sse4_1 sse4_2 x2apic movbe popcnt aes xsave avx rdrand hypervisor lahf_lm cmp_legacy cr8_legacy abm sse4a misalignsse 3dnowprefetch ssbd vmmcall fsgsbase bmi1 avx2 bmi2 rdseed clflushopt arat
bugs		: fxsave_leak sysret_ss_attrs null_seg spectre_v1 spectre_v2 retbleed smt_rsb
bogomips	: 6787.27
TLB size	: 2560 4K pages
clflush size	: 64
cache_alignment	: 64
address sizes	: 48 bits physical, 48 bits virtual
power management:

processor	: 4
vendor_id	: AuthenticAMD
cpu family	: 23
model		: 8
model name	: AMD Ryzen 5 2600 Six-Core Processor
stepping	: 2
cpu MHz		: 3393.638
cache size	: 512 KB
physical id	: 0
siblings	: 6
core id		: 4
cpu cores	: 6
apicid		: 4
initial apicid	: 4
fpu		: yes
fpu_exception	: yes
cpuid level	: 13
wp		: yes
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt rdtscp lm constant_tsc rep_good nopl nonstop_tsc cpuid extd_apicid pni pclmulqdq ssse3 cx16 sse4_1 sse4_2 x2apic movbe popcnt aes xsave avx rdrand hypervisor lahf_lm cmp_legacy cr8_legacy abm sse4a misalignsse 3dnowprefetch ssbd vmmcall fsgsbase bmi1 avx2 bmi2 rdseed clflushopt arat
bugs		: fxsave_leak sysret_ss_attrs null_seg spectre_v1 spectre_v2 retbleed smt_rsb
bogomips	: 6787.27
TLB size	: 2560 4K pages
clflush size	: 64
cache_alignment	: 64
address sizes	: 48 bits physical, 48 bits virtual
power management:

processor	: 5
vendor_id	: AuthenticAMD
cpu family	: 23
model		: 8
model name	: AMD Ryzen 5 2600 Six-Core Processor
stepping	: 2
cpu MHz		: 3393.638
cache size	: 512 KB
physical id	: 0
siblings	: 6
core id		: 5
cpu cores	: 6
apicid		: 5
initial apicid	: 5
fpu		: yes
fpu_exception	: yes
cpuid level	: 13
wp		: yes
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt rdtscp lm constant_tsc rep_good nopl nonstop_tsc cpuid extd_apicid pni pclmulqdq ssse3 cx16 sse4_1 sse4_2 x2apic movbe popcnt aes xsave avx rdrand hypervisor lahf_lm cmp_legacy cr8_legacy abm sse4a misalignsse 3dnowprefetch ssbd vmmcall fsgsbase bmi1 avx2 bmi2 rdseed clflushopt arat
bugs		: fxsave_leak sysret_ss_attrs null_seg spectre_v1 spectre_v2 retbleed smt_rsb
bogomips	: 6787.27
TLB size	: 2560 4K pages
clflush size	: 64
cache_alignment	: 64
address sizes	: 48 bits physical, 48 bits virtual
power management:

leo@leo-VirtualBox:~$ cat /proc/meminfo
MemTotal:        5917220 kB
MemFree:         2153620 kB
MemAvailable:    3671088 kB
Buffers:           53752 kB
Cached:          1705656 kB
SwapCached:            0 kB
Active:           583256 kB
Inactive:        2784744 kB
Active(anon):       3236 kB
Inactive(anon):  1677216 kB
Active(file):     580020 kB
Inactive(file):  1107528 kB
Unevictable:          32 kB
Mlocked:              32 kB
SwapTotal:       2097148 kB
SwapFree:        2097148 kB
Zswap:                 0 kB
Zswapped:              0 kB
Dirty:               132 kB
Writeback:             0 kB
AnonPages:       1608672 kB
Mapped:           585744 kB
Shmem:             78124 kB
KReclaimable:      80120 kB
Slab:             202404 kB
SReclaimable:      80120 kB
SUnreclaim:       122284 kB
KernelStack:       12848 kB
PageTables:        25320 kB
NFS_Unstable:          0 kB
Bounce:                0 kB
WritebackTmp:          0 kB
CommitLimit:     5055756 kB
Committed_AS:    5998196 kB
VmallocTotal:   34359738367 kB
VmallocUsed:       57064 kB
VmallocChunk:          0 kB
Percpu:             7872 kB
HardwareCorrupted:     0 kB
AnonHugePages:         0 kB
ShmemHugePages:        0 kB
ShmemPmdMapped:        0 kB
FileHugePages:         0 kB
FilePmdMapped:         0 kB
HugePages_Total:       0
HugePages_Free:        0
HugePages_Rsvd:        0
HugePages_Surp:        0
Hugepagesize:       2048 kB
Hugetlb:               0 kB
DirectMap4k:      171968 kB
DirectMap2M:     5971968 kB
leo@leo-VirtualBox:~$ dmesg
dmesg: read kernel buffer failed: Operation not permitted
leo@leo-VirtualBox:~$ pstree -p
systemd(1)─┬─ModemManager(851)─┬─{ModemManager}(877)
           │                   └─{ModemManager}(881)
           ├─NetworkManager(768)─┬─{NetworkManager}(839)
           │                     └─{NetworkManager}(841)
           ├─accounts-daemon(759)─┬─{accounts-daemon}(807)
           │                      └─{accounts-daemon}(838)
           ├─acpid(760)
           ├─avahi-daemon(763)───avahi-daemon(801)
           ├─colord(1708)─┬─{colord}(1710)
           │              └─{colord}(1712)
           ├─cron(764)
           ├─cups-browsed(915)─┬─{cups-browsed}(2317)
           │                   └─{cups-browsed}(2318)
           ├─cupsd(845)───dbus(890)
           ├─dbus-daemon(765)
           ├─fwupd(1889)─┬─{fwupd}(1890)
           │             ├─{fwupd}(1891)
           │             ├─{fwupd}(1892)
           │             └─{fwupd}(1893)
           ├─gdm3(880)─┬─gdm-session-wor(892)─┬─gdm-wayland-ses(990)─┬─gnome-se+
           │           │                      │                      ├─{gdm-way+
           │           │                      │                      └─{gdm-way+
           │           │                      ├─{gdm-session-wor}(893)
           │           │                      └─{gdm-session-wor}(895)
           │           ├─{gdm3}(883)
           │           └─{gdm3}(884)
           ├─gnome-keyring-d(976)─┬─{gnome-keyring-d}(977)
           │                      ├─{gnome-keyring-d}(979)
           │                      └─{gnome-keyring-d}(1064)
           ├─irqbalance(776)───{irqbalance}(797)
           ├─kerneloops(929)
           ├─kerneloops(935)
           ├─networkd-dispat(778)
           ├─packagekitd(1363)─┬─{packagekitd}(1364)
           │                   └─{packagekitd}(1365)
           ├─polkitd(781)─┬─{polkitd}(791)
           │              └─{polkitd}(837)
           ├─power-profiles-(784)─┬─{power-profiles-}(819)
           │                      └─{power-profiles-}(835)
           ├─rsyslogd(785)─┬─{rsyslogd}(802)
           │               ├─{rsyslogd}(803)
           │               └─{rsyslogd}(804)
           ├─rtkit-daemon(978)─┬─{rtkit-daemon}(985)
           │                   └─{rtkit-daemon}(986)
           ├─snapd(789)─┬─{snapd}(1006)
           │            ├─{snapd}(1007)
           │            ├─{snapd}(1008)
           │            ├─{snapd}(1009)
           │            ├─{snapd}(1013)
           │            ├─{snapd}(1053)
           │            ├─{snapd}(1097)
           │            ├─{snapd}(1109)
           │            ├─{snapd}(1111)
           │            ├─{snapd}(1112)
           │            ├─{snapd}(1127)
           │            ├─{snapd}(1187)
           │            ├─{snapd}(1188)
           │            ├─{snapd}(1215)
           │            └─{snapd}(1216)
           ├─switcheroo-cont(792)─┬─{switcheroo-cont}(832)
           │                      └─{switcheroo-cont}(840)
           ├─systemd(961)─┬─(sd-pam)(962)
           │              ├─at-spi2-registr(1383)─┬─{at-spi2-registr}(1387)
           │              │                       └─{at-spi2-registr}(1390)
           │              ├─dbus-daemon(992)
           │              ├─dconf-service(1326)─┬─{dconf-service}(1332)
           │              │                     └─{dconf-service}(1336)
           │              ├─evolution-addre(1330)─┬─{evolution-addre}(1339)
           │              │                       ├─{evolution-addre}(1342)
           │              │                       ├─{evolution-addre}(1348)
           │              │                       ├─{evolution-addre}(1349)
           │              │                       └─{evolution-addre}(1356)
           │              ├─evolution-calen(1278)─┬─{evolution-calen}(1280)
           │              │                       ├─{evolution-calen}(1282)
           │              │                       ├─{evolution-calen}(1303)
           │              │                       ├─{evolution-calen}(1304)
           │              │                       ├─{evolution-calen}(1317)
           │              │                       ├─{evolution-calen}(1322)
           │              │                       ├─{evolution-calen}(1325)
           │              │                       └─{evolution-calen}(1335)
           │              ├─evolution-sourc(1259)─┬─{evolution-sourc}(1260)
           │              │                       ├─{evolution-sourc}(1261)
           │              │                       └─{evolution-sourc}(1262)
           │              ├─gjs(1384)─┬─{gjs}(1386)
           │              │           ├─{gjs}(1389)
           │              │           ├─{gjs}(1394)
           │              │           ├─{gjs}(1395)
           │              │           ├─{gjs}(1396)
           │              │           ├─{gjs}(1398)
           │              │           ├─{gjs}(1399)
           │              │           └─{gjs}(1400)
           │              ├─gjs(1755)─┬─{gjs}(1757)
           │              │           ├─{gjs}(1758)
           │              │           ├─{gjs}(1759)
           │              │           ├─{gjs}(1760)
           │              │           ├─{gjs}(1761)
           │              │           ├─{gjs}(1762)
           │              │           ├─{gjs}(1763)
           │              │           └─{gjs}(1764)
           │              ├─gnome-calendar(2355)─┬─{gnome-calendar}(2377)
           │              │                      ├─{gnome-calendar}(2379)
           │              │                      ├─{gnome-calendar}(2391)
           │              │                      ├─{gnome-calendar}(2426)
           │              │                      └─{gnome-calendar}(2432)
           │              ├─gnome-session-b(1069)─┬─at-spi-bus-laun(1084)─┬─dbu+
           │              │                       │                       ├─{at+
           │              │                       │                       ├─{at+
           │              │                       │                       └─{at+
           │              │                       ├─evolution-alarm(1462)─┬─{ev+
           │              │                       │                       ├─{ev+
           │              │                       │                       ├─{ev+
           │              │                       │                       ├─{ev+
           │              │                       │                       └─{ev+
           │              │                       ├─gsd-disk-utilit(1464)─┬─{gs+
           │              │                       │                       └─{gs+
           │              │                       ├─update-notifier(3951)─┬─{up+
           │              │                       │                       ├─{up+
           │              │                       │                       └─{up+
           │              │                       ├─{gnome-session-b}(1071)
           │              │                       ├─{gnome-session-b}(1072)
           │              │                       └─{gnome-session-b}(1074)
           │              ├─gnome-session-c(1057)───{gnome-session-c}(1063)
           │              ├─gnome-shell(1088)─┬─Xwayland(2957)
           │              │                   ├─firefox(2624)─┬─Isolated Web Co+
           │              │                   │               ├─Isolated Web Co+
           │              │                   │               ├─Privileged Cont+
           │              │                   │               ├─RDD Process(392+
           │              │                   │               ├─Socket Process(+
           │              │                   │               ├─Utility Process+
           │              │                   │               ├─Web Content(385+
           │              │                   │               ├─Web Content(388+
           │              │                   │               ├─Web Content(411+
           │              │                   │               ├─WebExtensions(3+
           │              │                   │               ├─{firefox}(3027)
           │              │                   │               ├─{firefox}(3028)
           │              │                   │               ├─{firefox}(3042)
           │              │                   │               ├─{firefox}(3043)
           │              │                   │               ├─{firefox}(3044)
           │              │                   │               ├─{firefox}(3045)
           │              │                   │               ├─{firefox}(3047)
           │              │                   │               ├─{firefox}(3050)
           │              │                   │               ├─{firefox}(3052)
           │              │                   │               ├─{firefox}(3053)
           │              │                   │               ├─{firefox}(3054)
           │              │                   │               ├─{firefox}(3055)
           │              │                   │               ├─{firefox}(3056)
           │              │                   │               ├─{firefox}(3057)
           │              │                   │               ├─{firefox}(3058)
           │              │                   │               ├─{firefox}(3059)
           │              │                   │               ├─{firefox}(3081)
           │              │                   │               ├─{firefox}(3100)
           │              │                   │               ├─{firefox}(3101)
           │              │                   │               ├─{firefox}(3105)
           │              │                   │               ├─{firefox}(3182)
           │              │                   │               ├─{firefox}(3183)
           │              │                   │               ├─{firefox}(3184)
           │              │                   │               ├─{firefox}(3185)
           │              │                   │               ├─{firefox}(3186)
           │              │                   │               ├─{firefox}(3187)
           │              │                   │               ├─{firefox}(3188)
           │              │                   │               ├─{firefox}(3189)
           │              │                   │               ├─{firefox}(3190)
           │              │                   │               ├─{firefox}(3191)
           │              │                   │               ├─{firefox}(3192)
           │              │                   │               ├─{firefox}(3193)
           │              │                   │               ├─{firefox}(3194)
           │              │                   │               ├─{firefox}(3195)
           │              │                   │               ├─{firefox}(3196)
           │              │                   │               ├─{firefox}(3198)
           │              │                   │               ├─{firefox}(3199)
           │              │                   │               ├─{firefox}(3200)
           │              │                   │               ├─{firefox}(3201)
           │              │                   │               ├─{firefox}(3206)
           │              │                   │               ├─{firefox}(3209)
           │              │                   │               ├─{firefox}(3223)
           │              │                   │               ├─{firefox}(3240)
           │              │                   │               ├─{firefox}(3241)
           │              │                   │               ├─{firefox}(3242)
           │              │                   │               ├─{firefox}(3243)
           │              │                   │               ├─{firefox}(3247)
           │              │                   │               ├─{firefox}(3249)
           │              │                   │               ├─{firefox}(3250)
           │              │                   │               ├─{firefox}(3251)
           │              │                   │               ├─{firefox}(3257)
           │              │                   │               ├─{firefox}(3259)
           │              │                   │               ├─{firefox}(3260)
           │              │                   │               ├─{firefox}(3261)
           │              │                   │               ├─{firefox}(3275)
           │              │                   │               ├─{firefox}(3276)
           │              │                   │               ├─{firefox}(3278)
           │              │                   │               ├─{firefox}(3279)
           │              │                   │               ├─{firefox}(3280)
           │              │                   │               ├─{firefox}(3281)
           │              │                   │               ├─{firefox}(3413)
           │              │                   │               ├─{firefox}(3414)
           │              │                   │               ├─{firefox}(3420)
           │              │                   │               ├─{firefox}(3421)
           │              │                   │               ├─{firefox}(3427)
           │              │                   │               ├─{firefox}(3584)
           │              │                   │               ├─{firefox}(3594)
           │              │                   │               ├─{firefox}(3709)
           │              │                   │               ├─{firefox}(3713)
           │              │                   │               ├─{firefox}(3727)
           │              │                   │               ├─{firefox}(3750)
           │              │                   │               ├─{firefox}(3785)
           │              │                   │               ├─{firefox}(3789)
           │              │                   │               ├─{firefox}(3794)
           │              │                   │               ├─{firefox}(3796)
           │              │                   │               ├─{firefox}(3797)
           │              │                   │               ├─{firefox}(3804)
           │              │                   │               ├─{firefox}(3828)
           │              │                   │               ├─{firefox}(3829)
           │              │                   │               ├─{firefox}(3830)
           │              │                   │               ├─{firefox}(3831)
           │              │                   │               ├─{firefox}(3861)
           │              │                   │               ├─{firefox}(3889)
           │              │                   │               ├─{firefox}(3909)
           │              │                   │               ├─{firefox}(3930)
           │              │                   │               ├─{firefox}(3932)
           │              │                   │               ├─{firefox}(4046)
           │              │                   │               ├─{firefox}(4047)
           │              │                   │               ├─{firefox}(4048)
           │              │                   │               ├─{firefox}(4049)
           │              │                   │               ├─{firefox}(4078)
           │              │                   │               ├─{firefox}(4090)
           │              │                   │               ├─{firefox}(4091)
           │              │                   │               ├─{firefox}(4092)
           │              │                   │               ├─{firefox}(4093)
           │              │                   │               ├─{firefox}(4094)
           │              │                   │               ├─{firefox}(4095)
           │              │                   │               ├─{firefox}(4096)
           │              │                   │               ├─{firefox}(4097)
           │              │                   │               ├─{firefox}(4098)
           │              │                   │               ├─{firefox}(4099)
           │              │                   │               ├─{firefox}(4100)
           │              │                   │               ├─{firefox}(4101)
           │              │                   │               ├─{firefox}(4102)
           │              │                   │               ├─{firefox}(4111)
           │              │                   │               ├─{firefox}(4212)
           │              │                   │               ├─{firefox}(4276)
           │              │                   │               ├─{firefox}(4277)
           │              │                   │               ├─{firefox}(4278)
           │              │                   │               ├─{firefox}(4279)
           │              │                   │               ├─{firefox}(4287)
           │              │                   │               ├─{firefox}(4292)
           │              │                   │               ├─{firefox}(4293)
           │              │                   │               ├─{firefox}(4294)
           │              │                   │               ├─{firefox}(4295)
           │              │                   │               ├─{firefox}(4298)
           │              │                   │               ├─{firefox}(4299)
           │              │                   │               ├─{firefox}(4300)
           │              │                   │               ├─{firefox}(4301)
           │              │                   │               └─{firefox}(4328)
           │              │                   ├─gjs(1769)─┬─{gjs}(1772)
           │              │                   │           ├─{gjs}(1773)
           │              │                   │           ├─{gjs}(1774)
           │              │                   │           ├─{gjs}(1775)
           │              │                   │           ├─{gjs}(1776)
           │              │                   │           ├─{gjs}(1777)
           │              │                   │           ├─{gjs}(1778)
           │              │                   │           ├─{gjs}(1779)
           │              │                   │           └─{gjs}(1805)
           │              │                   ├─{gnome-shell}(1122)
           │              │                   ├─{gnome-shell}(1131)
           │              │                   ├─{gnome-shell}(1136)
           │              │                   ├─{gnome-shell}(1195)
           │              │                   ├─{gnome-shell}(1196)
           │              │                   ├─{gnome-shell}(1197)
           │              │                   ├─{gnome-shell}(1198)
           │              │                   ├─{gnome-shell}(1199)
           │              │                   ├─{gnome-shell}(1200)
           │              │                   ├─{gnome-shell}(1201)
           │              │                   ├─{gnome-shell}(1202)
           │              │                   ├─{gnome-shell}(1203)
           │              │                   ├─{gnome-shell}(1204)
           │              │                   ├─{gnome-shell}(1205)
           │              │                   ├─{gnome-shell}(1206)
           │              │                   ├─{gnome-shell}(1207)
           │              │                   ├─{gnome-shell}(1214)
           │              │                   ├─{gnome-shell}(1218)
           │              │                   ├─{gnome-shell}(1219)
           │              │                   ├─{gnome-shell}(1220)
           │              │                   ├─{gnome-shell}(1221)
           │              │                   ├─{gnome-shell}(1222)
           │              │                   ├─{gnome-shell}(1223)
           │              │                   ├─{gnome-shell}(2996)
           │              │                   └─{gnome-shell}(4235)
           │              ├─gnome-shell-cal(1253)─┬─{gnome-shell-cal}(1254)
           │              │                       ├─{gnome-shell-cal}(1256)
           │              │                       ├─{gnome-shell-cal}(1257)
           │              │                       ├─{gnome-shell-cal}(1258)
           │              │                       └─{gnome-shell-cal}(1276)
           │              ├─gnome-terminal-(4350)─┬─bash(4368)───pstree(4388)
           │              │                       ├─{gnome-terminal-}(4351)
           │              │                       ├─{gnome-terminal-}(4353)
           │              │                       └─{gnome-terminal-}(4354)
           │              ├─goa-daemon(1266)─┬─{goa-daemon}(1283)
           │              │                  ├─{goa-daemon}(1285)
           │              │                  └─{goa-daemon}(1286)
           │              ├─goa-identity-se(1289)─┬─{goa-identity-se}(1293)
           │              │                       └─{goa-identity-se}(1296)
           │              ├─gsd-a11y-settin(1393)─┬─{gsd-a11y-settin}(1414)
           │              │                       ├─{gsd-a11y-settin}(1416)
           │              │                       └─{gsd-a11y-settin}(1455)
           │              ├─gsd-color(1403)─┬─{gsd-color}(1452)
           │              │                 ├─{gsd-color}(1459)
           │              │                 └─{gsd-color}(1506)
           │              ├─gsd-datetime(1405)─┬─{gsd-datetime}(1420)
           │              │                    ├─{gsd-datetime}(1425)
           │              │                    └─{gsd-datetime}(1456)
           │              ├─gsd-housekeepin(1408)─┬─{gsd-housekeepin}(1415)
           │              │                       ├─{gsd-housekeepin}(1418)
           │              │                       └─{gsd-housekeepin}(1454)
           │              ├─gsd-keyboard(1412)─┬─{gsd-keyboard}(1421)
           │              │                    ├─{gsd-keyboard}(1424)
           │              │                    └─{gsd-keyboard}(1466)
           │              ├─gsd-media-keys(1419)─┬─{gsd-media-keys}(1494)
           │              │                      ├─{gsd-media-keys}(1499)
           │              │                      └─{gsd-media-keys}(1510)
           │              ├─gsd-power(1426)─┬─{gsd-power}(1448)
           │              │                 ├─{gsd-power}(1450)
           │              │                 └─{gsd-power}(1486)
           │              ├─gsd-print-notif(1427)─┬─{gsd-print-notif}(1435)
           │              │                       └─{gsd-print-notif}(1469)
           │              ├─gsd-printer(1609)─┬─{gsd-printer}(1615)
           │              │                   └─{gsd-printer}(1616)
           │              ├─gsd-rfkill(1428)─┬─{gsd-rfkill}(1438)
           │              │                  └─{gsd-rfkill}(1467)
           │              ├─gsd-screensaver(1429)─┬─{gsd-screensaver}(1437)
           │              │                       └─{gsd-screensaver}(1465)
           │              ├─gsd-sharing(1430)─┬─{gsd-sharing}(1443)
           │              │                   ├─{gsd-sharing}(1460)
           │              │                   └─{gsd-sharing}(1483)
           │              ├─gsd-smartcard(1432)─┬─{gsd-smartcard}(1446)
           │              │                     ├─{gsd-smartcard}(1485)
           │              │                     └─{gsd-smartcard}(1552)
           │              ├─gsd-sound(1433)─┬─{gsd-sound}(1440)
           │              │                 ├─{gsd-sound}(1468)
           │              │                 └─{gsd-sound}(1551)
           │              ├─gsd-wacom(1436)─┬─{gsd-wacom}(1476)
           │              │                 ├─{gsd-wacom}(1481)
           │              │                 └─{gsd-wacom}(1509)
           │              ├─gsd-xsettings(2961)─┬─{gsd-xsettings}(2963)
           │              │                     ├─{gsd-xsettings}(2964)
           │              │                     └─{gsd-xsettings}(2965)
           │              ├─gvfs-afc-volume(1321)─┬─{gvfs-afc-volume}(1327)
           │              │                       ├─{gvfs-afc-volume}(1328)
           │              │                       └─{gvfs-afc-volume}(1331)
           │              ├─gvfs-goa-volume(1338)─┬─{gvfs-goa-volume}(1341)
           │              │                       └─{gvfs-goa-volume}(1343)
           │              ├─gvfs-gphoto2-vo(1354)─┬─{gvfs-gphoto2-vo}(1357)
           │              │                       └─{gvfs-gphoto2-vo}(1359)
           │              ├─gvfs-mtp-volume(1347)─┬─{gvfs-mtp-volume}(1351)
           │              │                       └─{gvfs-mtp-volume}(1353)
           │              ├─gvfs-udisks2-vo(1290)─┬─{gvfs-udisks2-vo}(1292)
           │              │                       ├─{gvfs-udisks2-vo}(1294)
           │              │                       └─{gvfs-udisks2-vo}(1309)
           │              ├─gvfsd(999)─┬─gvfsd-trash(1370)─┬─{gvfsd-trash}(1371+
           │              │            │                   └─{gvfsd-trash}(1372+
           │              │            ├─{gvfsd}(1010)
           │              │            └─{gvfsd}(1012)
           │              ├─gvfsd-fuse(1025)─┬─{gvfsd-fuse}(1035)
           │              │                  ├─{gvfsd-fuse}(1036)
           │              │                  ├─{gvfsd-fuse}(1037)
           │              │                  ├─{gvfsd-fuse}(1038)
           │              │                  └─{gvfsd-fuse}(1040)
           │              ├─gvfsd-metadata(1863)─┬─{gvfsd-metadata}(1864)
           │              │                      └─{gvfsd-metadata}(1865)
           │              ├─ibus-portal(1527)─┬─{ibus-portal}(1531)
           │              │                   └─{ibus-portal}(1536)
           │              ├─ibus-x11(2986)─┬─{ibus-x11}(2988)
           │              │                └─{ibus-x11}(2989)
           │              ├─pipewire(969)───{pipewire}(997)
           │              ├─pipewire-media-(970)───{pipewire-media-}(989)
           │              ├─pulseaudio(971)─┬─{pulseaudio}(1034)
           │              │                 ├─{pulseaudio}(1039)
           │              │                 └─{pulseaudio}(1049)
           │              ├─seahorse(2358)─┬─{seahorse}(2376)
           │              │                ├─{seahorse}(2382)
           │              │                └─{seahorse}(2390)
           │              ├─sh(1392)───ibus-daemon(1401)─┬─ibus-dconf(1516)─┬─{+
           │              │                              │                  ├─{+
           │              │                              │                  └─{+
           │              │                              ├─ibus-engine-sim(1602+
           │              │                              ├─ibus-extension-(1519+
           │              │                              ├─{ibus-daemon}(1463)
           │              │                              └─{ibus-daemon}(1484)
           │              ├─snap(3286)─┬─{snap}(3294)
           │              │            ├─{snap}(3295)
           │              │            ├─{snap}(3296)
           │              │            ├─{snap}(3297)
           │              │            ├─{snap}(3298)
           │              │            ├─{snap}(3299)
           │              │            ├─{snap}(3300)
           │              │            ├─{snap}(3301)
           │              │            ├─{snap}(3302)
           │              │            └─{snap}(4143)
           │              ├─snap-store(1559)─┬─{snap-store}(1743)
           │              │                  ├─{snap-store}(1751)
           │              │                  ├─{snap-store}(1752)
           │              │                  └─{snap-store}(1852)
           │              ├─snapd-desktop-i(972)───snapd-desktop-i(1378)─┬─{sna+
           │              │                                              ├─{sna+
           │              │                                              └─{sna+
           │              ├─tracker-miner-f(1714)─┬─{tracker-miner-f}(1716)
           │              │                       ├─{tracker-miner-f}(1717)
           │              │                       ├─{tracker-miner-f}(1718)
           │              │                       ├─{tracker-miner-f}(1720)
           │              │                       └─{tracker-miner-f}(1767)
           │              ├─xdg-desktop-por(1461)─┬─{xdg-desktop-por}(1479)
           │              │                       ├─{xdg-desktop-por}(1511)
           │              │                       ├─{xdg-desktop-por}(1665)
           │              │                       ├─{xdg-desktop-por}(1802)
           │              │                       └─{xdg-desktop-por}(1803)
           │              ├─xdg-desktop-por(1557)─┬─{xdg-desktop-por}(1568)
           │              │                       ├─{xdg-desktop-por}(1570)
           │              │                       └─{xdg-desktop-por}(1583)
           │              ├─xdg-desktop-por(1667)─┬─{xdg-desktop-por}(1672)
           │              │                       ├─{xdg-desktop-por}(1674)
           │              │                       └─{xdg-desktop-por}(1675)
           │              ├─xdg-document-po(1152)─┬─fusermount3(1174)
           │              │                       ├─{xdg-document-po}(1160)
           │              │                       ├─{xdg-document-po}(1162)
           │              │                       ├─{xdg-document-po}(1173)
           │              │                       ├─{xdg-document-po}(1175)
           │              │                       └─{xdg-document-po}(1176)
           │              └─xdg-permission-(1163)─┬─{xdg-permission-}(1164)
           │                                      └─{xdg-permission-}(1166)
           ├─systemd-journal(460)
           ├─systemd-logind(796)
           ├─systemd-oomd(719)
           ├─systemd-resolve(720)
           ├─systemd-timesyn(721)───{systemd-timesyn}(733)
           ├─systemd-udevd(512)
           ├─udisksd(798)─┬─{udisksd}(820)
           │              ├─{udisksd}(836)
           │              ├─{udisksd}(870)
           │              └─{udisksd}(903)
           ├─unattended-upgr(869)───{unattended-upgr}(907)
           ├─upowerd(1263)─┬─{upowerd}(1268)
           │               └─{upowerd}(1269)
           └─wpa_supplicant(799)
leo@leo-VirtualBox:~$ PrtScn
PrtScn: command not found
leo@leo-VirtualBox:~$ apt list --installed
Listing... Done
accountsservice/jammy-updates,jammy-security,now 22.07.5-2ubuntu1.4 amd64 [installed,automatic]
acl/jammy,now 2.3.1-1 amd64 [installed,automatic]
acpi-support/jammy,now 0.144 amd64 [installed,automatic]
acpid/jammy,now 1:2.0.33-1ubuntu1 amd64 [installed,automatic]
adduser/jammy,jammy,now 3.118ubuntu5 all [installed,automatic]
adwaita-icon-theme/jammy,jammy,now 41.0-1ubuntu1 all [installed,automatic]
aisleriot/jammy,now 1:3.22.22-1 amd64 [installed,automatic]
alsa-base/jammy,jammy,now 1.0.25+dfsg-0ubuntu7 all [installed,automatic]
alsa-topology-conf/jammy,jammy,now 1.2.5.1-2 all [installed,automatic]
alsa-ucm-conf/now 1.2.6.3-1ubuntu1.6 all [installed,upgradable to: 1.2.6.3-1ubuntu1.7]
alsa-utils/jammy,now 1.2.6-1ubuntu1 amd64 [installed,automatic]
amd64-microcode/jammy,now 3.20191218.1ubuntu2 amd64 [installed,automatic]
anacron/jammy,now 2.3-31ubuntu2 amd64 [installed,automatic]
apg/jammy,now 2.2.3.dfsg.1-5build2 amd64 [installed,automatic]
apparmor/jammy-updates,now 3.0.4-2ubuntu2.2 amd64 [installed,automatic]
apport-gtk/jammy-updates,jammy-updates,now 2.20.11-0ubuntu82.5 all [installed,automatic]
apport-symptoms/jammy,jammy,now 0.24 all [installed,automatic]
apport/jammy-updates,jammy-updates,now 2.20.11-0ubuntu82.5 all [installed,automatic]
appstream/jammy,now 0.15.2-2 amd64 [installed,automatic]
apt-config-icons-hidpi/jammy,jammy,now 0.15.2-2 all [installed,automatic]
apt-config-icons/jammy,jammy,now 0.15.2-2 all [installed,automatic]
apt-utils/jammy-updates,now 2.4.9 amd64 [installed,automatic]
apt/jammy-updates,now 2.4.9 amd64 [installed,automatic]
aptdaemon-data/jammy,jammy,now 1.1.1+bzr982-0ubuntu39 all [installed,automatic]
aptdaemon/jammy,jammy,now 1.1.1+bzr982-0ubuntu39 all [installed,automatic]
apturl-common/jammy,now 0.5.2ubuntu22 amd64 [installed,automatic]
apturl/jammy,now 0.5.2ubuntu22 amd64 [installed,automatic]
aspell-en/jammy,jammy,now 2018.04.16-0-1 all [installed,automatic]
aspell/jammy,now 0.60.8-4build1 amd64 [installed,automatic]
at-spi2-core/jammy,now 2.44.0-3 amd64 [installed,automatic]
avahi-autoipd/jammy-updates,jammy-security,now 0.8-5ubuntu5.1 amd64 [installed,automatic]
avahi-daemon/jammy-updates,jammy-security,now 0.8-5ubuntu5.1 amd64 [installed,automatic]
avahi-utils/jammy-updates,jammy-security,now 0.8-5ubuntu5.1 amd64 [installed,automatic]
baobab/jammy,now 41.0-2 amd64 [installed,automatic]
base-files/jammy-updates,now 12ubuntu4.3 amd64 [installed,automatic]
base-passwd/jammy,now 3.5.52build1 amd64 [installed]
bash-completion/jammy,jammy,now 1:2.11-5ubuntu1 all [installed,automatic]
bash/jammy,now 5.1-6ubuntu1 amd64 [installed,automatic]
bc/jammy,now 1.07.1-3build1 amd64 [installed,automatic]
bind9-dnsutils/jammy-updates,jammy-security,now 1:9.18.12-0ubuntu0.22.04.2 amd64 [installed,automatic]
bind9-host/jammy-updates,jammy-security,now 1:9.18.12-0ubuntu0.22.04.2 amd64 [installed,automatic]
bind9-libs/jammy-updates,jammy-security,now 1:9.18.12-0ubuntu0.22.04.2 amd64 [installed,automatic]
bluez-cups/jammy,now 5.64-0ubuntu1 amd64 [installed,automatic]
bluez-obexd/jammy,now 5.64-0ubuntu1 amd64 [installed,automatic]
bluez/jammy,now 5.64-0ubuntu1 amd64 [installed,automatic]
bolt/jammy,now 0.9.2-1 amd64 [installed,automatic]
branding-ubuntu/jammy,jammy,now 0.10 all [installed,automatic]
brltty/jammy-updates,now 6.4-4ubuntu3 amd64 [installed,automatic]
bsdextrautils/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
bsdutils/jammy,now 1:2.37.2-4ubuntu3 amd64 [installed]
btrfs-progs/jammy,now 5.16.2-1 amd64 [installed,automatic]
bubblewrap/jammy,now 0.6.1-1 amd64 [installed,automatic]
busybox-initramfs/jammy,now 1:1.30.1-7ubuntu3 amd64 [installed,automatic]
busybox-static/jammy,now 1:1.30.1-7ubuntu3 amd64 [installed,automatic]
bzip2/jammy,now 1.0.8-5build1 amd64 [installed,automatic]
ca-certificates/jammy-updates,jammy-updates,jammy-security,jammy-security,now 20230311ubuntu0.22.04.1 all [installed,automatic]
calamares-settings-lubuntu/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:22.04.4.3 all [installed]
calamares-settings-ubuntu-common/jammy-updates,jammy-security,now 1:22.04.4.3 amd64 [installed,automatic]
calamares/jammy-updates,now 3.2.61-0ubuntu0.1 amd64 [installed,automatic]
cheese-common/jammy,jammy,now 41.1-1build1 all [installed,automatic]
cheese/jammy,now 41.1-1build1 amd64 [installed,automatic]
colord-data/jammy,jammy,now 1.4.6-1 all [installed,automatic]
colord/jammy,now 1.4.6-1 amd64 [installed,automatic]
command-not-found/jammy,jammy,now 22.04.0 all [installed,automatic]
console-setup-linux/jammy,jammy,now 1.205ubuntu3 all [installed,automatic]
console-setup/jammy,jammy,now 1.205ubuntu3 all [installed,automatic]
coreutils/jammy,now 8.32-4.1ubuntu1 amd64 [installed,automatic]
cpio/jammy,now 2.13+dfsg-7 amd64 [installed,automatic]
cpp-11/jammy-updates,jammy-security,now 11.3.0-1ubuntu1~22.04.1 amd64 [installed,automatic]
cpp/jammy,now 4:11.2.0-1ubuntu1 amd64 [installed,automatic]
cracklib-runtime/jammy,now 2.9.6-3.4build4 amd64 [installed,automatic]
cron/jammy,now 3.0pl1-137ubuntu3 amd64 [installed,automatic]
cryptsetup-bin/jammy-updates,now 2:2.4.3-1ubuntu1.1 amd64 [installed,automatic]
cryptsetup-initramfs/jammy-updates,jammy-updates,now 2:2.4.3-1ubuntu1.1 all [installed,automatic]
cryptsetup/jammy-updates,now 2:2.4.3-1ubuntu1.1 amd64 [installed,automatic]
cups-browsed/jammy-updates,jammy-security,now 1.28.15-0ubuntu1.2 amd64 [installed,automatic]
cups-bsd/jammy-updates,jammy-security,now 2.4.1op1-1ubuntu4.4 amd64 [installed,automatic]
cups-client/jammy-updates,jammy-security,now 2.4.1op1-1ubuntu4.4 amd64 [installed,automatic]
cups-common/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2.4.1op1-1ubuntu4.4 all [installed,automatic]
cups-core-drivers/jammy-updates,jammy-security,now 2.4.1op1-1ubuntu4.4 amd64 [installed,automatic]
cups-daemon/jammy-updates,jammy-security,now 2.4.1op1-1ubuntu4.4 amd64 [installed,automatic]
cups-filters-core-drivers/jammy-updates,jammy-security,now 1.28.15-0ubuntu1.2 amd64 [installed,automatic]
cups-filters/jammy-updates,jammy-security,now 1.28.15-0ubuntu1.2 amd64 [installed,automatic]
cups-ipp-utils/jammy-updates,jammy-security,now 2.4.1op1-1ubuntu4.4 amd64 [installed,automatic]
cups-pk-helper/jammy,now 0.2.6-1ubuntu5 amd64 [installed,automatic]
cups-ppdc/jammy-updates,jammy-security,now 2.4.1op1-1ubuntu4.4 amd64 [installed,automatic]
cups-server-common/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2.4.1op1-1ubuntu4.4 all [installed,automatic]
cups/jammy-updates,jammy-security,now 2.4.1op1-1ubuntu4.4 amd64 [installed,automatic]
dash/jammy,now 0.5.11+git20210903+057cd650a4ed-3build1 amd64 [installed]
dbus-user-session/jammy-updates,jammy-security,now 1.12.20-2ubuntu4.1 amd64 [installed,automatic]
dbus/jammy-updates,jammy-security,now 1.12.20-2ubuntu4.1 amd64 [installed,automatic]
dc/jammy,now 1.07.1-3build1 amd64 [installed,automatic]
dconf-cli/jammy,now 0.40.0-3 amd64 [installed,automatic]
dconf-gsettings-backend/jammy,now 0.40.0-3 amd64 [installed,automatic]
dconf-service/jammy,now 0.40.0-3 amd64 [installed,automatic]
debconf-i18n/jammy,jammy,now 1.5.79ubuntu1 all [installed,automatic]
debconf/jammy,jammy,now 1.5.79ubuntu1 all [installed,automatic]
debianutils/jammy,now 5.5-1ubuntu2 amd64 [installed,automatic]
deja-dup/jammy-updates,now 42.9-1ubuntu3 amd64 [installed,automatic]
desktop-file-utils/jammy,now 0.26-1ubuntu3 amd64 [installed,automatic]
dictionaries-common/jammy,jammy,now 1.28.14 all [installed,automatic]
diffutils/jammy,now 1:3.8-0ubuntu2 amd64 [installed]
dirmngr/jammy-updates,jammy-security,now 2.2.27-3ubuntu2.1 amd64 [installed,automatic]
distro-info-data/jammy-updates,jammy-updates,now 0.52ubuntu0.4 all [installed,automatic]
distro-info/jammy,now 1.1build1 amd64 [installed,automatic]
dmidecode/jammy-updates,now 3.3-3ubuntu0.1 amd64 [installed,automatic]
dmsetup/jammy,now 2:1.02.175-2.1ubuntu4 amd64 [installed,automatic]
dmz-cursor-theme/jammy,jammy,now 0.4.5ubuntu1 all [installed,automatic]
dns-root-data/jammy,jammy,now 2021011101 all [installed,automatic]
dnsmasq-base/jammy-updates,jammy-security,now 2.86-1.1ubuntu0.3 amd64 [installed,automatic]
docbook-xml/jammy,jammy,now 4.5-11 all [installed,automatic]
dosfstools/jammy,now 4.2-1build3 amd64 [installed,automatic]
dpkg/jammy-updates,now 1.21.1ubuntu2.2 amd64 [installed,automatic]
duplicity/jammy,now 0.8.21-1build1 amd64 [installed,automatic]
e2fsprogs/jammy-updates,jammy-security,now 1.46.5-2ubuntu1.1 amd64 [installed,automatic]
ed/jammy,now 1.18-1 amd64 [installed,automatic]
efibootmgr/jammy,now 17-1ubuntu2 amd64 [installed]
eject/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
emacsen-common/jammy,jammy,now 3.0.4 all [installed,automatic]
enchant-2/jammy,now 2.3.2-1ubuntu2 amd64 [installed,automatic]
eog/jammy,now 42.0-1 amd64 [installed,automatic]
espeak-ng-data/jammy,now 1.50+dfsg-10 amd64 [installed,automatic]
ethtool/jammy,now 1:5.16-1 amd64 [installed,automatic]
evince-common/jammy-updates,jammy-updates,now 42.3-0ubuntu3 all [installed,automatic]
evince/jammy-updates,now 42.3-0ubuntu3 amd64 [installed,automatic]
evolution-data-server-common/jammy-updates,jammy-updates,now 3.44.4-0ubuntu1 all [installed,automatic]
evolution-data-server/jammy-updates,now 3.44.4-0ubuntu1 amd64 [installed,automatic]
fdisk/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
file-roller/jammy,now 3.42.0-1 amd64 [installed,automatic]
file/jammy,now 1:5.41-3 amd64 [installed,automatic]
findutils/jammy,now 4.8.0-1ubuntu3 amd64 [installed]
firmware-sof-signed/jammy-updates,jammy-updates,now 2.0-1ubuntu4.1 all [installed,automatic]
fontconfig-config/jammy,jammy,now 2.13.1-4.2ubuntu5 all [installed,automatic]
fontconfig/jammy,now 2.13.1-4.2ubuntu5 amd64 [installed,automatic]
fonts-beng-extra/jammy,jammy,now 3.2.1-1 all [installed,automatic]
fonts-beng/jammy,jammy,now 2:1.3 all [installed,automatic]
fonts-dejavu-core/jammy,jammy,now 2.37-2build1 all [installed,automatic]
fonts-deva-extra/jammy,jammy,now 3.0-5 all [installed,automatic]
fonts-deva/jammy,jammy,now 2:1.3 all [installed,automatic]
fonts-droid-fallback/jammy,jammy,now 1:6.0.1r16-1.1build1 all [installed,automatic]
fonts-freefont-ttf/jammy,jammy,now 20120503-10build1 all [installed,automatic]
fonts-gargi/jammy,jammy,now 2.0-5 all [installed,automatic]
fonts-gubbi/jammy,jammy,now 1.3-5build1 all [installed,automatic]
fonts-gujr-extra/jammy,jammy,now 1.0.1-1 all [installed,automatic]
fonts-gujr/jammy,jammy,now 2:1.4 all [installed,automatic]
fonts-guru-extra/jammy,jammy,now 2.0-5 all [installed,automatic]
fonts-guru/jammy,jammy,now 2:1.3 all [installed,automatic]
fonts-indic/jammy,jammy,now 2:1.4 all [installed]
fonts-kacst-one/jammy,jammy,now 5.0+svn11846-10 all [installed,automatic]
fonts-kacst/jammy,jammy,now 2.01+mry-15 all [installed,automatic]
fonts-kalapi/jammy,jammy,now 1.0-4 all [installed,automatic]
fonts-khmeros-core/jammy,jammy,now 5.0-9ubuntu1 all [installed,automatic]
fonts-knda/jammy,jammy,now 2:1.3 all [installed,automatic]
fonts-lao/jammy,jammy,now 0.0.20060226-10ubuntu2 all [installed,automatic]
fonts-liberation2/jammy,jammy,now 2.1.5-1 all [installed,automatic]
fonts-liberation/jammy,jammy,now 1:1.07.4-11 all [installed,automatic]
fonts-lklug-sinhala/jammy,jammy,now 0.6-4 all [installed,automatic]
fonts-lohit-beng-assamese/jammy,jammy,now 2.91.5-2 all [installed,automatic]
fonts-lohit-beng-bengali/jammy,jammy,now 2.91.5-2 all [installed,automatic]
fonts-lohit-deva/jammy,jammy,now 2.95.4-4 all [installed,automatic]
fonts-lohit-gujr/jammy,jammy,now 2.92.4-4 all [installed,automatic]
fonts-lohit-guru/jammy,jammy,now 2.91.2-2build1 all [installed,automatic]
fonts-lohit-knda/jammy,jammy,now 2.5.4-3 all [installed,automatic]
fonts-lohit-mlym/jammy,jammy,now 2.92.2-2 all [installed,automatic]
fonts-lohit-orya/jammy,jammy,now 2.91.2-2 all [installed,automatic]
fonts-lohit-taml-classical/jammy,jammy,now 2.5.4-2 all [installed,automatic]
fonts-lohit-taml/jammy,jammy,now 2.91.3-2 all [installed,automatic]
fonts-lohit-telu/jammy,jammy,now 2.5.5-2build1 all [installed,automatic]
fonts-mlym/jammy,jammy,now 2:1.3 all [installed,automatic]
fonts-nakula/jammy,jammy,now 1.0-4 all [installed,automatic]
fonts-navilu/jammy,jammy,now 1.2-3 all [installed,automatic]
fonts-noto-cjk/jammy,jammy,now 1:20220127+repack1-1 all [installed,automatic]
fonts-noto-color-emoji/jammy-updates,jammy-updates,now 2.038-0ubuntu1 all [installed,automatic]
fonts-noto-mono/jammy,jammy,now 20201225-1build1 all [installed,automatic]
fonts-opensymbol/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2:102.12+LibO7.3.7-0ubuntu0.22.04.3 all [installed,automatic]
fonts-orya-extra/jammy,jammy,now 2.0-6 all [installed,automatic]
fonts-orya/jammy,jammy,now 2:1.3 all [installed,automatic]
fonts-pagul/jammy,jammy,now 1.0-8 all [installed,automatic]
fonts-sahadeva/jammy,jammy,now 1.0-5 all [installed,automatic]
fonts-samyak-deva/jammy,jammy,now 1.2.2-5build1 all [installed,automatic]
fonts-samyak-gujr/jammy,jammy,now 1.2.2-5build1 all [installed,automatic]
fonts-samyak-mlym/jammy,jammy,now 1.2.2-5build1 all [installed,automatic]
fonts-samyak-taml/jammy,jammy,now 1.2.2-5build1 all [installed,automatic]
fonts-sarai/jammy,jammy,now 1.0-3 all [installed,automatic]
fonts-sil-abyssinica/jammy,jammy,now 2.100-3 all [installed,automatic]
fonts-sil-padauk/jammy,jammy,now 5.000-3 all [installed,automatic]
fonts-smc-anjalioldlipi/jammy,jammy,now 7.1.2-2 all [installed,automatic]
fonts-smc-chilanka/jammy,jammy,now 1.540-1 all [installed,automatic]
fonts-smc-dyuthi/jammy,jammy,now 3.0.2-2 all [installed,automatic]
fonts-smc-gayathri/jammy,jammy,now 1.110-2-1 all [installed,automatic]
fonts-smc-karumbi/jammy,jammy,now 1.1.2-2 all [installed,automatic]
fonts-smc-keraleeyam/jammy,jammy,now 3.0.2-2 all [installed,automatic]
fonts-smc-manjari/jammy,jammy,now 2.000-3 all [installed,automatic]
fonts-smc-meera/jammy,jammy,now 7.0.3-1 all [installed,automatic]
fonts-smc-rachana/jammy,jammy,now 7.0.2-1build1 all [installed,automatic]
fonts-smc-raghumalayalamsans/jammy,jammy,now 2.2.1-1 all [installed,automatic]
fonts-smc-suruma/jammy,jammy,now 3.2.3-1 all [installed,automatic]
fonts-smc-uroob/jammy,jammy,now 2.0.2-1 all [installed,automatic]
fonts-smc/jammy,jammy,now 1:7.2 all [installed,automatic]
fonts-taml/jammy,jammy,now 2:1.4 all [installed,automatic]
fonts-telu-extra/jammy,jammy,now 2.0-5 all [installed,automatic]
fonts-telu/jammy,jammy,now 2:1.3 all [installed,automatic]
fonts-teluguvijayam/jammy,jammy,now 2.1-1 all [installed,automatic]
fonts-thai-tlwg/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tibetan-machine/jammy,jammy,now 1.901b-6 all [installed,automatic]
fonts-tlwg-garuda-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-garuda/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-kinnari-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-kinnari/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-laksaman-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-laksaman/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-loma-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-loma/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-mono-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-mono/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-norasi-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-norasi/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-purisa-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-purisa/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-sawasdee-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-sawasdee/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-typewriter-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-typewriter/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-typist-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-typist/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-typo-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-typo/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-umpush-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-umpush/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-waree-ttf/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-tlwg-waree/jammy,jammy,now 1:0.7.3-1 all [installed,automatic]
fonts-ubuntu/jammy,jammy,now 0.83-6ubuntu1 all [installed,automatic]
fonts-urw-base35/jammy,jammy,now 20200910-1 all [installed,automatic]
fonts-yrsa-rasa/jammy,jammy,now 2.005-1 all [installed,automatic]
foomatic-db-compressed-ppds/jammy,jammy,now 20220223-0ubuntu1 all [installed,automatic]
fprintd/jammy-updates,now 1.94.2-1ubuntu0.22.04.1 amd64 [installed,automatic]
friendly-recovery/jammy,jammy,now 0.2.42 all [installed,automatic]
ftp/jammy,jammy,now 20210827-4build1 all [installed,automatic]
fuse3/jammy,now 3.10.5-1build1 amd64 [installed,automatic]
fwupd-signed/jammy-updates,now 1.51.1~22.04.1+1.4-0ubuntu0.1 amd64 [installed,automatic]
fwupd/jammy-updates,now 1.7.9-1~22.04.3 amd64 [installed,automatic]
gamemode-daemon/jammy,now 1.6.1-1build2 amd64 [installed,automatic]
gamemode/jammy,now 1.6.1-1build2 amd64 [installed,automatic]
gamin/jammy,now 0.1.10-6 amd64 [installed,automatic]
gcc-11-base/jammy-updates,jammy-security,now 11.3.0-1ubuntu1~22.04.1 amd64 [installed,automatic]
gcc-12-base/jammy-updates,jammy-security,now 12.1.0-2ubuntu1~22.04 amd64 [installed,automatic]
gcr/jammy,now 3.40.0-4 amd64 [installed,automatic]
gdb/jammy-updates,now 12.1-0ubuntu1~22.04 amd64 [installed,automatic]
gdisk/jammy,now 1.0.8-4build1 amd64 [installed,automatic]
gdm3/jammy-updates,now 42.0-1ubuntu7.22.04.3 amd64 [installed,automatic]
gedit-common/jammy,jammy,now 41.0-3 all [installed,automatic]
gedit/jammy,now 41.0-3 amd64 [installed,automatic]
genisoimage/jammy,now 9:1.1.11-3.2ubuntu1 amd64 [installed,automatic]
geoclue-2.0/jammy,now 2.5.7-3ubuntu3 amd64 [installed,automatic]
gettext-base/jammy,now 0.21-4ubuntu4 amd64 [installed,automatic]
ghostscript-x/jammy-updates,jammy-security,now 9.55.0~dfsg1-0ubuntu5.3 amd64 [installed,automatic]
ghostscript/jammy-updates,jammy-security,now 9.55.0~dfsg1-0ubuntu5.3 amd64 [installed,automatic]
gir1.2-accountsservice-1.0/jammy-updates,jammy-security,now 22.07.5-2ubuntu1.4 amd64 [installed,automatic]
gir1.2-adw-1/jammy,now 1.1.0-1ubuntu2 amd64 [installed,upgradable to: 1.1.7-0ubuntu0.22.04.1]
gir1.2-atk-1.0/jammy,now 2.36.0-3build1 amd64 [installed,automatic]
gir1.2-atspi-2.0/jammy,now 2.44.0-3 amd64 [installed,automatic]
gir1.2-dbusmenu-glib-0.4/jammy,now 16.04.1+18.10.20180917-0ubuntu8 amd64 [installed,automatic]
gir1.2-dee-1.0/jammy,now 1.2.7+17.10.20170616-6ubuntu4 amd64 [installed,automatic]
gir1.2-freedesktop/jammy,now 1.72.0-1 amd64 [installed,automatic]
gir1.2-gck-1/jammy,now 3.40.0-4 amd64 [installed,automatic]
gir1.2-gcr-3/jammy,now 3.40.0-4 amd64 [installed,automatic]
gir1.2-gdesktopenums-3.0/jammy,now 42.0-1ubuntu1 amd64 [installed,automatic]
gir1.2-gdkpixbuf-2.0/jammy-updates,now 2.42.8+dfsg-1ubuntu0.2 amd64 [installed,automatic]
gir1.2-gdm-1.0/jammy-updates,now 42.0-1ubuntu7.22.04.3 amd64 [installed,automatic]
gir1.2-geoclue-2.0/jammy,now 2.5.7-3ubuntu3 amd64 [installed,automatic]
gir1.2-glib-2.0/jammy,now 1.72.0-1 amd64 [installed,automatic]
gir1.2-gmenu-3.0/jammy,now 3.36.0-1ubuntu3 amd64 [installed,automatic]
gir1.2-gnomebluetooth-3.0/jammy,now 42.0-5 amd64 [installed,automatic]
gir1.2-gnomedesktop-3.0/now 42.5-0ubuntu1 amd64 [installed,upgradable to: 42.9-0ubuntu1]
gir1.2-goa-1.0/jammy,now 3.44.0-1ubuntu1 amd64 [installed,automatic]
gir1.2-graphene-1.0/jammy,now 1.10.8-1 amd64 [installed,automatic]
gir1.2-gst-plugins-base-1.0/jammy,now 1.20.1-1 amd64 [installed,automatic]
gir1.2-gstreamer-1.0/jammy-updates,now 1.20.3-0ubuntu1 amd64 [installed,automatic]
gir1.2-gtk-3.0/jammy-updates,now 3.24.33-1ubuntu2 amd64 [installed,automatic]
gir1.2-gtk-4.0/jammy-updates,now 4.6.6+ds-0ubuntu1 amd64 [installed,automatic]
gir1.2-gtksource-4/jammy,now 4.8.3-1 amd64 [installed,automatic]
gir1.2-gudev-1.0/jammy,now 1:237-2build1 amd64 [installed,automatic]
gir1.2-gweather-3.0/jammy,now 40.0-5build1 amd64 [installed,automatic]
gir1.2-handy-1/jammy,now 1.6.1-1 amd64 [installed,automatic]
gir1.2-harfbuzz-0.0/jammy-updates,jammy-security,now 2.7.4-1ubuntu3.1 amd64 [installed,automatic]
gir1.2-ibus-1.0/jammy,now 1.5.26-4 amd64 [installed,automatic]
gir1.2-javascriptcoregtk-4.0/jammy-updates,jammy-security,now 2.38.6-0ubuntu0.22.04.1 amd64 [installed,automatic]
gir1.2-json-1.0/jammy,now 1.6.6-1build1 amd64 [installed,automatic]
gir1.2-mutter-10/now 42.5-0ubuntu1 amd64 [installed,upgradable to: 42.9-0ubuntu1]
gir1.2-nm-1.0/jammy-updates,now 1.36.6-0ubuntu2 amd64 [installed,automatic]
gir1.2-nma-1.0/jammy,now 1.8.34-1ubuntu1 amd64 [installed,automatic]
gir1.2-notify-0.7/jammy-updates,now 0.7.9-3ubuntu5.22.04.1 amd64 [installed,automatic]
gir1.2-packagekitglib-1.0/jammy,now 1.2.5-2ubuntu2 amd64 [installed,automatic]
gir1.2-pango-1.0/jammy-updates,now 1.50.6+ds-2ubuntu1 amd64 [installed,automatic]
gir1.2-peas-1.0/jammy,now 1.32.0-1 amd64 [installed,automatic]
gir1.2-polkit-1.0/jammy,now 0.105-33 amd64 [installed,automatic]
gir1.2-rb-3.0/jammy,now 3.4.4-5ubuntu1 amd64 [installed,automatic]
gir1.2-rsvg-2.0/jammy,now 2.52.5+dfsg-3 amd64 [installed,automatic]
gir1.2-secret-1/jammy,now 0.20.5-2 amd64 [installed,automatic]
gir1.2-snapd-1/jammy,now 1.60-0ubuntu1 amd64 [installed,automatic]
gir1.2-soup-2.4/jammy,now 2.74.2-3 amd64 [installed,automatic]
gir1.2-totem-1.0/jammy,now 42.0-1ubuntu1 amd64 [installed,automatic]
gir1.2-totemplparser-1.0/jammy,now 3.26.6-1build1 amd64 [installed,automatic]
gir1.2-udisks-2.0/jammy,now 2.9.4-1ubuntu2 amd64 [installed,automatic]
gir1.2-unity-7.0/jammy,now 7.1.4+19.04.20190319-6build1 amd64 [installed,automatic]
gir1.2-upowerglib-1.0/jammy,now 0.99.17-1 amd64 [installed,automatic]
gir1.2-vte-2.91/jammy,now 0.68.0-1 amd64 [installed,automatic]
gir1.2-webkit2-4.0/jammy-updates,jammy-security,now 2.38.6-0ubuntu0.22.04.1 amd64 [installed,automatic]
gir1.2-wnck-3.0/jammy,now 40.1-1 amd64 [installed,automatic]
gjs/now 1.72.2-0ubuntu2 amd64 [installed,upgradable to: 1.72.4-0ubuntu0.22.04.1]
gkbd-capplet/jammy,now 3.26.1-2 amd64 [installed,automatic]
glib-networking-common/jammy,jammy,now 2.72.0-1 all [installed,automatic]
glib-networking-services/jammy,now 2.72.0-1 amd64 [installed,automatic]
glib-networking/jammy,now 2.72.0-1 amd64 [installed,automatic]
gnome-accessibility-themes/jammy,jammy,now 3.28-1ubuntu3 all [installed,automatic]
gnome-bluetooth-3-common/jammy,jammy,now 42.0-5 all [installed,automatic]
gnome-bluetooth-common/jammy,jammy,now 3.34.5-8 all [installed,automatic]
gnome-bluetooth/jammy,now 3.34.5-8 amd64 [installed,automatic]
gnome-calculator/jammy,now 1:41.1-2ubuntu2 amd64 [installed,automatic]
gnome-calendar/jammy,now 41.2-3 amd64 [installed,automatic]
gnome-characters/jammy,now 41.0-4 amd64 [installed,automatic]
gnome-control-center-data/jammy-updates,jammy-updates,now 1:41.7-0ubuntu0.22.04.6 all [installed,automatic]
gnome-control-center-faces/jammy-updates,jammy-updates,now 1:41.7-0ubuntu0.22.04.6 all [installed,automatic]
gnome-control-center/jammy-updates,now 1:41.7-0ubuntu0.22.04.6 amd64 [installed,automatic]
gnome-desktop3-data/now 42.5-0ubuntu1 all [installed,upgradable to: 42.9-0ubuntu1]
gnome-disk-utility/jammy,now 42.0-1ubuntu1 amd64 [installed,automatic]
gnome-font-viewer/jammy,now 41.0-2 amd64 [installed,automatic]
gnome-initial-setup/jammy-updates,now 42.0.1-1ubuntu2.3 amd64 [installed,automatic]
gnome-keyring-pkcs11/jammy-updates,now 40.0-3ubuntu3 amd64 [installed,automatic]
gnome-keyring/jammy-updates,now 40.0-3ubuntu3 amd64 [installed,automatic]
gnome-logs/jammy,now 42.0-1 amd64 [installed,automatic]
gnome-mahjongg/jammy,now 1:3.38.3-2 amd64 [installed,automatic]
gnome-menus/jammy,now 3.36.0-1ubuntu3 amd64 [installed,automatic]
gnome-mines/jammy,now 1:40.1-1 amd64 [installed,automatic]
gnome-online-accounts/jammy,now 3.44.0-1ubuntu1 amd64 [installed,automatic]
gnome-power-manager/jammy,now 3.32.0-2build2 amd64 [installed,automatic]
gnome-remote-desktop/jammy-updates,now 42.7-0ubuntu1 amd64 [installed,automatic]
gnome-session-bin/jammy,now 42.0-1ubuntu2 amd64 [installed,automatic]
gnome-session-canberra/jammy-updates,now 0.30-10ubuntu1.22.04.1 amd64 [installed,automatic]
gnome-session-common/jammy,jammy,now 42.0-1ubuntu2 all [installed,automatic]
gnome-settings-daemon-common/jammy-updates,jammy-updates,now 42.1-1ubuntu2.2 all [installed,automatic]
gnome-settings-daemon/jammy-updates,now 42.1-1ubuntu2.2 amd64 [installed,automatic]
gnome-shell-common/now 42.5-0ubuntu1 all [installed,upgradable to: 42.9-0ubuntu2]
gnome-shell-extension-appindicator/jammy,jammy,now 42-2~fakesync1 all [installed,automatic]
gnome-shell-extension-desktop-icons-ng/jammy-updates,jammy-updates,now 43-2ubuntu1 all [installed,automatic]
gnome-shell-extension-ubuntu-dock/jammy-updates,jammy-updates,now 72~ubuntu5.22.04.2.1 all [installed,automatic]
gnome-shell/now 42.5-0ubuntu1 amd64 [installed,upgradable to: 42.9-0ubuntu2]
gnome-startup-applications/jammy,now 42.0-1ubuntu2 amd64 [installed,automatic]
gnome-sudoku/jammy,now 1:42.0-1 amd64 [installed,automatic]
gnome-system-monitor/jammy,now 42.0-1 amd64 [installed,automatic]
gnome-terminal-data/jammy,jammy,now 3.44.0-1ubuntu1 all [installed,automatic]
gnome-terminal/jammy,now 3.44.0-1ubuntu1 amd64 [installed,automatic]
gnome-themes-extra-data/jammy,jammy,now 3.28-1ubuntu3 all [installed,automatic]
gnome-themes-extra/jammy,now 3.28-1ubuntu3 amd64 [installed,automatic]
gnome-todo-common/jammy,jammy,now 3.28.1-6ubuntu1 all [installed,automatic]
gnome-todo/jammy,now 3.28.1-6ubuntu1 amd64 [installed,automatic]
gnome-user-docs/jammy,jammy,now 41.5-1ubuntu2 all [installed,automatic]
gnome-video-effects/jammy,jammy,now 0.5.0-1ubuntu1 all [installed,automatic]
gnupg-l10n/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2.2.27-3ubuntu2.1 all [installed,automatic]
gnupg-utils/jammy-updates,jammy-security,now 2.2.27-3ubuntu2.1 amd64 [installed,automatic]
gnupg/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2.2.27-3ubuntu2.1 all [installed,automatic]
gpg-agent/jammy-updates,jammy-security,now 2.2.27-3ubuntu2.1 amd64 [installed,automatic]
gpg-wks-client/jammy-updates,jammy-security,now 2.2.27-3ubuntu2.1 amd64 [installed,automatic]
gpg-wks-server/jammy-updates,jammy-security,now 2.2.27-3ubuntu2.1 amd64 [installed,automatic]
gpg/jammy-updates,jammy-security,now 2.2.27-3ubuntu2.1 amd64 [installed,automatic]
gpgconf/jammy-updates,jammy-security,now 2.2.27-3ubuntu2.1 amd64 [installed,automatic]
gpgsm/jammy-updates,jammy-security,now 2.2.27-3ubuntu2.1 amd64 [installed,automatic]
gpgv/jammy-updates,jammy-security,now 2.2.27-3ubuntu2.1 amd64 [installed,automatic]
grep/jammy,now 3.7-1build1 amd64 [installed]
grilo-plugins-0.3-base/jammy,now 0.3.14-1ubuntu2 amd64 [installed,automatic]
groff-base/jammy,now 1.22.4-8build1 amd64 [installed,automatic]
grub-common/jammy-updates,now 2.06-2ubuntu7.2 amd64 [installed]
grub-efi-amd64-bin/jammy-updates,now 2.06-2ubuntu14.1 amd64 [installed]
grub-efi-amd64-signed/jammy-updates,now 1.187.3~22.04.1+2.06-2ubuntu14.1 amd64 [installed]
grub-gfxpayload-lists/jammy,now 0.7 amd64 [installed]
grub-pc-bin/jammy-updates,now 2.06-2ubuntu7.2 amd64 [installed]
grub-pc/jammy-updates,now 2.06-2ubuntu7.2 amd64 [installed]
grub2-common/jammy-updates,now 2.06-2ubuntu7.2 amd64 [installed]
gsettings-desktop-schemas/jammy,jammy,now 42.0-1ubuntu1 all [installed,automatic]
gsettings-ubuntu-schemas/jammy,jammy,now 0.0.7+21.10.20210712-0ubuntu2 all [installed,automatic]
gstreamer1.0-alsa/jammy,now 1.20.1-1 amd64 [installed,automatic]
gstreamer1.0-clutter-3.0/jammy-updates,now 3.0.27-2ubuntu1 amd64 [installed,automatic]
gstreamer1.0-gl/jammy,now 1.20.1-1 amd64 [installed,automatic]
gstreamer1.0-gtk3/jammy-updates,now 1.20.3-0ubuntu1 amd64 [installed,automatic]
gstreamer1.0-packagekit/jammy,now 1.2.5-2ubuntu2 amd64 [installed,automatic]
gstreamer1.0-pipewire/jammy-updates,now 0.3.48-1ubuntu3 amd64 [installed,automatic]
gstreamer1.0-plugins-base-apps/jammy,now 1.20.1-1 amd64 [installed,automatic]
gstreamer1.0-plugins-base/jammy,now 1.20.1-1 amd64 [installed,automatic]
gstreamer1.0-plugins-good/jammy-updates,now 1.20.3-0ubuntu1 amd64 [installed,automatic]
gstreamer1.0-pulseaudio/jammy-updates,now 1.20.3-0ubuntu1 amd64 [installed,automatic]
gstreamer1.0-tools/jammy-updates,now 1.20.3-0ubuntu1 amd64 [installed,automatic]
gstreamer1.0-x/jammy,now 1.20.1-1 amd64 [installed,automatic]
gtk-update-icon-cache/jammy-updates,now 3.24.33-1ubuntu2 amd64 [installed,automatic]
gtk2-engines-murrine/jammy,now 0.98.2-3build2 amd64 [installed,automatic]
gtk2-engines-pixbuf/jammy,now 2.24.33-2ubuntu2 amd64 [installed,automatic]
guile-2.2-libs/jammy,now 2.2.7+1-6build2 amd64 [installed,automatic]
gvfs-backends/jammy-updates,now 1.48.2-0ubuntu1 amd64 [installed,automatic]
gvfs-common/jammy-updates,jammy-updates,now 1.48.2-0ubuntu1 all [installed,automatic]
gvfs-daemons/jammy-updates,now 1.48.2-0ubuntu1 amd64 [installed,automatic]
gvfs-fuse/jammy-updates,now 1.48.2-0ubuntu1 amd64 [installed,automatic]
gvfs-libs/jammy-updates,now 1.48.2-0ubuntu1 amd64 [installed,automatic]
gvfs/jammy-updates,now 1.48.2-0ubuntu1 amd64 [installed,automatic]
gzip/jammy-updates,now 1.10-4ubuntu4.1 amd64 [installed]
hdparm/jammy,now 9.60+ds-1build3 amd64 [installed,automatic]
hicolor-icon-theme/jammy,jammy,now 0.17-2 all [installed,automatic]
hostname/jammy,now 3.23ubuntu2 amd64 [installed]
hplip-data/jammy,jammy,now 3.21.12+dfsg0-1 all [installed,automatic]
hplip/jammy,now 3.21.12+dfsg0-1 amd64 [installed,automatic]
humanity-icon-theme/jammy,jammy,now 0.6.16 all [installed,automatic]
hunspell-en-us/jammy,jammy,now 1:2020.12.07-2 all [installed,automatic]
hyphen-en-us/jammy,jammy,now 2.8.8-7build2 all [installed]
ibus-data/jammy,jammy,now 1.5.26-4 all [installed,automatic]
ibus-gtk3/jammy,now 1.5.26-4 amd64 [installed,automatic]
ibus-gtk4/jammy,now 1.5.26-4 amd64 [installed,automatic]
ibus-gtk/jammy,now 1.5.26-4 amd64 [installed,automatic]
ibus-table/jammy,jammy,now 1.16.7-1 all [installed,automatic]
ibus/jammy,now 1.5.26-4 amd64 [installed,automatic]
iio-sensor-proxy/jammy,now 3.3-0ubuntu6 amd64 [installed,automatic]
im-config/jammy-updates,jammy-updates,now 0.50-2ubuntu22.04.1 all [installed,automatic]
info/jammy,now 6.8-4build1 amd64 [installed,automatic]
init-system-helpers/jammy,jammy,now 1.62 all [installed,automatic]
init/jammy,now 1.62 amd64 [installed]
initramfs-tools-bin/now 0.140ubuntu13.1 amd64 [installed,upgradable to: 0.140ubuntu13.2]
initramfs-tools-core/now 0.140ubuntu13.1 all [installed,upgradable to: 0.140ubuntu13.2]
initramfs-tools/now 0.140ubuntu13.1 all [installed,upgradable to: 0.140ubuntu13.2]
inputattach/jammy,now 1:1.7.1-1build2 amd64 [installed,automatic]
install-info/jammy,now 6.8-4build1 amd64 [installed,automatic]
intel-microcode/jammy-updates,jammy-security,now 3.20230214.0ubuntu0.22.04.1 amd64 [installed,automatic]
ipp-usb/jammy-updates,jammy-security,now 0.9.20-1ubuntu0.22.04.1 amd64 [installed,automatic]
iproute2/jammy,now 5.15.0-1ubuntu2 amd64 [installed,automatic]
iptables/jammy-updates,now 1.8.7-1ubuntu5.1 amd64 [installed,automatic]
iputils-ping/jammy,now 3:20211215-1 amd64 [installed,automatic]
iputils-tracepath/jammy,now 3:20211215-1 amd64 [installed,automatic]
irqbalance/jammy,now 1.8.0-1build1 amd64 [installed,automatic]
isc-dhcp-client/jammy-updates,now 4.4.1-2.3ubuntu2.4 amd64 [installed,automatic]
isc-dhcp-common/jammy-updates,now 4.4.1-2.3ubuntu2.4 amd64 [installed,automatic]
iso-codes/jammy,jammy,now 4.9.0-1 all [installed,automatic]
iucode-tool/jammy,now 2.3.1-1build1 amd64 [installed,automatic]
kbd/jammy-updates,now 2.3.0-3ubuntu4.22.04 amd64 [installed,automatic]
kded5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
kerneloops/jammy,now 0.12+git20140509-6ubuntu5 amd64 [installed,automatic]
keyboard-configuration/jammy,jammy,now 1.205ubuntu3 all [installed,automatic]
keyutils/jammy,now 1.6.1-2ubuntu3 amd64 [installed,automatic]
kio/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
klibc-utils/jammy,now 2.0.10-4 amd64 [installed,automatic]
kmod/jammy,now 29-1ubuntu1 amd64 [installed,automatic]
kwayland-data/jammy,jammy,now 4:5.92.0-0ubuntu1 all [installed,automatic]
kwayland-integration/jammy,now 4:5.24.4-0ubuntu1 amd64 [installed,automatic]
language-pack-en-base/jammy-updates,jammy-updates,now 1:22.04+20230209 all [installed]
language-pack-en/jammy-updates,jammy-updates,now 1:22.04+20230209 all [installed]
language-pack-gnome-en-base/jammy-updates,jammy-updates,now 1:22.04+20230209 all [installed]
language-pack-gnome-en/jammy-updates,jammy-updates,now 1:22.04+20230209 all [installed]
language-selector-common/jammy-updates,jammy-updates,now 0.219.1 all [installed,automatic]
language-selector-gnome/jammy-updates,jammy-updates,now 0.219.1 all [installed,automatic]
laptop-detect/jammy,jammy,now 0.16 all [installed,automatic]
less/jammy-updates,jammy-security,now 590-1ubuntu0.22.04.1 amd64 [installed,automatic]
libaa1/jammy,now 1.4p5-50build1 amd64 [installed,automatic]
libabsl20210324/jammy,now 0~20210324.2-2 amd64 [installed,automatic]
libabw-0.1-1/jammy,now 0.1.3-1build3 amd64 [installed,automatic]
libaccountsservice0/jammy-updates,jammy-security,now 22.07.5-2ubuntu1.4 amd64 [installed,automatic]
libacl1/jammy,now 2.3.1-1 amd64 [installed,automatic]
libadwaita-1-0/jammy,now 1.1.0-1ubuntu2 amd64 [installed,upgradable to: 1.1.7-0ubuntu0.22.04.1]
libao-common/jammy,jammy,now 1.2.2+20180113-1.1ubuntu3 all [installed,automatic]
libao4/jammy,now 1.2.2+20180113-1.1ubuntu3 amd64 [installed,automatic]
libapparmor1/jammy-updates,now 3.0.4-2ubuntu2.2 amd64 [installed,automatic]
libappstream4/jammy,now 0.15.2-2 amd64 [installed,automatic]
libapt-pkg6.0/jammy-updates,now 2.4.9 amd64 [installed,automatic]
libarchive13/jammy,now 3.6.0-1ubuntu1 amd64 [installed,automatic]
libargon2-1/jammy,now 0~20171227-0.3 amd64 [installed,automatic]
libasound2-data/jammy,jammy,now 1.2.6.1-1ubuntu1 all [installed,automatic]
libasound2-plugins/jammy,now 1.2.6-1 amd64 [installed,automatic]
libasound2/jammy,now 1.2.6.1-1ubuntu1 amd64 [installed,automatic]
libaspell15/jammy,now 0.60.8-4build1 amd64 [installed,automatic]
libassuan0/jammy,now 2.5.5-1build1 amd64 [installed,automatic]
libasyncns0/jammy,now 0.8-6build2 amd64 [installed,automatic]
libatasmart4/jammy,now 0.19-5build2 amd64 [installed,automatic]
libatk-adaptor/jammy,now 2.38.0-3 amd64 [installed,automatic]
libatk-bridge2.0-0/jammy,now 2.38.0-3 amd64 [installed,automatic]
libatk1.0-0/jammy,now 2.36.0-3build1 amd64 [installed,automatic]
libatk1.0-data/jammy,jammy,now 2.36.0-3build1 all [installed,automatic]
libatkmm-1.6-1v5/jammy,now 2.28.2-1build1 amd64 [installed,automatic]
libatm1/jammy,now 1:2.5.1-4build2 amd64 [installed,automatic]
libatomic1/jammy-updates,jammy-security,now 12.1.0-2ubuntu1~22.04 amd64 [installed,automatic]
libatopology2/jammy,now 1.2.6.1-1ubuntu1 amd64 [installed,automatic]
libatspi2.0-0/jammy,now 2.44.0-3 amd64 [installed,automatic]
libattr1/jammy,now 1:2.5.1-1build1 amd64 [installed,automatic]
libaudit-common/jammy,jammy,now 1:3.0.7-1build1 all [installed,automatic]
libaudit1/jammy,now 1:3.0.7-1build1 amd64 [installed,automatic]
libauthen-sasl-perl/jammy,jammy,now 2.1600-1.1 all [installed,automatic]
libavahi-client3/jammy-updates,jammy-security,now 0.8-5ubuntu5.1 amd64 [installed,automatic]
libavahi-common-data/jammy-updates,jammy-security,now 0.8-5ubuntu5.1 amd64 [installed,automatic]
libavahi-common3/jammy-updates,jammy-security,now 0.8-5ubuntu5.1 amd64 [installed,automatic]
libavahi-core7/jammy-updates,jammy-security,now 0.8-5ubuntu5.1 amd64 [installed,automatic]
libavahi-glib1/jammy-updates,jammy-security,now 0.8-5ubuntu5.1 amd64 [installed,automatic]
libavahi-ui-gtk3-0/jammy-updates,jammy-security,now 0.8-5ubuntu5.1 amd64 [installed,automatic]
libavc1394-0/jammy,now 0.5.4-5build2 amd64 [installed,automatic]
libayatana-appindicator3-1/jammy,now 0.5.90-7ubuntu2 amd64 [installed,automatic]
libayatana-ido3-0.4-0/jammy,now 0.9.1-1 amd64 [installed,automatic]
libayatana-indicator3-7/jammy,now 0.9.1-1 amd64 [installed,automatic]
libbabeltrace1/jammy,now 1.5.8-2build1 amd64 [installed,automatic]
libblkid1/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
libblockdev-crypto2/jammy,now 2.26-1 amd64 [installed,automatic]
libblockdev-fs2/jammy,now 2.26-1 amd64 [installed,automatic]
libblockdev-loop2/jammy,now 2.26-1 amd64 [installed,automatic]
libblockdev-part-err2/jammy,now 2.26-1 amd64 [installed,automatic]
libblockdev-part2/jammy,now 2.26-1 amd64 [installed,automatic]
libblockdev-swap2/jammy,now 2.26-1 amd64 [installed,automatic]
libblockdev-utils2/jammy,now 2.26-1 amd64 [installed,automatic]
libblockdev2/jammy,now 2.26-1 amd64 [installed,automatic]
libbluetooth3/jammy,now 5.64-0ubuntu1 amd64 [installed,automatic]
libboost-filesystem1.74.0/jammy,now 1.74.0-14ubuntu3 amd64 [installed,automatic]
libboost-iostreams1.74.0/jammy,now 1.74.0-14ubuntu3 amd64 [installed,automatic]
libboost-locale1.74.0/jammy,now 1.74.0-14ubuntu3 amd64 [installed,automatic]
libboost-python1.74.0/jammy,now 1.74.0-14ubuntu3 amd64 [installed,automatic]
libboost-regex1.74.0/jammy,now 1.74.0-14ubuntu3 amd64 [installed,automatic]
libboost-thread1.74.0/jammy,now 1.74.0-14ubuntu3 amd64 [installed,automatic]
libbpf0/jammy-updates,jammy-security,now 1:0.5.0-1ubuntu22.04.1 amd64 [installed,automatic]
libbrlapi0.8/jammy-updates,now 6.4-4ubuntu3 amd64 [installed,automatic]
libbrotli1/jammy,now 1.0.9-2build6 amd64 [installed,automatic]
libbsd0/jammy,now 0.11.5-1 amd64 [installed,automatic]
libbz2-1.0/jammy,now 1.0.8-5build1 amd64 [installed,automatic]
libc-bin/jammy-updates,now 2.35-0ubuntu3.1 amd64 [installed,automatic]
libc6-dbg/jammy-updates,now 2.35-0ubuntu3.1 amd64 [installed,automatic]
libc6/jammy-updates,now 2.35-0ubuntu3.1 amd64 [installed,automatic]
libcaca0/jammy,now 0.99.beta19-2.2ubuntu4 amd64 [installed,automatic]
libcairo-gobject-perl/jammy,now 1.005-3build1 amd64 [installed,automatic]
libcairo-gobject2/jammy,now 1.16.0-5ubuntu2 amd64 [installed,automatic]
libcairo-perl/jammy,now 1.109-2build1 amd64 [installed,automatic]
libcairo-script-interpreter2/jammy,now 1.16.0-5ubuntu2 amd64 [installed,automatic]
libcairo2/jammy,now 1.16.0-5ubuntu2 amd64 [installed,automatic]
libcairomm-1.0-1v5/jammy,now 1.12.2-4build3 amd64 [installed,automatic]
libcamel-1.2-63/jammy-updates,now 3.44.4-0ubuntu1 amd64 [installed,automatic]
libcanberra-gtk3-0/jammy-updates,now 0.30-10ubuntu1.22.04.1 amd64 [installed,automatic]
libcanberra-gtk3-module/jammy-updates,now 0.30-10ubuntu1.22.04.1 amd64 [installed,automatic]
libcanberra-pulse/jammy-updates,now 0.30-10ubuntu1.22.04.1 amd64 [installed,automatic]
libcanberra0/jammy-updates,now 0.30-10ubuntu1.22.04.1 amd64 [installed,automatic]
libcap-ng0/jammy,now 0.7.9-2.2build3 amd64 [installed,automatic]
libcap2-bin/jammy-updates,jammy-security,now 1:2.44-1ubuntu0.22.04.1 amd64 [installed,automatic]
libcap2/jammy-updates,jammy-security,now 1:2.44-1ubuntu0.22.04.1 amd64 [installed,automatic]
libcbor0.8/jammy,now 0.8.0-2ubuntu1 amd64 [installed,automatic]
libcdio-cdda2/jammy,now 10.2+2.0.0-1build3 amd64 [installed,automatic]
libcdio-paranoia2/jammy,now 10.2+2.0.0-1build3 amd64 [installed,automatic]
libcdio19/jammy,now 2.1.0-3build1 amd64 [installed,automatic]
libcdparanoia0/jammy,now 3.10.2+debian-14build2 amd64 [installed,automatic]
libcdr-0.1-1/jammy,now 0.1.6-2build2 amd64 [installed,automatic]
libcheese-gtk25/jammy,now 41.1-1build1 amd64 [installed,automatic]
libcheese8/jammy,now 41.1-1build1 amd64 [installed,automatic]
libclone-perl/jammy,now 0.45-1build3 amd64 [installed,automatic]
libclucene-contribs1v5/jammy,now 2.3.3.4+dfsg-1ubuntu5 amd64 [installed,automatic]
libclucene-core1v5/jammy,now 2.3.3.4+dfsg-1ubuntu5 amd64 [installed,automatic]
libclutter-1.0-0/jammy,now 1.26.4+dfsg-4build1 amd64 [installed,automatic]
libclutter-1.0-common/jammy,jammy,now 1.26.4+dfsg-4build1 all [installed,automatic]
libclutter-gst-3.0-0/jammy-updates,now 3.0.27-2ubuntu1 amd64 [installed,automatic]
libclutter-gtk-1.0-0/jammy,now 1.8.4-4build2 amd64 [installed,automatic]
libcogl-common/jammy,jammy,now 1.22.8-3build1 all [installed,automatic]
libcogl-pango20/jammy,now 1.22.8-3build1 amd64 [installed,automatic]
libcogl-path20/jammy,now 1.22.8-3build1 amd64 [installed,automatic]
libcogl20/jammy,now 1.22.8-3build1 amd64 [installed,automatic]
libcolamd2/jammy,now 1:5.10.1+dfsg-4build1 amd64 [installed,automatic]
libcolord-gtk1/jammy,now 0.3.0-1 amd64 [installed,automatic]
libcolord2/jammy,now 1.4.6-1 amd64 [installed,automatic]
libcolorhug2/jammy,now 1.4.6-1 amd64 [installed,automatic]
libcom-err2/jammy-updates,jammy-security,now 1.46.5-2ubuntu1.1 amd64 [installed,automatic]
libcrack2/jammy,now 2.9.6-3.4build4 amd64 [installed,automatic]
libcrypt1/jammy,now 1:4.4.27-1 amd64 [installed,automatic]
libcryptsetup12/jammy-updates,now 2:2.4.3-1ubuntu1.1 amd64 [installed,automatic]
libcue2/jammy,now 2.2.1-3build3 amd64 [installed,automatic]
libcups2/jammy-updates,jammy-security,now 2.4.1op1-1ubuntu4.4 amd64 [installed,automatic]
libcupsfilters1/jammy-updates,jammy-security,now 1.28.15-0ubuntu1.2 amd64 [installed,automatic]
libcupsimage2/jammy-updates,jammy-security,now 2.4.1op1-1ubuntu4.4 amd64 [installed,automatic]
libcurl3-gnutls/jammy-updates,jammy-security,now 7.81.0-1ubuntu1.13 amd64 [installed,automatic]
libcurl4/jammy-updates,jammy-security,now 7.81.0-1ubuntu1.13 amd64 [installed,automatic]
libdaemon0/jammy,now 0.14-7.1ubuntu3 amd64 [installed,automatic]
libdata-dump-perl/jammy,jammy,now 1.25-1 all [installed,automatic]
libdatrie1/jammy,now 0.2.13-2 amd64 [installed,automatic]
libdazzle-1.0-0/jammy,now 3.44.0-1 amd64 [installed,automatic]
libdazzle-common/jammy,jammy,now 3.44.0-1 all [installed,automatic]
libdb5.3/jammy,now 5.3.28+dfsg1-0.8ubuntu3 amd64 [installed,automatic]
libdbus-1-3/jammy-updates,jammy-security,now 1.12.20-2ubuntu4.1 amd64 [installed,automatic]
libdbus-glib-1-2/jammy,now 0.112-2build1 amd64 [installed,automatic]
libdbusmenu-glib4/jammy,now 16.04.1+18.10.20180917-0ubuntu8 amd64 [installed,automatic]
libdbusmenu-gtk3-4/jammy,now 16.04.1+18.10.20180917-0ubuntu8 amd64 [installed,automatic]
libdbusmenu-qt5-2/jammy,now 0.9.3+16.04.20160218-2build1 amd64 [installed,automatic]
libdconf1/jammy,now 0.40.0-3 amd64 [installed,automatic]
libdebconfclient0/jammy,now 0.261ubuntu1 amd64 [installed]
libdebuginfod-common/jammy,jammy,now 0.186-1build1 all [installed,automatic]
libdebuginfod1/jammy,now 0.186-1build1 amd64 [installed,automatic]
libdee-1.0-4/jammy,now 1.2.7+17.10.20170616-6ubuntu4 amd64 [installed,automatic]
libdeflate0/jammy,now 1.10-2 amd64 [installed,automatic]
libdevmapper1.02.1/jammy,now 2:1.02.175-2.1ubuntu4 amd64 [installed,automatic]
libdjvulibre-text/jammy,jammy,now 3.5.28-2build2 all [installed,automatic]
libdjvulibre21/jammy,now 3.5.28-2build2 amd64 [installed,automatic]
libdmapsharing-3.0-2/jammy,now 2.9.41-3build2 amd64 [installed,automatic]
libdns-export1110/jammy,now 1:9.11.19+dfsg-2.1ubuntu3 amd64 [installed,automatic]
libdotconf0/jammy,now 1.3-0.3fakesync1build2 amd64 [installed,automatic]
libdouble-conversion3/jammy,now 3.1.7-4 amd64 [installed,automatic]
libdrm-amdgpu1/jammy-updates,now 2.4.113-2~ubuntu0.22.04.1 amd64 [installed,automatic]
libdrm-common/jammy-updates,jammy-updates,now 2.4.113-2~ubuntu0.22.04.1 all [installed,automatic]
libdrm-intel1/jammy-updates,now 2.4.113-2~ubuntu0.22.04.1 amd64 [installed,automatic]
libdrm-nouveau2/jammy-updates,now 2.4.113-2~ubuntu0.22.04.1 amd64 [installed,automatic]
libdrm-radeon1/jammy-updates,now 2.4.113-2~ubuntu0.22.04.1 amd64 [installed,automatic]
libdrm2/jammy-updates,now 2.4.113-2~ubuntu0.22.04.1 amd64 [installed,automatic]
libdv4/jammy,now 1.0.0-14build1 amd64 [installed,automatic]
libdw1/jammy,now 0.186-1build1 amd64 [installed,automatic]
libe-book-0.1-1/jammy,now 0.1.3-2build2 amd64 [installed,automatic]
libebackend-1.2-10/jammy-updates,now 3.44.4-0ubuntu1 amd64 [installed,automatic]
libebook-1.2-20/jammy-updates,now 3.44.4-0ubuntu1 amd64 [installed,automatic]
libebook-contacts-1.2-3/jammy-updates,now 3.44.4-0ubuntu1 amd64 [installed,automatic]
libecal-2.0-1/jammy-updates,now 3.44.4-0ubuntu1 amd64 [installed,automatic]
libedata-book-1.2-26/jammy-updates,now 3.44.4-0ubuntu1 amd64 [installed,automatic]
libedata-cal-2.0-1/jammy-updates,now 3.44.4-0ubuntu1 amd64 [installed,automatic]
libedataserver-1.2-26/jammy-updates,now 3.44.4-0ubuntu1 amd64 [installed,automatic]
libedataserverui-1.2-3/jammy-updates,now 3.44.4-0ubuntu1 amd64 [installed,automatic]
libedit2/jammy,now 3.1-20210910-1build1 amd64 [installed,automatic]
libefiboot1/jammy,now 37-6ubuntu2 amd64 [installed,automatic]
libefivar1/jammy,now 37-6ubuntu2 amd64 [installed,automatic]
libegl-mesa0/jammy-updates,now 22.2.5-0ubuntu0.1~22.04.3 amd64 [installed,automatic]
libegl1/jammy,now 1.4.0-1 amd64 [installed,automatic]
libelf1/jammy,now 0.186-1build1 amd64 [installed,automatic]
libenchant-2-2/jammy,now 2.3.2-1ubuntu2 amd64 [installed,automatic]
libencode-locale-perl/jammy,jammy,now 1.05-1.1 all [installed,automatic]
libeot0/jammy,now 0.01-5build2 amd64 [installed,automatic]
libepoxy0/jammy,now 1.5.10-1 amd64 [installed,automatic]
libepubgen-0.1-1/jammy,now 0.1.1-1ubuntu5 amd64 [installed,automatic]
libespeak-ng1/jammy,now 1.50+dfsg-10 amd64 [installed,automatic]
libestr0/jammy,now 0.1.10-2.1build3 amd64 [installed,automatic]
libetonyek-0.1-1/jammy,now 0.1.10-3build1 amd64 [installed,automatic]
libevdev2/jammy,now 1.12.1+dfsg-1 amd64 [installed,automatic]
libevdocument3-4/jammy-updates,now 42.3-0ubuntu3 amd64 [installed,automatic]
libevent-2.1-7/jammy,now 2.1.12-stable-1build3 amd64 [installed,automatic]
libevview3-3/jammy-updates,now 42.3-0ubuntu3 amd64 [installed,automatic]
libexempi8/jammy-updates,jammy-security,now 2.5.2-1ubuntu0.22.04.1 amd64 [installed,automatic]
libexif12/jammy,now 0.6.24-1build1 amd64 [installed,automatic]
libexiv2-27/jammy,now 0.27.5-3ubuntu1 amd64 [installed,automatic]
libexpat1/jammy-updates,jammy-security,now 2.4.7-1ubuntu0.2 amd64 [installed,automatic]
libext2fs2/jammy-updates,jammy-security,now 1.46.5-2ubuntu1.1 amd64 [installed,automatic]
libexttextcat-2.0-0/jammy,now 3.4.5-1build2 amd64 [installed,automatic]
libexttextcat-data/jammy,jammy,now 3.4.5-1build2 all [installed,automatic]
libextutils-depends-perl/jammy,jammy,now 0.8001-1 all [installed,automatic]
libfastjson4/jammy,now 0.99.9-1build2 amd64 [installed,automatic]
libfdisk1/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
libffi8/jammy,now 3.4.2-4 amd64 [installed,automatic]
libfftw3-single3/jammy,now 3.3.8-2ubuntu8 amd64 [installed,automatic]
libfido2-1/jammy,now 1.10.0-1 amd64 [installed,automatic]
libfile-basedir-perl/jammy,jammy,now 0.09-1 all [installed,automatic]
libfile-desktopentry-perl/jammy,jammy,now 0.22-2 all [installed,automatic]
libfile-listing-perl/jammy,jammy,now 6.14-1 all [installed,automatic]
libfile-mimeinfo-perl/jammy,jammy,now 0.31-1 all [installed,automatic]
libflac8/jammy-updates,jammy-security,now 1.3.3-2ubuntu0.1 amd64 [installed,automatic]
libflashrom1/jammy,now 1.2-5build1 amd64 [installed]
libfont-afm-perl/jammy,jammy,now 1.20-3 all [installed,automatic]
libfontconfig1/jammy,now 2.13.1-4.2ubuntu5 amd64 [installed,automatic]
libfontembed1/jammy-updates,jammy-security,now 1.28.15-0ubuntu1.2 amd64 [installed,automatic]
libfontenc1/jammy,now 1:1.1.4-1build3 amd64 [installed,automatic]
libfprint-2-2/jammy-updates,now 1:1.94.3+tod1-0ubuntu2~22.04.04 amd64 [installed,automatic]
libfreehand-0.1-1/jammy,now 0.1.2-3build2 amd64 [installed,automatic]
libfreerdp-client2-2/jammy-updates,jammy-security,now 2.6.1+dfsg1-3ubuntu2.3 amd64 [installed,automatic]
libfreerdp-server2-2/jammy-updates,jammy-security,now 2.6.1+dfsg1-3ubuntu2.3 amd64 [installed,automatic]
libfreerdp2-2/jammy-updates,jammy-security,now 2.6.1+dfsg1-3ubuntu2.3 amd64 [installed,automatic]
libfreetype6/jammy-updates,jammy-security,now 2.11.1+dfsg-1ubuntu0.2 amd64 [installed,automatic]
libfribidi0/jammy-updates,jammy-security,now 1.0.8-2ubuntu3.1 amd64 [installed,automatic]
libftdi1-2/jammy,now 1.5-5build3 amd64 [installed]
libfuse3-3/jammy,now 3.10.5-1build1 amd64 [installed,automatic]
libfwupd2/jammy-updates,now 1.7.9-1~22.04.3 amd64 [installed,automatic]
libfwupdplugin5/jammy-updates,now 1.7.9-1~22.04.3 amd64 [installed,automatic]
libgail-common/jammy,now 2.24.33-2ubuntu2 amd64 [installed,automatic]
libgail18/jammy,now 2.24.33-2ubuntu2 amd64 [installed,automatic]
libgamemode0/jammy,now 1.6.1-1build2 amd64 [installed,automatic]
libgamemodeauto0/jammy,now 1.6.1-1build2 amd64 [installed,automatic]
libgamin0/jammy,now 0.1.10-6 amd64 [installed,automatic]
libgbm1/jammy-updates,now 22.2.5-0ubuntu0.1~22.04.3 amd64 [installed,automatic]
libgc1/jammy,now 1:8.0.6-1.1build1 amd64 [installed,automatic]
libgcab-1.0-0/jammy,now 1.4-3build2 amd64 [installed,automatic]
libgcc-s1/jammy-updates,jammy-security,now 12.1.0-2ubuntu1~22.04 amd64 [installed,automatic]
libgck-1-0/jammy,now 3.40.0-4 amd64 [installed,automatic]
libgcr-base-3-1/jammy,now 3.40.0-4 amd64 [installed,automatic]
libgcr-ui-3-1/jammy,now 3.40.0-4 amd64 [installed,automatic]
libgcrypt20/jammy,now 1.9.4-3ubuntu3 amd64 [installed,automatic]
libgd3/jammy,now 2.3.0-2ubuntu2 amd64 [installed,automatic]
libgdata-common/jammy,jammy,now 0.18.1-2build1 all [installed,automatic]
libgdata22/jammy,now 0.18.1-2build1 amd64 [installed,automatic]
libgdbm-compat4/jammy,now 1.23-1 amd64 [installed,automatic]
libgdbm6/jammy,now 1.23-1 amd64 [installed,automatic]
libgdk-pixbuf-2.0-0/jammy-updates,now 2.42.8+dfsg-1ubuntu0.2 amd64 [installed,automatic]
libgdk-pixbuf2.0-bin/jammy-updates,now 2.42.8+dfsg-1ubuntu0.2 amd64 [installed,automatic]
libgdk-pixbuf2.0-common/jammy-updates,jammy-updates,now 2.42.8+dfsg-1ubuntu0.2 all [installed,automatic]
libgdm1/jammy-updates,now 42.0-1ubuntu7.22.04.3 amd64 [installed,automatic]
libgee-0.8-2/jammy,now 0.20.5-2 amd64 [installed,automatic]
libgeoclue-2-0/jammy,now 2.5.7-3ubuntu3 amd64 [installed,automatic]
libgeocode-glib0/jammy,now 3.26.2-2build2 amd64 [installed,automatic]
libgexiv2-2/jammy,now 0.14.0-1build1 amd64 [installed,automatic]
libgif7/jammy,now 5.1.9-2build2 amd64 [installed,automatic]
libgirepository-1.0-1/jammy,now 1.72.0-1 amd64 [installed,automatic]
libgjs0g/now 1.72.2-0ubuntu2 amd64 [installed,upgradable to: 1.72.4-0ubuntu0.22.04.1]
libgl1-amber-dri/jammy,now 21.3.7-0ubuntu1 amd64 [installed,automatic]
libgl1-mesa-dri/jammy-updates,now 22.2.5-0ubuntu0.1~22.04.3 amd64 [installed,automatic]
libgl1/jammy,now 1.4.0-1 amd64 [installed,automatic]
libglapi-mesa/jammy-updates,now 22.2.5-0ubuntu0.1~22.04.3 amd64 [installed,automatic]
libgles2/jammy,now 1.4.0-1 amd64 [installed,automatic]
libglib-object-introspection-perl/jammy,now 0.049-1+build2 amd64 [installed,automatic]
libglib-perl/jammy,now 3:1.329.3-2build1 amd64 [installed,automatic]
libglib2.0-0/jammy-updates,jammy-security,now 2.72.4-0ubuntu2.2 amd64 [installed,automatic]
libglib2.0-bin/jammy-updates,jammy-security,now 2.72.4-0ubuntu2.2 amd64 [installed,automatic]
libglib2.0-data/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2.72.4-0ubuntu2.2 all [installed,automatic]
libglibmm-2.4-1v5/jammy,now 2.66.2-2 amd64 [installed,automatic]
libglu1-mesa/jammy,now 9.0.2-1 amd64 [installed,automatic]
libglvnd0/jammy,now 1.4.0-1 amd64 [installed,automatic]
libglx-mesa0/jammy-updates,now 22.2.5-0ubuntu0.1~22.04.3 amd64 [installed,automatic]
libglx0/jammy,now 1.4.0-1 amd64 [installed,automatic]
libgmp10/jammy,now 2:6.2.1+dfsg-3ubuntu1 amd64 [installed,automatic]
libgnome-autoar-0-0/jammy,now 0.4.3-1 amd64 [installed,automatic]
libgnome-bg-4-1/now 42.5-0ubuntu1 amd64 [installed,upgradable to: 42.9-0ubuntu1]
libgnome-bluetooth-3.0-13/jammy,now 42.0-5 amd64 [installed,automatic]
libgnome-bluetooth13/jammy,now 3.34.5-8 amd64 [installed,automatic]
libgnome-desktop-3-19/now 42.5-0ubuntu1 amd64 [installed,upgradable to: 42.9-0ubuntu1]
libgnome-desktop-4-1/now 42.5-0ubuntu1 amd64 [installed,upgradable to: 42.9-0ubuntu1]
libgnome-games-support-1-3/jammy,now 1.8.2-1build1 amd64 [installed,automatic]
libgnome-games-support-common/jammy,jammy,now 1.8.2-1build1 all [installed,automatic]
libgnome-menu-3-0/jammy,now 3.36.0-1ubuntu3 amd64 [installed,automatic]
libgnome-todo/jammy,now 3.28.1-6ubuntu1 amd64 [installed,automatic]
libgnomekbd-common/jammy,jammy,now 3.26.1-2 all [installed,automatic]
libgnomekbd8/jammy,now 3.26.1-2 amd64 [installed,automatic]
libgnutls30/jammy-updates,jammy-security,now 3.7.3-4ubuntu1.2 amd64 [installed,automatic]
libgoa-1.0-0b/jammy,now 3.44.0-1ubuntu1 amd64 [installed,automatic]
libgoa-1.0-common/jammy,jammy,now 3.44.0-1ubuntu1 all [installed,automatic]
libgoa-backend-1.0-1/jammy,now 3.44.0-1ubuntu1 amd64 [installed,automatic]
libgom-1.0-0/jammy,now 0.4-1build2 amd64 [installed,automatic]
libgomp1/jammy-updates,jammy-security,now 12.1.0-2ubuntu1~22.04 amd64 [installed,automatic]
libgpg-error0/jammy,now 1.43-3 amd64 [installed,automatic]
libgpgme11/jammy,now 1.16.0-1.2ubuntu4 amd64 [installed,automatic]
libgpgmepp6/jammy,now 1.16.0-1.2ubuntu4 amd64 [installed,automatic]
libgphoto2-6/jammy,now 2.5.27-1build2 amd64 [installed,automatic]
libgphoto2-l10n/jammy,jammy,now 2.5.27-1build2 all [installed,automatic]
libgphoto2-port12/jammy,now 2.5.27-1build2 amd64 [installed,automatic]
libgpm2/jammy,now 1.20.7-10build1 amd64 [installed,automatic]
libgpod-common/jammy,now 0.8.3-16build2 amd64 [installed,automatic]
libgpod4/jammy,now 0.8.3-16build2 amd64 [installed,automatic]
libgraphene-1.0-0/jammy,now 1.10.8-1 amd64 [installed,automatic]
libgraphite2-3/jammy,now 1.3.14-1build2 amd64 [installed,automatic]
libgrilo-0.3-0/jammy,now 0.3.14-1build1 amd64 [installed,automatic]
libgs9-common/jammy-updates,jammy-updates,jammy-security,jammy-security,now 9.55.0~dfsg1-0ubuntu5.3 all [installed,automatic]
libgs9/jammy-updates,jammy-security,now 9.55.0~dfsg1-0ubuntu5.3 amd64 [installed,automatic]
libgsf-1-114/jammy,now 1.14.47-1build2 amd64 [installed,automatic]
libgsf-1-common/jammy,jammy,now 1.14.47-1build2 all [installed,automatic]
libgsound0/jammy,now 1.0.3-2build1 amd64 [installed,automatic]
libgspell-1-2/jammy,now 1.9.1-4 amd64 [installed,automatic]
libgspell-1-common/jammy,jammy,now 1.9.1-4 all [installed,automatic]
libgssapi-krb5-2/jammy-updates,now 1.19.2-2ubuntu0.2 amd64 [installed,automatic]
libgssdp-1.2-0/jammy,now 1.4.0.1-2build1 amd64 [installed,automatic]
libgstreamer-gl1.0-0/jammy,now 1.20.1-1 amd64 [installed,automatic]
libgstreamer-plugins-base1.0-0/jammy,now 1.20.1-1 amd64 [installed,automatic]
libgstreamer-plugins-good1.0-0/jammy-updates,now 1.20.3-0ubuntu1 amd64 [installed,automatic]
libgstreamer1.0-0/jammy-updates,now 1.20.3-0ubuntu1 amd64 [installed,automatic]
libgtk-3-0/jammy-updates,now 3.24.33-1ubuntu2 amd64 [installed,automatic]
libgtk-3-bin/jammy-updates,now 3.24.33-1ubuntu2 amd64 [installed,automatic]
libgtk-3-common/jammy-updates,jammy-updates,now 3.24.33-1ubuntu2 all [installed,automatic]
libgtk-4-1/jammy-updates,now 4.6.6+ds-0ubuntu1 amd64 [installed,automatic]
libgtk-4-bin/jammy-updates,now 4.6.6+ds-0ubuntu1 amd64 [installed,automatic]
libgtk-4-common/jammy-updates,jammy-updates,now 4.6.6+ds-0ubuntu1 all [installed,automatic]
libgtk2.0-0/jammy,now 2.24.33-2ubuntu2 amd64 [installed,automatic]
libgtk2.0-bin/jammy,now 2.24.33-2ubuntu2 amd64 [installed,automatic]
libgtk2.0-common/jammy,jammy,now 2.24.33-2ubuntu2 all [installed,automatic]
libgtk3-perl/jammy,jammy,now 0.038-1 all [installed,automatic]
libgtkmm-3.0-1v5/jammy,now 3.24.5-1build1 amd64 [installed,automatic]
libgtksourceview-4-0/jammy,now 4.8.3-1 amd64 [installed,automatic]
libgtksourceview-4-common/jammy,jammy,now 4.8.3-1 all [installed,automatic]
libgtop-2.0-11/jammy,now 2.40.0-2build3 amd64 [installed,automatic]
libgtop2-common/jammy,jammy,now 2.40.0-2build3 all [installed,automatic]
libgudev-1.0-0/jammy,now 1:237-2build1 amd64 [installed,automatic]
libgupnp-1.2-1/jammy,now 1.4.3-1 amd64 [installed,automatic]
libgupnp-av-1.0-3/jammy,now 0.14.0-3 amd64 [installed,automatic]
libgupnp-dlna-2.0-4/jammy,now 0.12.0-3 amd64 [installed,automatic]
libgusb2/jammy,now 0.3.10-1 amd64 [installed,automatic]
libgweather-3-16/jammy,now 40.0-5build1 amd64 [installed,automatic]
libgweather-common/jammy,jammy,now 40.0-5build1 all [installed,automatic]
libgxps2/jammy,now 0.3.2-2 amd64 [installed,automatic]
libhandy-1-0/jammy,now 1.6.1-1 amd64 [installed,automatic]
libharfbuzz-icu0/jammy-updates,jammy-security,now 2.7.4-1ubuntu3.1 amd64 [installed,automatic]
libharfbuzz0b/jammy-updates,jammy-security,now 2.7.4-1ubuntu3.1 amd64 [installed,automatic]
libhfstospell11/jammy,now 0.5.2-1build3 amd64 [installed,automatic]
libhogweed6/jammy,now 3.7.3-1build2 amd64 [installed,automatic]
libhpmud0/jammy,now 3.21.12+dfsg0-1 amd64 [installed,automatic]
libhtml-form-perl/jammy,jammy,now 6.07-1 all [installed,automatic]
libhtml-format-perl/jammy,jammy,now 2.12-1.1 all [installed,automatic]
libhtml-parser-perl/jammy,now 3.76-1build2 amd64 [installed,automatic]
libhtml-tagset-perl/jammy,jammy,now 3.20-4 all [installed,automatic]
libhtml-tree-perl/jammy,jammy,now 5.07-2 all [installed,automatic]
libhttp-cookies-perl/jammy,jammy,now 6.10-1 all [installed,automatic]
libhttp-daemon-perl/jammy-updates,jammy-updates,jammy-security,jammy-security,now 6.13-1ubuntu0.1 all [installed,automatic]
libhttp-date-perl/jammy,jammy,now 6.05-1 all [installed,automatic]
libhttp-message-perl/jammy,jammy,now 6.36-1 all [installed,automatic]
libhttp-negotiate-perl/jammy,jammy,now 6.01-1 all [installed,automatic]
libhunspell-1.7-0/jammy,now 1.7.0-4build1 amd64 [installed,automatic]
libhyphen0/jammy,now 2.8.8-7build2 amd64 [installed,automatic]
libibus-1.0-5/jammy,now 1.5.26-4 amd64 [installed,automatic]
libical3/jammy,now 3.0.14-1build1 amd64 [installed,automatic]
libice6/jammy,now 2:1.0.10-1build2 amd64 [installed,automatic]
libicu70/jammy,now 70.1-2 amd64 [installed,automatic]
libidn12/jammy,now 1.38-4build1 amd64 [installed,upgradable to: 1.38-4ubuntu1]
libidn2-0/jammy,now 2.3.2-2build1 amd64 [installed,automatic]
libiec61883-0/jammy,now 1.2.0-4build3 amd64 [installed,automatic]
libieee1284-3/jammy,now 0.2.11-14build2 amd64 [installed,automatic]
libijs-0.35/jammy,now 0.35-15build2 amd64 [installed,automatic]
libimagequant0/jammy,now 2.17.0-1 amd64 [installed,automatic]
libimobiledevice6/jammy,now 1.3.0-6build3 amd64 [installed,automatic]
libinih1/jammy,now 53-1ubuntu3 amd64 [installed,automatic]
libinput-bin/now 1.20.0-1ubuntu0.2 amd64 [installed,upgradable to: 1.20.0-1ubuntu0.3]
libinput10/now 1.20.0-1ubuntu0.2 amd64 [installed,upgradable to: 1.20.0-1ubuntu0.3]
libio-html-perl/jammy,jammy,now 1.004-2 all [installed,automatic]
libio-socket-ssl-perl/jammy,jammy,now 2.074-2 all [installed,automatic]
libio-stringy-perl/jammy,jammy,now 2.111-3 all [installed,automatic]
libip4tc2/jammy-updates,now 1.8.7-1ubuntu5.1 amd64 [installed,automatic]
libip6tc2/jammy-updates,now 1.8.7-1ubuntu5.1 amd64 [installed,automatic]
libipc-system-simple-perl/jammy,jammy,now 1.30-1 all [installed,automatic]
libipt2/jammy,now 2.0.5-1 amd64 [installed,automatic]
libisc-export1105/jammy,now 1:9.11.19+dfsg-2.1ubuntu3 amd64 [installed,automatic]
libisl23/jammy,now 0.24-2build1 amd64 [installed,automatic]
libiw30/jammy,now 30~pre9-13.1ubuntu4 amd64 [installed,automatic]
libjack-jackd2-0/jammy,now 1.9.20~dfsg-1 amd64 [installed,automatic]
libjansson4/jammy,now 2.13.1-1.1build3 amd64 [installed,automatic]
libjavascriptcoregtk-4.0-18/jammy-updates,jammy-security,now 2.38.6-0ubuntu0.22.04.1 amd64 [installed,automatic]
libjbig0/jammy-updates,jammy-security,now 2.1-3.1ubuntu0.22.04.1 amd64 [installed,automatic]
libjbig2dec0/jammy,now 0.19-3build2 amd64 [installed,automatic]
libjcat1/jammy,now 0.1.9-1 amd64 [installed,automatic]
libjpeg-turbo8/jammy,now 2.1.2-0ubuntu1 amd64 [installed,automatic]
libjpeg8/jammy,now 8c-2ubuntu10 amd64 [installed,automatic]
libjson-c5/jammy-updates,now 0.15-3~ubuntu1.22.04.1 amd64 [installed,automatic]
libjson-glib-1.0-0/jammy,now 1.6.6-1build1 amd64 [installed,automatic]
libjson-glib-1.0-common/jammy,jammy,now 1.6.6-1build1 all [installed,automatic]
libk5crypto3/jammy-updates,now 1.19.2-2ubuntu0.2 amd64 [installed,automatic]
libkeyutils1/jammy,now 1.6.1-2ubuntu3 amd64 [installed,automatic]
libkf5archive5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5auth-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5authcore5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5codecs-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5codecs5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5completion-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5completion5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5config-bin/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5config-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5configcore5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5configgui5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5configwidgets-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5configwidgets5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5coreaddons-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5coreaddons5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5crash5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5dbusaddons-bin/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5dbusaddons-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5dbusaddons5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5doctools5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5globalaccel-bin/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5globalaccel-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5globalaccel5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5globalaccelprivate5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5guiaddons-bin/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5guiaddons-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5guiaddons5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5i18n-data/jammy,jammy,now 5.92.0-0ubuntu2 all [installed,automatic]
libkf5i18n5/jammy,now 5.92.0-0ubuntu2 amd64 [installed,automatic]
libkf5iconthemes-bin/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5iconthemes-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5iconthemes5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5idletime5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5itemviews-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5itemviews5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5jobwidgets-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5jobwidgets5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5kiocore5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5kiogui5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5kiontlm5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5kiowidgets5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5notifications-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5notifications5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5parts-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5parts-plugins/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5parts5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5service-bin/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5service-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5service5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5solid5-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5solid5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5sonnet5-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5sonnetcore5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5sonnetui5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5textwidgets-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5textwidgets5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5wallet-bin/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5wallet-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5wallet5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5waylandclient5/jammy,now 4:5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5widgetsaddons-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5widgetsaddons5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5windowsystem-data/jammy,jammy,now 5.92.0-0ubuntu1 all [installed,automatic]
libkf5windowsystem5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
libkf5xmlgui-bin/jammy,now 5.92.0-0ubuntu2 amd64 [installed,automatic]
libkf5xmlgui-data/jammy,jammy,now 5.92.0-0ubuntu2 all [installed,automatic]
libkf5xmlgui5/jammy,now 5.92.0-0ubuntu2 amd64 [installed,automatic]
libklibc/jammy,now 2.0.10-4 amd64 [installed,automatic]
libkmod2/jammy,now 29-1ubuntu1 amd64 [installed,automatic]
libkpathsea6/jammy-updates,jammy-security,now 2021.20210626.59705-1ubuntu0.1 amd64 [installed,automatic]
libkpmcore11/jammy,now 21.12.3-0ubuntu1 amd64 [installed,automatic]
libkrb5-3/jammy-updates,now 1.19.2-2ubuntu0.2 amd64 [installed,automatic]
libkrb5support0/jammy-updates,now 1.19.2-2ubuntu0.2 amd64 [installed,automatic]
libksba8/jammy-updates,jammy-security,now 1.6.0-2ubuntu0.2 amd64 [installed,automatic]
libkwalletbackend5-5/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
liblangtag-common/jammy,jammy,now 0.6.3-2ubuntu1 all [installed,automatic]
liblangtag1/jammy,now 0.6.3-2ubuntu1 amd64 [installed,automatic]
liblcms2-2/jammy,now 2.12~rc1-2build2 amd64 [installed,automatic]
liblcms2-utils/jammy,now 2.12~rc1-2build2 amd64 [installed,automatic]
libldap-2.5-0/jammy-updates,now 2.5.14+dfsg-0ubuntu0.22.04.2 amd64 [installed,automatic]
libldap-common/jammy-updates,jammy-updates,now 2.5.14+dfsg-0ubuntu0.22.04.2 all [installed,automatic]
libldb2/jammy-updates,jammy-security,now 2:2.4.4-0ubuntu0.22.04.2 amd64 [installed,automatic]
liblirc-client0/jammy,now 0.10.1-6.3ubuntu1 amd64 [installed,automatic]
libllvm13/jammy-updates,jammy-security,now 1:13.0.1-2ubuntu2.1 amd64 [installed]
libllvm15/jammy-updates,jammy-security,now 1:15.0.7-0ubuntu0.22.04.2 amd64 [installed,automatic]
liblmdb0/jammy,now 0.9.24-1build2 amd64 [installed,automatic]
liblocale-gettext-perl/jammy,now 1.07-4build3 amd64 [installed,automatic]
liblouis-data/jammy-updates,jammy-updates,jammy-security,jammy-security,now 3.20.0-2ubuntu0.2 all [installed,automatic]
liblouis20/jammy-updates,jammy-security,now 3.20.0-2ubuntu0.2 amd64 [installed,automatic]
liblouisutdml-bin/jammy,now 2.10.0-4 amd64 [installed,automatic]
liblouisutdml-data/jammy,jammy,now 2.10.0-4 all [installed,automatic]
liblouisutdml9/jammy,now 2.10.0-4 amd64 [installed,automatic]
libltdl7/jammy,now 2.4.6-15build2 amd64 [installed,automatic]
liblua5.3-0/jammy,now 5.3.6-1build1 amd64 [installed,automatic]
liblwp-mediatypes-perl/jammy,jammy,now 6.04-1 all [installed,automatic]
liblwp-protocol-https-perl/jammy,jammy,now 6.10-1 all [installed,automatic]
liblz4-1/jammy,now 1.9.3-2build2 amd64 [installed,automatic]
liblzma5/jammy,now 5.2.5-2ubuntu1 amd64 [installed,automatic]
liblzo2-2/jammy,now 2.10-2build3 amd64 [installed,automatic]
libmagic-mgc/jammy,now 1:5.41-3 amd64 [installed,automatic]
libmagic1/jammy,now 1:5.41-3 amd64 [installed,automatic]
libmailtools-perl/jammy,jammy,now 2.21-1 all [installed,automatic]
libmanette-0.2-0/jammy,now 0.2.6-3build1 amd64 [installed,automatic]
libmaxminddb0/jammy,now 1.5.2-1build2 amd64 [installed,automatic]
libmbim-glib4/jammy-updates,now 1.28.0-1~ubuntu20.04.1 amd64 [installed,automatic]
libmbim-proxy/jammy-updates,now 1.28.0-1~ubuntu20.04.1 amd64 [installed,automatic]
libmd0/jammy,now 1.0.4-1build1 amd64 [installed,automatic]
libmd4c0/jammy,now 0.4.8-1 amd64 [installed,automatic]
libmediaart-2.0-0/jammy,now 1.9.5-2build1 amd64 [installed,automatic]
libmessaging-menu0/jammy,now 22.2.0-1 amd64 [installed,automatic]
libmhash2/jammy,now 0.9.9.9-9build2 amd64 [installed,automatic]
libminiupnpc17/jammy,now 2.2.3-1build1 amd64 [installed,automatic]
libmm-glib0/jammy-updates,now 1.20.0-1~ubuntu22.04.2 amd64 [installed,automatic]
libmnl0/jammy,now 1.0.4-3build2 amd64 [installed,automatic]
libmount1/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
libmozjs-91-0/jammy-updates,jammy-security,now 91.10.0-0ubuntu1 amd64 [installed,automatic]
libmp3lame0/jammy,now 3.100-3build2 amd64 [installed,automatic]
libmpc3/jammy,now 1.2.1-2build1 amd64 [installed,automatic]
libmpdec3/jammy,now 2.5.1-2build2 amd64 [installed,automatic]
libmpfr6/jammy,now 4.1.0-3build3 amd64 [installed,automatic]
libmpg123-0/jammy,now 1.29.3-1build1 amd64 [installed,automatic]
libmspack0/jammy,now 0.10.1-2build2 amd64 [installed,automatic]
libmspub-0.1-1/jammy,now 0.1.4-3build3 amd64 [installed,automatic]
libmtdev1/jammy,now 1.1.6-1build4 amd64 [installed,automatic]
libmtp-common/jammy,jammy,now 1.1.19-1build1 all [installed,automatic]
libmtp-runtime/jammy,now 1.1.19-1build1 amd64 [installed,automatic]
libmtp9/jammy,now 1.1.19-1build1 amd64 [installed,automatic]
libmutter-10-0/now 42.5-0ubuntu1 amd64 [installed,upgradable to: 42.9-0ubuntu1]
libmwaw-0.3-3/jammy,now 0.3.21-1build1 amd64 [installed,automatic]
libmythes-1.2-0/jammy,now 2:1.2.4-4build1 amd64 [installed,automatic]
libnatpmp1/jammy,now 20150609-7.1build2 amd64 [installed,automatic]
libnautilus-extension1a/jammy-updates,now 1:42.6-0ubuntu1 amd64 [installed,automatic]
libncurses6/jammy-updates,jammy-security,now 6.3-2ubuntu0.1 amd64 [installed,automatic]
libncursesw6/jammy-updates,jammy-security,now 6.3-2ubuntu0.1 amd64 [installed,automatic]
libndp0/jammy,now 1.8-0ubuntu3 amd64 [installed,automatic]
libnet-dbus-perl/jammy,now 1.2.0-1build3 amd64 [installed,automatic]
libnet-http-perl/jammy,jammy,now 6.22-1 all [installed,automatic]
libnet-smtp-ssl-perl/jammy,jammy,now 1.04-1 all [installed,automatic]
libnet-ssleay-perl/jammy,now 1.92-1build2 amd64 [installed,automatic]
libnetfilter-conntrack3/jammy,now 1.0.9-1 amd64 [installed,automatic]
libnetplan0/jammy-updates,now 0.105-0ubuntu2~22.04.3 amd64 [installed,automatic]
libnettle8/jammy,now 3.7.3-1build2 amd64 [installed,automatic]
libnewt0.52/jammy,now 0.52.21-5ubuntu2 amd64 [installed,automatic]
libnfnetlink0/jammy,now 1.0.1-3build3 amd64 [installed,automatic]
libnfs13/jammy,now 4.0.0-1build2 amd64 [installed,automatic]
libnftables1/jammy-updates,now 1.0.2-1ubuntu3 amd64 [installed,automatic]
libnftnl11/jammy,now 1.2.1-1build1 amd64 [installed,automatic]
libnghttp2-14/jammy,now 1.43.0-1build3 amd64 [installed,automatic]
libnl-3-200/jammy,now 3.5.0-0.1 amd64 [installed,automatic]
libnl-genl-3-200/jammy,now 3.5.0-0.1 amd64 [installed,automatic]
libnl-route-3-200/jammy,now 3.5.0-0.1 amd64 [installed,automatic]
libnm0/jammy-updates,now 1.36.6-0ubuntu2 amd64 [installed,automatic]
libnma-common/jammy,jammy,now 1.8.34-1ubuntu1 all [installed,automatic]
libnma0/jammy,now 1.8.34-1ubuntu1 amd64 [installed,automatic]
libnotify-bin/jammy-updates,now 0.7.9-3ubuntu5.22.04.1 amd64 [installed,automatic]
libnotify4/jammy-updates,now 0.7.9-3ubuntu5.22.04.1 amd64 [installed,automatic]
libnpth0/jammy,now 1.6-3build2 amd64 [installed,automatic]
libnsl2/jammy,now 1.3.0-2build2 amd64 [installed,automatic]
libnspr4/jammy,now 2:4.32-3build1 amd64 [installed,automatic]
libnss-mdns/jammy,now 0.15.1-1ubuntu1 amd64 [installed,automatic]
libnss-systemd/jammy-updates,now 249.11-0ubuntu3.9 amd64 [installed,automatic]
libnss3/jammy-updates,jammy-security,now 2:3.68.2-0ubuntu1.2 amd64 [installed,automatic]
libntfs-3g89/jammy-updates,jammy-security,now 1:2021.8.22-3ubuntu1.2 amd64 [installed,automatic]
libnuma1/jammy,now 2.0.14-3ubuntu2 amd64 [installed,automatic]
libodfgen-0.1-1/jammy,now 0.1.8-2build2 amd64 [installed,automatic]
libogg0/jammy,now 1.3.5-0ubuntu3 amd64 [installed,automatic]
libopengl0/jammy,now 1.4.0-1 amd64 [installed,automatic]
libopenjp2-7/jammy,now 2.4.0-6 amd64 [installed,automatic]
libopus0/jammy,now 1.3.1-0.1build2 amd64 [installed,automatic]
liborc-0.4-0/jammy,now 1:0.4.32-2 amd64 [installed,automatic]
liborcus-0.17-0/jammy,now 0.17.2-2 amd64 [installed,automatic]
liborcus-parser-0.17-0/jammy,now 0.17.2-2 amd64 [installed,automatic]
libp11-kit0/jammy,now 0.24.0-6build1 amd64 [installed,automatic]
libpackagekit-glib2-18/jammy,now 1.2.5-2ubuntu2 amd64 [installed,automatic]
libpagemaker-0.0-0/jammy,now 0.0.4-1build3 amd64 [installed,automatic]
libpam-cap/jammy-updates,jammy-security,now 1:2.44-1ubuntu0.22.04.1 amd64 [installed,automatic]
libpam-fprintd/jammy-updates,now 1.94.2-1ubuntu0.22.04.1 amd64 [installed,automatic]
libpam-gnome-keyring/jammy-updates,now 40.0-3ubuntu3 amd64 [installed,automatic]
libpam-modules-bin/jammy-updates,jammy-security,now 1.4.0-11ubuntu2.3 amd64 [installed,automatic]
libpam-modules/jammy-updates,jammy-security,now 1.4.0-11ubuntu2.3 amd64 [installed,automatic]
libpam-pwquality/jammy,now 1.4.4-1build2 amd64 [installed,automatic]
libpam-runtime/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1.4.0-11ubuntu2.3 all [installed,automatic]
libpam-sss/jammy-updates,now 2.6.3-1ubuntu3.2 amd64 [installed,automatic]
libpam-systemd/jammy-updates,now 249.11-0ubuntu3.9 amd64 [installed,automatic]
libpam0g/jammy-updates,jammy-security,now 1.4.0-11ubuntu2.3 amd64 [installed,automatic]
libpango-1.0-0/jammy-updates,now 1.50.6+ds-2ubuntu1 amd64 [installed,automatic]
libpangocairo-1.0-0/jammy-updates,now 1.50.6+ds-2ubuntu1 amd64 [installed,automatic]
libpangoft2-1.0-0/jammy-updates,now 1.50.6+ds-2ubuntu1 amd64 [installed,automatic]
libpangomm-1.4-1v5/jammy,now 2.46.2-1 amd64 [installed,automatic]
libpangoxft-1.0-0/jammy-updates,now 1.50.6+ds-2ubuntu1 amd64 [installed,automatic]
libpaper-utils/jammy,now 1.1.28build2 amd64 [installed,automatic]
libpaper1/jammy,now 1.1.28build2 amd64 [installed,automatic]
libparted-fs-resize0/jammy,now 3.4-2build1 amd64 [installed,automatic]
libparted2/jammy,now 3.4-2build1 amd64 [installed,automatic]
libpcap0.8/jammy,now 1.10.1-4build1 amd64 [installed,automatic]
libpcaudio0/jammy,now 1.1-6build2 amd64 [installed,automatic]
libpci3/jammy,now 1:3.7.0-6 amd64 [installed,automatic]
libpciaccess0/jammy,now 0.16-3 amd64 [installed,automatic]
libpcre2-16-0/jammy-updates,jammy-security,now 10.39-3ubuntu0.1 amd64 [installed,automatic]
libpcre2-32-0/jammy-updates,jammy-security,now 10.39-3ubuntu0.1 amd64 [installed,automatic]
libpcre2-8-0/jammy-updates,jammy-security,now 10.39-3ubuntu0.1 amd64 [installed,automatic]
libpcre3/jammy-updates,jammy-security,now 2:8.39-13ubuntu0.22.04.1 amd64 [installed,automatic]
libpcsclite1/jammy,now 1.9.5-3 amd64 [installed,automatic]
libpeas-1.0-0/jammy,now 1.32.0-1 amd64 [installed,automatic]
libpeas-common/jammy,jammy,now 1.32.0-1 all [installed,automatic]
libperl5.34/jammy-updates,jammy-security,now 5.34.0-3ubuntu1.2 amd64 [installed,automatic]
libphonenumber8/jammy,now 8.12.44-1 amd64 [installed,automatic]
libpipeline1/jammy,now 1.5.5-1 amd64 [installed,automatic]
libpipewire-0.3-0/jammy-updates,now 0.3.48-1ubuntu3 amd64 [installed,automatic]
libpipewire-0.3-common/jammy-updates,jammy-updates,now 0.3.48-1ubuntu3 all [installed,automatic]
libpipewire-0.3-modules/jammy-updates,now 0.3.48-1ubuntu3 amd64 [installed,automatic]
libpixman-1-0/jammy-updates,jammy-security,now 0.40.0-1ubuntu0.22.04.1 amd64 [installed,automatic]
libpkcs11-helper1/jammy-updates,now 1.28-1ubuntu0.22.04.1 amd64 [installed,automatic]
libplist3/jammy,now 2.2.0-6build2 amd64 [installed,automatic]
libplymouth5/jammy,now 0.9.5+git20211018-1ubuntu3 amd64 [installed,automatic]
libpng16-16/jammy,now 1.6.37-3build5 amd64 [installed,automatic]
libpolkit-agent-1-0/jammy,now 0.105-33 amd64 [installed,automatic]
libpolkit-gobject-1-0/jammy,now 0.105-33 amd64 [installed,automatic]
libpolkit-qt5-1-1/jammy,now 0.114.0-2 amd64 [installed,automatic]
libpoppler-cpp0v5/jammy-updates,jammy-security,now 22.02.0-2ubuntu0.1 amd64 [installed,automatic]
libpoppler-glib8/jammy-updates,jammy-security,now 22.02.0-2ubuntu0.1 amd64 [installed,automatic]
libpoppler118/jammy-updates,jammy-security,now 22.02.0-2ubuntu0.1 amd64 [installed,automatic]
libpopt0/jammy,now 1.18-3build1 amd64 [installed,automatic]
libprocps8/jammy,now 2:3.3.17-6ubuntu2 amd64 [installed,automatic]
libprotobuf23/jammy-updates,jammy-security,now 3.12.4-1ubuntu7.22.04.1 amd64 [installed,automatic]
libproxy1-plugin-gsettings/jammy,now 0.4.17-2 amd64 [installed,automatic]
libproxy1-plugin-networkmanager/jammy,now 0.4.17-2 amd64 [installed,automatic]
libproxy1v5/jammy,now 0.4.17-2 amd64 [installed,automatic]
libpsl5/jammy,now 0.21.0-1.2build2 amd64 [installed,automatic]
libpulse-mainloop-glib0/jammy-updates,now 1:15.99.1+dfsg1-1ubuntu2.1 amd64 [installed,automatic]
libpulse0/jammy-updates,now 1:15.99.1+dfsg1-1ubuntu2.1 amd64 [installed,automatic]
libpulsedsp/jammy-updates,now 1:15.99.1+dfsg1-1ubuntu2.1 amd64 [installed,automatic]
libpwquality-common/jammy,jammy,now 1.4.4-1build2 all [installed,automatic]
libpwquality1/jammy,now 1.4.4-1build2 amd64 [installed,automatic]
libpython3-stdlib/jammy-updates,now 3.10.6-1~22.04 amd64 [installed,automatic]
libpython3.10-minimal/jammy-updates,jammy-security,now 3.10.6-1~22.04.2ubuntu1.1 amd64 [installed,automatic]
libpython3.10-stdlib/jammy-updates,jammy-security,now 3.10.6-1~22.04.2ubuntu1.1 amd64 [installed,automatic]
libpython3.10/jammy-updates,jammy-security,now 3.10.6-1~22.04.2ubuntu1.1 amd64 [installed,automatic]
libqmi-glib5/jammy-updates,now 1.32.0-1ubuntu0.22.04.1 amd64 [installed,automatic]
libqmi-proxy/jammy-updates,now 1.32.0-1ubuntu0.22.04.1 amd64 [installed,automatic]
libqpdf28/jammy,now 10.6.3-1 amd64 [installed,automatic]
libqqwing2v5/jammy,now 1.3.4-1.1ubuntu3 amd64 [installed,automatic]
libqt5core5a/jammy-updates,now 5.15.3+dfsg-2ubuntu0.2 amd64 [installed,automatic]
libqt5dbus5/jammy-updates,now 5.15.3+dfsg-2ubuntu0.2 amd64 [installed,automatic]
libqt5gui5/jammy-updates,now 5.15.3+dfsg-2ubuntu0.2 amd64 [installed,automatic]
libqt5network5/jammy-updates,now 5.15.3+dfsg-2ubuntu0.2 amd64 [installed,automatic]
libqt5positioning5/jammy,now 5.15.3+dfsg-3 amd64 [installed,automatic]
libqt5printsupport5/jammy-updates,now 5.15.3+dfsg-2ubuntu0.2 amd64 [installed,automatic]
libqt5qml5/jammy,now 5.15.3+dfsg-1 amd64 [installed,automatic]
libqt5qmlmodels5/jammy,now 5.15.3+dfsg-1 amd64 [installed,automatic]
libqt5qmlworkerscript5/jammy,now 5.15.3+dfsg-1 amd64 [installed,automatic]
libqt5quick5/jammy,now 5.15.3+dfsg-1 amd64 [installed,automatic]
libqt5quickwidgets5/jammy,now 5.15.3+dfsg-1 amd64 [installed,automatic]
libqt5sensors5/jammy,now 5.15.3-1 amd64 [installed,automatic]
libqt5svg5/jammy,now 5.15.3-1 amd64 [installed,automatic]
libqt5texttospeech5/jammy,now 5.15.3-1 amd64 [installed,automatic]
libqt5waylandclient5/jammy,now 5.15.3-1 amd64 [installed,automatic]
libqt5waylandcompositor5/jammy,now 5.15.3-1 amd64 [installed,automatic]
libqt5webchannel5/jammy,now 5.15.3-1 amd64 [installed,automatic]
libqt5webkit5/jammy,now 5.212.0~alpha4-15ubuntu1 amd64 [installed,automatic]
libqt5widgets5/jammy-updates,now 5.15.3+dfsg-2ubuntu0.2 amd64 [installed,automatic]
libqt5x11extras5/jammy,now 5.15.3-1 amd64 [installed,automatic]
libqt5xml5/jammy-updates,now 5.15.3+dfsg-2ubuntu0.2 amd64 [installed,automatic]
libraptor2-0/jammy,now 2.0.15-0ubuntu4 amd64 [installed,automatic]
libraqm0/jammy,now 0.7.0-4ubuntu1 amd64 [installed,automatic]
librasqal3/jammy,now 0.9.33-0.2ubuntu1 amd64 [installed,automatic]
libraw1394-11/jammy,now 2.1.2-2build2 amd64 [installed,automatic]
libraw20/jammy-updates,jammy-security,now 0.20.2-2ubuntu2.22.04.1 amd64 [installed,automatic]
librdf0/jammy,now 1.0.17-1.1ubuntu3 amd64 [installed,automatic]
libreadline8/jammy,now 8.1.2-1 amd64 [installed,automatic]
libreoffice-base-core/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libreoffice-calc/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libreoffice-common/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 all [installed,automatic]
libreoffice-core/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libreoffice-draw/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libreoffice-gnome/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libreoffice-gtk3/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libreoffice-help-common/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 all [installed]
libreoffice-help-en-us/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 all [installed]
libreoffice-impress/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libreoffice-math/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libreoffice-ogltrans/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 all [installed,automatic]
libreoffice-pdfimport/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 all [installed,automatic]
libreoffice-style-breeze/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 all [installed,automatic]
libreoffice-style-colibre/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 all [installed,automatic]
libreoffice-style-elementary/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 all [installed,automatic]
libreoffice-style-yaru/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 all [installed,automatic]
libreoffice-writer/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
librest-0.7-0/jammy,now 0.8.1-1.1build2 amd64 [installed,automatic]
librevenge-0.0-0/jammy,now 0.0.4-6ubuntu7 amd64 [installed,automatic]
librhythmbox-core10/jammy,now 3.4.4-5ubuntu1 amd64 [installed,automatic]
librsvg2-2/jammy,now 2.52.5+dfsg-3 amd64 [installed,automatic]
librsvg2-common/jammy,now 2.52.5+dfsg-3 amd64 [installed,automatic]
librsync2/jammy,now 2.3.2-1ubuntu1 amd64 [installed,automatic]
librtmp1/jammy,now 2.4+20151223.gitfa8646d.1-2build4 amd64 [installed,automatic]
librygel-core-2.6-2/jammy,now 0.40.3-1ubuntu2 amd64 [installed,automatic]
librygel-db-2.6-2/jammy,now 0.40.3-1ubuntu2 amd64 [installed,automatic]
librygel-renderer-2.6-2/jammy,now 0.40.3-1ubuntu2 amd64 [installed,automatic]
librygel-server-2.6-2/jammy,now 0.40.3-1ubuntu2 amd64 [installed,automatic]
libsamplerate0/jammy,now 0.2.2-1build1 amd64 [installed,automatic]
libsane-common/jammy,jammy,now 1.1.1-5 all [installed,automatic]
libsane-hpaio/jammy,now 3.21.12+dfsg0-1 amd64 [installed,automatic]
libsane1/jammy,now 1.1.1-5 amd64 [installed,automatic]
libsasl2-2/jammy-updates,now 2.1.27+dfsg2-3ubuntu1.2 amd64 [installed,automatic]
libsasl2-modules-db/jammy-updates,now 2.1.27+dfsg2-3ubuntu1.2 amd64 [installed,automatic]
libsasl2-modules-gssapi-mit/jammy-updates,now 2.1.27+dfsg2-3ubuntu1.2 amd64 [installed,automatic]
libsasl2-modules/jammy-updates,now 2.1.27+dfsg2-3ubuntu1.2 amd64 [installed,automatic]
libsbc1/jammy,now 1.5-3build2 amd64 [installed,automatic]
libseccomp2/jammy,now 2.5.3-2ubuntu2 amd64 [installed,automatic]
libsecret-1-0/jammy,now 0.20.5-2 amd64 [installed,automatic]
libsecret-common/jammy,jammy,now 0.20.5-2 all [installed,automatic]
libselinux1/jammy,now 3.3-1build2 amd64 [installed,automatic]
libsemanage-common/jammy,jammy,now 3.3-1build2 all [installed,automatic]
libsemanage2/jammy,now 3.3-1build2 amd64 [installed,automatic]
libsensors-config/jammy,jammy,now 1:3.6.0-7ubuntu1 all [installed,automatic]
libsensors5/jammy,now 1:3.6.0-7ubuntu1 amd64 [installed,automatic]
libsepol2/jammy,now 3.3-1build1 amd64 [installed,automatic]
libsgutils2-2/jammy,now 1.46-1build1 amd64 [installed,automatic]
libshout3/jammy,now 2.4.5-1build3 amd64 [installed,automatic]
libsigc++-2.0-0v5/jammy,now 2.10.4-2ubuntu3 amd64 [installed,automatic]
libslang2/jammy,now 2.3.2-5build4 amd64 [installed,automatic]
libsm6/jammy,now 2:1.2.3-1build2 amd64 [installed,automatic]
libsmartcols1/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
libsmbclient/jammy-updates,jammy-security,now 2:4.15.13+dfsg-0ubuntu1.2 amd64 [installed,automatic]
libsmbios-c2/jammy,now 2.4.3-1build1 amd64 [installed,automatic]
libsnapd-glib1/jammy,now 1.60-0ubuntu1 amd64 [installed,automatic]
libsndfile1/jammy,now 1.0.31-2build1 amd64 [installed,automatic]
libsnmp-base/jammy-updates,jammy-updates,now 5.9.1+dfsg-1ubuntu2.6 all [installed,automatic]
libsnmp40/jammy-updates,now 5.9.1+dfsg-1ubuntu2.6 amd64 [installed,automatic]
libsodium23/jammy,now 1.0.18-1build2 amd64 [installed,automatic]
libsonic0/jammy,now 0.2.0-11build1 amd64 [installed,automatic]
libsoup-gnome2.4-1/jammy,now 2.74.2-3 amd64 [installed,automatic]
libsoup2.4-1/jammy,now 2.74.2-3 amd64 [installed,automatic]
libsoup2.4-common/jammy,jammy,now 2.74.2-3 all [installed,automatic]
libsource-highlight-common/jammy,jammy,now 3.1.9-4.1build2 all [installed,automatic]
libsource-highlight4v5/jammy,now 3.1.9-4.1build2 amd64 [installed,automatic]
libsoxr0/jammy,now 0.1.3-4build2 amd64 [installed,automatic]
libspa-0.2-modules/jammy-updates,now 0.3.48-1ubuntu3 amd64 [installed,automatic]
libspectre1/jammy,now 0.2.10-1 amd64 [installed,automatic]
libspeechd2/now 0.11.1-1ubuntu2 amd64 [installed,upgradable to: 0.11.1-1ubuntu3]
libspeex1/jammy,now 1.2~rc1.2-1.1ubuntu3 amd64 [installed,automatic]
libspeexdsp1/jammy,now 1.2~rc1.2-1.1ubuntu3 amd64 [installed,automatic]
libsqlite3-0/jammy-updates,jammy-security,now 3.37.2-2ubuntu0.1 amd64 [installed,automatic]
libss2/jammy-updates,jammy-security,now 1.46.5-2ubuntu1.1 amd64 [installed,automatic]
libssh-4/jammy-updates,jammy-security,now 0.9.6-2ubuntu0.22.04.1 amd64 [installed,automatic]
libssl3/jammy-updates,jammy-security,now 3.0.2-0ubuntu1.10 amd64 [installed,automatic]
libstartup-notification0/jammy,now 0.12-6build2 amd64 [installed,automatic]
libstdc++6/jammy-updates,jammy-security,now 12.1.0-2ubuntu1~22.04 amd64 [installed,automatic]
libstemmer0d/jammy,now 2.2.0-1build1 amd64 [installed,automatic]
libsuitesparseconfig5/jammy,now 1:5.10.1+dfsg-4build1 amd64 [installed,automatic]
libsynctex2/jammy-updates,jammy-security,now 2021.20210626.59705-1ubuntu0.1 amd64 [installed,automatic]
libsysmetrics1/jammy,now 1.7.1 amd64 [installed,automatic]
libsystemd0/jammy-updates,now 249.11-0ubuntu3.9 amd64 [installed,automatic]
libtag1v5-vanilla/jammy,now 1.11.1+dfsg.1-3ubuntu3 amd64 [installed,automatic]
libtag1v5/jammy,now 1.11.1+dfsg.1-3ubuntu3 amd64 [installed,automatic]
libtalloc2/jammy,now 2.3.3-2build1 amd64 [installed,automatic]
libtasn1-6/jammy,now 4.18.0-4build1 amd64 [installed,automatic]
libtcl8.6/jammy,now 8.6.12+dfsg-1build1 amd64 [installed,automatic]
libtdb1/jammy,now 1.4.5-2build1 amd64 [installed,automatic]
libteamdctl0/jammy,now 1.31-1build2 amd64 [installed,automatic]
libtevent0/jammy,now 0.11.0-1build1 amd64 [installed,automatic]
libtext-charwidth-perl/jammy,now 0.04-10build3 amd64 [installed,automatic]
libtext-iconv-perl/jammy,now 1.7-7build3 amd64 [installed,automatic]
libtext-wrapi18n-perl/jammy,jammy,now 0.06-9 all [installed,automatic]
libthai-data/jammy,jammy,now 0.1.29-1build1 all [installed,automatic]
libthai0/jammy,now 0.1.29-1build1 amd64 [installed,automatic]
libtheora0/jammy,now 1.1.1+dfsg.1-15ubuntu4 amd64 [installed,automatic]
libtie-ixhash-perl/jammy,jammy,now 1.23-2.1 all [installed,automatic]
libtiff5/jammy-updates,jammy-security,now 4.3.0-6ubuntu0.4 amd64 [installed,automatic]
libtimedate-perl/jammy,jammy,now 2.3300-2 all [installed,automatic]
libtinfo6/jammy-updates,jammy-security,now 6.3-2ubuntu0.1 amd64 [installed,automatic]
libtirpc-common/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1.3.2-2ubuntu0.1 all [installed,automatic]
libtirpc3/jammy-updates,jammy-security,now 1.3.2-2ubuntu0.1 amd64 [installed,automatic]
libtotem-plparser-common/jammy,jammy,now 3.26.6-1build1 all [installed,automatic]
libtotem-plparser18/jammy,now 3.26.6-1build1 amd64 [installed,automatic]
libtotem0/jammy,now 42.0-1ubuntu1 amd64 [installed,automatic]
libtracker-sparql-3.0-0/jammy,now 3.3.0-1 amd64 [installed,automatic]
libtry-tiny-perl/jammy,jammy,now 0.31-1 all [installed,automatic]
libtss2-esys-3.0.2-0/jammy,now 3.2.0-1ubuntu1 amd64 [installed,automatic]
libtss2-mu0/jammy,now 3.2.0-1ubuntu1 amd64 [installed,automatic]
libtss2-sys1/jammy,now 3.2.0-1ubuntu1 amd64 [installed,automatic]
libtss2-tcti-cmd0/jammy,now 3.2.0-1ubuntu1 amd64 [installed,automatic]
libtss2-tcti-device0/jammy,now 3.2.0-1ubuntu1 amd64 [installed,automatic]
libtss2-tcti-mssim0/jammy,now 3.2.0-1ubuntu1 amd64 [installed,automatic]
libtss2-tcti-swtpm0/jammy,now 3.2.0-1ubuntu1 amd64 [installed,automatic]
libtwolame0/jammy,now 0.4.0-2build2 amd64 [installed,automatic]
libu2f-udev/jammy,jammy,now 1.1.10-3build2 all [installed,automatic]
libuchardet0/jammy,now 0.0.7-1build2 amd64 [installed,automatic]
libudev1/jammy-updates,now 249.11-0ubuntu3.9 amd64 [installed,automatic]
libudisks2-0/jammy,now 2.9.4-1ubuntu2 amd64 [installed,automatic]
libunistring2/jammy,now 1.0-1 amd64 [installed,automatic]
libunity-protocol-private0/jammy,now 7.1.4+19.04.20190319-6build1 amd64 [installed,automatic]
libunity-scopes-json-def-desktop/jammy,jammy,now 7.1.4+19.04.20190319-6build1 all [installed,automatic]
libunity9/jammy,now 7.1.4+19.04.20190319-6build1 amd64 [installed,automatic]
libuno-cppu3/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libuno-cppuhelpergcc3-3/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libuno-purpenvhelpergcc3-3/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libuno-sal3/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libuno-salhelpergcc3-3/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
libunwind8/jammy,now 1.3.2-2build2 amd64 [installed,automatic]
libupower-glib3/jammy,now 0.99.17-1 amd64 [installed,automatic]
liburi-perl/jammy,jammy,now 5.10-1 all [installed,automatic]
libusb-1.0-0/jammy-updates,now 2:1.0.25-1ubuntu2 amd64 [installed,automatic]
libusbmuxd6/jammy,now 2.0.2-3build2 amd64 [installed,automatic]
libuuid1/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
libuv1/jammy,now 1.43.0-1 amd64 [installed,automatic]
libv4l-0/jammy,now 1.22.1-2build1 amd64 [installed,automatic]
libv4lconvert0/jammy,now 1.22.1-2build1 amd64 [installed,automatic]
libvisio-0.1-1/jammy,now 0.1.7-1build5 amd64 [installed,automatic]
libvisual-0.4-0/jammy,now 0.4.0-17build2 amd64 [installed,automatic]
libvncclient1/jammy,now 0.9.13+dfsg-3build2 amd64 [installed,automatic]
libvncserver1/jammy,now 0.9.13+dfsg-3build2 amd64 [installed,automatic]
libvoikko1/jammy,now 4.3.1-1build1 amd64 [installed,automatic]
libvolume-key1/jammy,now 0.3.12-3.1build3 amd64 [installed,automatic]
libvorbis0a/jammy,now 1.3.7-1build2 amd64 [installed,automatic]
libvorbisenc2/jammy,now 1.3.7-1build2 amd64 [installed,automatic]
libvorbisfile3/jammy,now 1.3.7-1build2 amd64 [installed,automatic]
libvpx7/jammy,now 1.11.0-2ubuntu2 amd64 [installed,automatic]
libvte-2.91-0/jammy,now 0.68.0-1 amd64 [installed,automatic]
libvte-2.91-common/jammy,now 0.68.0-1 amd64 [installed,automatic]
libvulkan1/jammy,now 1.3.204.1-2 amd64 [installed,automatic]
libwacom-bin/jammy,now 2.2.0-1 amd64 [installed,automatic]
libwacom-common/jammy,jammy,now 2.2.0-1 all [installed,automatic]
libwacom9/jammy,now 2.2.0-1 amd64 [installed,automatic]
libwavpack1/jammy,now 5.4.0-1build2 amd64 [installed,automatic]
libwayland-client0/jammy-updates,jammy-security,now 1.20.0-1ubuntu0.1 amd64 [installed,automatic]
libwayland-cursor0/jammy-updates,jammy-security,now 1.20.0-1ubuntu0.1 amd64 [installed,automatic]
libwayland-egl1/jammy-updates,jammy-security,now 1.20.0-1ubuntu0.1 amd64 [installed,automatic]
libwayland-server0/jammy-updates,jammy-security,now 1.20.0-1ubuntu0.1 amd64 [installed,automatic]
libwbclient0/jammy-updates,jammy-security,now 2:4.15.13+dfsg-0ubuntu1.2 amd64 [installed,automatic]
libwebkit2gtk-4.0-37/jammy-updates,jammy-security,now 2.38.6-0ubuntu0.22.04.1 amd64 [installed,automatic]
libwebp7/jammy-updates,jammy-security,now 1.2.2-2ubuntu0.22.04.1 amd64 [installed,automatic]
libwebpdemux2/jammy-updates,jammy-security,now 1.2.2-2ubuntu0.22.04.1 amd64 [installed,automatic]
libwebpmux3/jammy-updates,jammy-security,now 1.2.2-2ubuntu0.22.04.1 amd64 [installed,automatic]
libwebrtc-audio-processing1/jammy,now 0.3.1-0ubuntu5 amd64 [installed,automatic]
libwhoopsie-preferences0/jammy,now 23 amd64 [installed,automatic]
libwhoopsie0/jammy,now 0.2.77 amd64 [installed,automatic]
libwinpr2-2/jammy-updates,jammy-security,now 2.6.1+dfsg1-3ubuntu2.3 amd64 [installed,automatic]
libwmf-0.2-7-gtk/jammy,now 0.2.12-5ubuntu1 amd64 [installed,automatic]
libwmf-0.2-7/jammy,now 0.2.12-5ubuntu1 amd64 [installed,automatic]
libwmf0.2-7-gtk/jammy,now 0.2.12-5ubuntu1 amd64 [installed,automatic]
libwmflite-0.2-7/jammy,now 0.2.12-5ubuntu1 amd64 [installed,automatic]
libwnck-3-0/jammy,now 40.1-1 amd64 [installed,automatic]
libwnck-3-common/jammy,jammy,now 40.1-1 all [installed,automatic]
libwoff1/jammy,now 1.0.2-1build4 amd64 [installed,automatic]
libwpd-0.10-10/jammy,now 0.10.3-2build1 amd64 [installed,automatic]
libwpg-0.3-3/jammy,now 0.3.3-1build3 amd64 [installed,automatic]
libwps-0.4-4/jammy,now 0.4.12-2build1 amd64 [installed,automatic]
libwrap0/jammy,now 7.6.q-31build2 amd64 [installed,automatic]
libwww-perl/jammy,jammy,now 6.61-1 all [installed,automatic]
libwww-robotrules-perl/jammy,jammy,now 6.02-1 all [installed,automatic]
libx11-6/jammy-updates,jammy-security,now 2:1.7.5-1ubuntu0.2 amd64 [installed,automatic]
libx11-data/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2:1.7.5-1ubuntu0.2 all [installed,automatic]
libx11-protocol-perl/jammy,jammy,now 0.56-7.1 all [installed,automatic]
libx11-xcb1/jammy-updates,jammy-security,now 2:1.7.5-1ubuntu0.2 amd64 [installed,automatic]
libxatracker2/jammy-updates,now 22.2.5-0ubuntu0.1~22.04.3 amd64 [installed,automatic]
libxau6/jammy,now 1:1.0.9-1build5 amd64 [installed,automatic]
libxaw7/jammy,now 2:1.0.14-1 amd64 [installed,automatic]
libxcb-dri2-0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-dri3-0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-glx0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-icccm4/jammy,now 0.4.1-1.1build2 amd64 [installed,automatic]
libxcb-image0/jammy,now 0.4.0-2 amd64 [installed,automatic]
libxcb-keysyms1/jammy,now 0.4.0-1build3 amd64 [installed,automatic]
libxcb-present0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-randr0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-render-util0/jammy,now 0.3.9-1build3 amd64 [installed,automatic]
libxcb-render0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-res0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-shape0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-shm0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-sync1/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-util1/jammy,now 0.4.0-1build2 amd64 [installed,automatic]
libxcb-xfixes0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-xinerama0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-xinput0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-xkb1/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb-xv0/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcb1/jammy,now 1.14-3ubuntu3 amd64 [installed,automatic]
libxcomposite1/jammy,now 1:0.4.5-1build2 amd64 [installed,automatic]
libxcursor1/jammy,now 1:1.2.0-2build4 amd64 [installed,automatic]
libxcvt0/jammy,now 0.1.1-3 amd64 [installed,automatic]
libxdamage1/jammy,now 1:1.1.5-2build2 amd64 [installed,automatic]
libxdmcp6/jammy,now 1:1.1.3-0ubuntu5 amd64 [installed,automatic]
libxext6/jammy,now 2:1.3.4-1build1 amd64 [installed,automatic]
libxfixes3/jammy,now 1:6.0.0-1 amd64 [installed,automatic]
libxfont2/jammy,now 1:2.0.5-1build1 amd64 [installed,automatic]
libxft2/jammy,now 2.3.4-1 amd64 [installed,automatic]
libxi6/jammy,now 2:1.8-1build1 amd64 [installed,automatic]
libxinerama1/jammy,now 2:1.1.4-3 amd64 [installed,automatic]
libxkbcommon-x11-0/jammy,now 1.4.0-1 amd64 [installed,automatic]
libxkbcommon0/jammy,now 1.4.0-1 amd64 [installed,automatic]
libxkbfile1/jammy,now 1:1.1.0-1build3 amd64 [installed,automatic]
libxkbregistry0/jammy,now 1.4.0-1 amd64 [installed,automatic]
libxklavier16/jammy,now 5.4-4build2 amd64 [installed,automatic]
libxml-parser-perl/jammy,now 2.46-3build1 amd64 [installed,automatic]
libxml-twig-perl/jammy,jammy,now 1:3.52-1 all [installed,automatic]
libxml-xpathengine-perl/jammy,jammy,now 0.14-1 all [installed,automatic]
libxml2/jammy-updates,jammy-security,now 2.9.13+dfsg-1ubuntu0.3 amd64 [installed,automatic]
libxmlb2/jammy,now 0.3.6-2build1 amd64 [installed,automatic]
libxmlsec1-nss/jammy,now 1.2.33-1build2 amd64 [installed,automatic]
libxmlsec1-openssl/jammy,now 1.2.33-1build2 amd64 [installed,automatic]
libxmlsec1/jammy,now 1.2.33-1build2 amd64 [installed,automatic]
libxmu6/jammy,now 2:1.1.3-3 amd64 [installed,automatic]
libxmuu1/jammy,now 2:1.1.3-3 amd64 [installed,automatic]
libxpm4/jammy-updates,jammy-security,now 1:3.5.12-1ubuntu0.22.04.1 amd64 [installed,automatic]
libxrandr2/jammy,now 2:1.5.2-1build1 amd64 [installed,automatic]
libxrender1/jammy,now 1:0.9.10-1build4 amd64 [installed,automatic]
libxres1/jammy,now 2:1.2.1-1 amd64 [installed,automatic]
libxshmfence1/jammy,now 1.3-1build4 amd64 [installed,automatic]
libxslt1.1/jammy-updates,jammy-security,now 1.1.34-4ubuntu0.22.04.1 amd64 [installed,automatic]
libxss1/jammy,now 1:1.2.3-1build2 amd64 [installed,automatic]
libxt6/jammy,now 1:1.2.1-1 amd64 [installed,automatic]
libxtables12/jammy-updates,now 1.8.7-1ubuntu5.1 amd64 [installed,automatic]
libxtst6/jammy,now 2:1.2.3-1build4 amd64 [installed,automatic]
libxv1/jammy,now 2:1.0.11-1build2 amd64 [installed,automatic]
libxvmc1/jammy,now 2:1.0.12-2build2 amd64 [installed,automatic]
libxxf86dga1/jammy,now 2:1.1.5-0ubuntu3 amd64 [installed,automatic]
libxxf86vm1/jammy,now 1:1.1.4-1build3 amd64 [installed,automatic]
libxxhash0/jammy,now 0.8.1-1 amd64 [installed,automatic]
libyajl2/jammy,now 2.1.0-3build2 amd64 [installed,automatic]
libyaml-0-2/jammy,now 0.2.2-1build2 amd64 [installed,automatic]
libyaml-cpp0.7/jammy,now 0.7.0+dfsg-8build1 amd64 [installed,automatic]
libyelp0/jammy,now 42.1-1 amd64 [installed,automatic]
libzstd1/jammy,now 1.4.8+dfsg-3build1 amd64 [installed,automatic]
linux-base/jammy,jammy,now 4.5ubuntu9 all [installed,automatic]
linux-firmware/jammy-updates,jammy-updates,jammy-security,jammy-security,now 20220329.git681281e4-0ubuntu3.14 all [installed,automatic]
linux-generic-hwe-22.04/jammy-updates,jammy-security,now 5.19.0.46.47~22.04.21 amd64 [installed]
linux-headers-5.19.0-32-generic/now 5.19.0-32.33~22.04.1 amd64 [installed,local]
linux-headers-5.19.0-46-generic/jammy-updates,jammy-security,now 5.19.0-46.47~22.04.1 amd64 [installed,automatic]
linux-headers-generic-hwe-22.04/jammy-updates,jammy-security,now 5.19.0.46.47~22.04.21 amd64 [installed,automatic]
linux-hwe-5.19-headers-5.19.0-32/now 5.19.0-32.33~22.04.1 all [installed,local]
linux-hwe-5.19-headers-5.19.0-46/jammy-updates,jammy-updates,jammy-security,jammy-security,now 5.19.0-46.47~22.04.1 all [installed,automatic]
linux-image-5.19.0-32-generic/now 5.19.0-32.33~22.04.1 amd64 [installed,local]
linux-image-5.19.0-46-generic/jammy-updates,jammy-security,now 5.19.0-46.47~22.04.1 amd64 [installed,automatic]
linux-image-generic-hwe-22.04/jammy-updates,jammy-security,now 5.19.0.46.47~22.04.21 amd64 [installed,automatic]
linux-modules-5.19.0-32-generic/now 5.19.0-32.33~22.04.1 amd64 [installed,local]
linux-modules-5.19.0-46-generic/jammy-updates,jammy-security,now 5.19.0-46.47~22.04.1 amd64 [installed,automatic]
linux-modules-extra-5.19.0-32-generic/now 5.19.0-32.33~22.04.1 amd64 [installed,local]
linux-modules-extra-5.19.0-46-generic/jammy-updates,jammy-security,now 5.19.0-46.47~22.04.1 amd64 [installed,automatic]
linux-sound-base/jammy,jammy,now 1.0.25+dfsg-0ubuntu7 all [installed,automatic]
locales/jammy-updates,jammy-updates,now 2.35-0ubuntu3.1 all [installed,automatic]
login/jammy-updates,jammy-security,now 1:4.8.1-2ubuntu2.1 amd64 [installed]
logrotate/jammy-updates,jammy-security,now 3.19.0-1ubuntu1.1 amd64 [installed,automatic]
logsave/jammy-updates,jammy-security,now 1.46.5-2ubuntu1.1 amd64 [installed,automatic]
lp-solve/jammy,now 5.5.2.5-2build2 amd64 [installed,automatic]
lsb-base/jammy,jammy,now 11.1.0ubuntu4 all [installed,automatic]
lsb-release/jammy,jammy,now 11.1.0ubuntu4 all [installed,automatic]
lshw/jammy,now 02.19.git.2021.06.19.996aaad9c7-2build1 amd64 [installed,automatic]
lsof/jammy,now 4.93.2+dfsg-1.1build2 amd64 [installed,automatic]
mailcap/jammy,jammy,now 3.70+nmu1ubuntu1 all [installed,automatic]
man-db/jammy,now 2.10.2-1 amd64 [installed,automatic]
manpages/jammy,jammy,now 5.10-1ubuntu1 all [installed,automatic]
mawk/jammy,now 1.3.4.20200120-3 amd64 [installed,automatic]
media-player-info/jammy,jammy,now 24-2 all [installed,automatic]
media-types/jammy,jammy,now 7.0.0 all [installed,automatic]
memtest86+/jammy,now 5.31b+dfsg-4 amd64 [installed,automatic]
mesa-vulkan-drivers/jammy-updates,now 22.2.5-0ubuntu0.1~22.04.3 amd64 [installed,automatic]
mime-support/jammy,jammy,now 3.66 all [installed,automatic]
mobile-broadband-provider-info/jammy,jammy,now 20220315-1 all [installed,automatic]
modemmanager/jammy-updates,now 1.20.0-1~ubuntu22.04.2 amd64 [installed,automatic]
mokutil/jammy-updates,now 0.6.0-2~22.04.1 amd64 [installed]
mount/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
mousetweaks/jammy,now 3.32.0-3build2 amd64 [installed,automatic]
mscompress/jammy,now 0.4-9build1 amd64 [installed,automatic]
mtr-tiny/jammy,now 0.95-1 amd64 [installed,automatic]
mutter-common/now 42.5-0ubuntu1 all [installed,upgradable to: 42.9-0ubuntu1]
mythes-en-us/jammy,jammy,now 1:7.2.0-2 all [installed]
nano/jammy,now 6.2-1 amd64 [installed,automatic]
nautilus-data/jammy-updates,jammy-updates,now 1:42.6-0ubuntu1 all [installed,automatic]
nautilus-extension-gnome-terminal/jammy,now 3.44.0-1ubuntu1 amd64 [installed,automatic]
nautilus-sendto/jammy,now 3.8.6-4 amd64 [installed,automatic]
nautilus-share/jammy,now 0.7.3-2ubuntu6 amd64 [installed,automatic]
nautilus/jammy-updates,now 1:42.6-0ubuntu1 amd64 [installed,automatic]
ncurses-base/jammy-updates,jammy-updates,jammy-security,jammy-security,now 6.3-2ubuntu0.1 all [installed]
ncurses-bin/jammy-updates,jammy-security,now 6.3-2ubuntu0.1 amd64 [installed]
netbase/jammy,jammy,now 6.3 all [installed,automatic]
netcat-openbsd/jammy,now 1.218-4ubuntu1 amd64 [installed,automatic]
netplan.io/jammy-updates,now 0.105-0ubuntu2~22.04.3 amd64 [installed,automatic]
network-manager-config-connectivity-ubuntu/jammy-updates,jammy-updates,now 1.36.6-0ubuntu2 all [installed,automatic]
network-manager-gnome/jammy,now 1.24.0-1ubuntu3 amd64 [installed,automatic]
network-manager-openvpn-gnome/jammy,now 1.8.18-1 amd64 [installed,automatic]
network-manager-openvpn/jammy,now 1.8.18-1 amd64 [installed,automatic]
network-manager-pptp-gnome/jammy,now 1.2.10-1 amd64 [installed,automatic]
network-manager-pptp/jammy,now 1.2.10-1 amd64 [installed,automatic]
network-manager/jammy-updates,now 1.36.6-0ubuntu2 amd64 [installed,automatic]
networkd-dispatcher/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2.1-2ubuntu0.22.04.2 all [installed,automatic]
nftables/jammy-updates,now 1.0.2-1ubuntu3 amd64 [installed,automatic]
ntfs-3g/jammy-updates,jammy-security,now 1:2021.8.22-3ubuntu1.2 amd64 [installed,automatic]
open-vm-tools-desktop/jammy-updates,now 2:12.1.5-3~ubuntu0.22.04.1 amd64 [installed]
open-vm-tools/jammy-updates,now 2:12.1.5-3~ubuntu0.22.04.1 amd64 [installed,automatic]
openprinting-ppds/jammy,jammy,now 20220223-0ubuntu1 all [installed,automatic]
openssh-client/jammy-updates,now 1:8.9p1-3ubuntu0.1 amd64 [installed,automatic]
openssl/jammy-updates,jammy-security,now 3.0.2-0ubuntu1.10 amd64 [installed,automatic]
openvpn/jammy-updates,now 2.5.5-1ubuntu3.1 amd64 [installed,automatic]
orca/jammy-updates,jammy-updates,jammy-security,jammy-security,now 42.0-1ubuntu2 all [installed,automatic]
os-prober/jammy,now 1.79ubuntu2 amd64 [installed]
p11-kit-modules/jammy,now 0.24.0-6build1 amd64 [installed,automatic]
p11-kit/jammy,now 0.24.0-6build1 amd64 [installed,automatic]
packagekit-tools/jammy,now 1.2.5-2ubuntu2 amd64 [installed,automatic]
packagekit/jammy,now 1.2.5-2ubuntu2 amd64 [installed,automatic]
parted/jammy,now 3.4-2build1 amd64 [installed,automatic]
passwd/jammy-updates,jammy-security,now 1:4.8.1-2ubuntu2.1 amd64 [installed,automatic]
patch/jammy,now 2.7.6-7build2 amd64 [installed,automatic]
pci.ids/jammy,jammy,now 0.0~2022.01.22-1 all [installed,automatic]
pciutils/jammy,now 1:3.7.0-6 amd64 [installed,automatic]
pcmciautils/jammy,now 018-13build1 amd64 [installed,automatic]
perl-base/jammy-updates,jammy-security,now 5.34.0-3ubuntu1.2 amd64 [installed,automatic]
perl-modules-5.34/jammy-updates,jammy-updates,jammy-security,jammy-security,now 5.34.0-3ubuntu1.2 all [installed,automatic]
perl-openssl-defaults/jammy,now 5build2 amd64 [installed,automatic]
perl/jammy-updates,jammy-security,now 5.34.0-3ubuntu1.2 amd64 [installed,automatic]
pinentry-curses/jammy,now 1.1.1-1build2 amd64 [installed,automatic]
pinentry-gnome3/jammy,now 1.1.1-1build2 amd64 [installed,automatic]
pipewire-bin/jammy-updates,now 0.3.48-1ubuntu3 amd64 [installed,automatic]
pipewire-media-session/jammy,now 0.4.1-2ubuntu1 amd64 [installed,automatic]
pipewire/jammy-updates,now 0.3.48-1ubuntu3 amd64 [installed,automatic]
pkexec/jammy,now 0.105-33 amd64 [installed,automatic]
plymouth-label/jammy,now 0.9.5+git20211018-1ubuntu3 amd64 [installed,automatic]
plymouth-theme-spinner/jammy,now 0.9.5+git20211018-1ubuntu3 amd64 [installed,automatic]
plymouth-theme-ubuntu-text/jammy,now 0.9.5+git20211018-1ubuntu3 amd64 [installed,automatic]
plymouth/jammy,now 0.9.5+git20211018-1ubuntu3 amd64 [installed,automatic]
policykit-1/jammy,now 0.105-33 amd64 [installed,automatic]
policykit-desktop-privileges/jammy,jammy,now 0.21 all [installed,automatic]
polkitd/jammy,now 0.105-33 amd64 [installed,automatic]
poppler-data/jammy,jammy,now 0.4.11-1 all [installed,automatic]
poppler-utils/jammy-updates,jammy-security,now 22.02.0-2ubuntu0.1 amd64 [installed,automatic]
power-profiles-daemon/jammy,now 0.10.1-3 amd64 [installed,automatic]
powermgmt-base/jammy,jammy,now 1.36 all [installed,automatic]
ppp/jammy,now 2.4.9-1+1ubuntu3 amd64 [installed,automatic]
pptp-linux/jammy,now 1.10.0-1build3 amd64 [installed,automatic]
printer-driver-brlaser/jammy,now 6-3 amd64 [installed,automatic]
printer-driver-c2esp/jammy,now 27-11build1 amd64 [installed,automatic]
printer-driver-foo2zjs-common/jammy-updates,jammy-updates,jammy-security,jammy-security,now 20200505dfsg0-2ubuntu2.22.04.1 all [installed,automatic]
printer-driver-foo2zjs/jammy-updates,jammy-security,now 20200505dfsg0-2ubuntu2.22.04.1 amd64 [installed,automatic]
printer-driver-hpcups/jammy,now 3.21.12+dfsg0-1 amd64 [installed,automatic]
printer-driver-m2300w/jammy,now 0.51-15build1 amd64 [installed,automatic]
printer-driver-min12xxw/jammy,now 0.0.9-11build2 amd64 [installed,automatic]
printer-driver-pnm2ppa/jammy,now 1.13+nondbs-0ubuntu9 amd64 [installed,automatic]
printer-driver-postscript-hp/jammy,now 3.21.12+dfsg0-1 amd64 [installed,automatic]
printer-driver-ptouch/jammy,now 1.6-2build1 amd64 [installed,automatic]
printer-driver-pxljr/jammy,now 1.4+repack0-6build1 amd64 [installed,automatic]
printer-driver-sag-gdi/jammy,jammy,now 0.1-8 all [installed,automatic]
printer-driver-splix/jammy-updates,jammy-security,now 2.0.0+svn315-7fakesync1ubuntu0.22.04.1 amd64 [installed,automatic]
procps/jammy,now 2:3.3.17-6ubuntu2 amd64 [installed,automatic]
psmisc/jammy,now 23.4-2build3 amd64 [installed,automatic]
publicsuffix/jammy,jammy,now 20211207.1025-1 all [installed,automatic]
pulseaudio-module-bluetooth/jammy-updates,now 1:15.99.1+dfsg1-1ubuntu2.1 amd64 [installed,automatic]
pulseaudio-utils/jammy-updates,now 1:15.99.1+dfsg1-1ubuntu2.1 amd64 [installed,automatic]
pulseaudio/jammy-updates,now 1:15.99.1+dfsg1-1ubuntu2.1 amd64 [installed,automatic]
python-apt-common/jammy-updates,jammy-updates,now 2.4.0ubuntu1 all [installed,automatic]
python3-apport/jammy-updates,jammy-updates,now 2.20.11-0ubuntu82.5 all [installed,automatic]
python3-apt/jammy-updates,now 2.4.0ubuntu1 amd64 [installed,automatic]
python3-aptdaemon.gtk3widgets/jammy,jammy,now 1.1.1+bzr982-0ubuntu39 all [installed,automatic]
python3-aptdaemon/jammy,jammy,now 1.1.1+bzr982-0ubuntu39 all [installed,automatic]
python3-bcrypt/jammy,now 3.2.0-1build1 amd64 [installed,automatic]
python3-blinker/jammy,jammy,now 1.4+dfsg1-0.4 all [installed,automatic]
python3-brlapi/jammy-updates,now 6.4-4ubuntu3 amd64 [installed,automatic]
python3-cairo/jammy,now 1.20.1-3build1 amd64 [installed,automatic]
python3-certifi/jammy,jammy,now 2020.6.20-1 all [installed,automatic]
python3-cffi-backend/jammy,now 1.15.0-1build2 amd64 [installed,automatic]
python3-chardet/jammy,jammy,now 4.0.0-1 all [installed,automatic]
python3-click/jammy,jammy,now 8.0.3-1 all [installed,automatic]
python3-colorama/jammy,jammy,now 0.4.4-1 all [installed,automatic]
python3-commandnotfound/jammy,jammy,now 22.04.0 all [installed,automatic]
python3-cryptography/jammy,now 3.4.8-1ubuntu2 amd64 [installed,automatic]
python3-cups/jammy,now 2.0.1-5build1 amd64 [installed,automatic]
python3-cupshelpers/jammy,jammy,now 1.5.16-0ubuntu3 all [installed,automatic]
python3-dateutil/jammy,jammy,now 2.8.1-6 all [installed,automatic]
python3-dbus/jammy,now 1.2.18-3build1 amd64 [installed,automatic]
python3-debconf/jammy,jammy,now 1.5.79ubuntu1 all [installed,automatic]
python3-debian/jammy,jammy,now 0.1.43ubuntu1 all [installed,upgradable to: 0.1.43ubuntu1.1]
python3-defer/jammy,jammy,now 1.0.6-2.1ubuntu1 all [installed,automatic]
python3-distro-info/jammy,jammy,now 1.1build1 all [installed,automatic]
python3-distro/jammy,jammy,now 1.7.0-1 all [installed,automatic]
python3-distupgrade/jammy-updates,jammy-updates,now 1:22.04.16 all [installed,automatic]
python3-fasteners/jammy,jammy,now 0.14.1-2 all [installed,automatic]
python3-future/jammy-updates,jammy-updates,jammy-security,jammy-security,now 0.18.2-5ubuntu0.1 all [installed,automatic]
python3-gdbm/jammy-updates,now 3.10.6-1~22.04 amd64 [installed,automatic]
python3-gi-cairo/jammy-updates,now 3.42.1-0ubuntu1 amd64 [installed,automatic]
python3-gi/jammy-updates,now 3.42.1-0ubuntu1 amd64 [installed,automatic]
python3-httplib2/jammy,jammy,now 0.20.2-2 all [installed,automatic]
python3-ibus-1.0/jammy,jammy,now 1.5.26-4 all [installed,automatic]
python3-idna/jammy,jammy,now 3.3-1 all [installed,automatic]
python3-importlib-metadata/jammy,jammy,now 4.6.4-1 all [installed,automatic]
python3-jeepney/jammy,jammy,now 0.7.1-3 all [installed,automatic]
python3-jwt/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2.3.0-1ubuntu0.2 all [installed,automatic]
python3-keyring/jammy,jammy,now 23.5.0-1 all [installed,automatic]
python3-launchpadlib/jammy,jammy,now 1.10.16-1 all [installed,automatic]
python3-lazr.restfulclient/jammy,jammy,now 0.14.4-1 all [installed,automatic]
python3-lazr.uri/jammy,jammy,now 1.0.6-2 all [installed,automatic]
python3-ldb/jammy-updates,jammy-security,now 2:2.4.4-0ubuntu0.22.04.2 amd64 [installed,automatic]
python3-lib2to3/jammy-updates,jammy-updates,now 3.10.6-1~22.04 all [installed,automatic]
python3-lockfile/jammy,jammy,now 1:0.12.2-2.2 all [installed,automatic]
python3-louis/jammy-updates,jammy-updates,jammy-security,jammy-security,now 3.20.0-2ubuntu0.2 all [installed,automatic]
python3-macaroonbakery/jammy-updates,jammy-updates,now 1.3.1-2ubuntu0.1 all [installed,automatic]
python3-mako/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1.1.3+ds1-2ubuntu0.1 all [installed,automatic]
python3-markupsafe/jammy,now 2.0.1-2build1 amd64 [installed,automatic]
python3-minimal/jammy-updates,now 3.10.6-1~22.04 amd64 [installed,automatic]
python3-monotonic/jammy,jammy,now 1.6-2 all [installed,automatic]
python3-more-itertools/jammy,jammy,now 8.10.0-2 all [installed,automatic]
python3-nacl/jammy,now 1.5.0-2 amd64 [installed,automatic]
python3-netifaces/jammy,now 0.11.0-1build2 amd64 [installed,automatic]
python3-oauthlib/jammy-updates,jammy-updates,jammy-security,jammy-security,now 3.2.0-1ubuntu0.1 all [installed,automatic]
python3-olefile/jammy,jammy,now 0.46-3 all [installed,automatic]
python3-paramiko/jammy,jammy,now 2.9.3-0ubuntu1 all [installed,automatic]
python3-pexpect/jammy,jammy,now 4.8.0-2ubuntu1 all [installed,automatic]
python3-pil/jammy-updates,jammy-security,now 9.0.1-1ubuntu0.1 amd64 [installed,automatic]
python3-pkg-resources/jammy-updates,jammy-updates,jammy-security,jammy-security,now 59.6.0-1.2ubuntu0.22.04.1 all [installed,automatic]
python3-problem-report/jammy-updates,jammy-updates,now 2.20.11-0ubuntu82.5 all [installed,automatic]
python3-protobuf/jammy-updates,jammy-security,now 3.12.4-1ubuntu7.22.04.1 amd64 [installed,automatic]
python3-ptyprocess/jammy,jammy,now 0.7.0-3 all [installed,automatic]
python3-pyatspi/jammy,jammy,now 2.38.2-1 all [installed,automatic]
python3-pymacaroons/jammy,jammy,now 0.13.0-4 all [installed,automatic]
python3-pyparsing/jammy,jammy,now 2.4.7-1 all [installed,automatic]
python3-renderpm/jammy-updates,jammy-security,now 3.6.8-1ubuntu0.1 amd64 [installed,automatic]
python3-reportlab-accel/jammy-updates,jammy-security,now 3.6.8-1ubuntu0.1 amd64 [installed,automatic]
python3-reportlab/jammy-updates,jammy-updates,jammy-security,jammy-security,now 3.6.8-1ubuntu0.1 all [installed,automatic]
python3-requests/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2.25.1+dfsg-2ubuntu0.1 all [installed,automatic]
python3-rfc3339/jammy,jammy,now 1.1-3 all [installed,automatic]
python3-secretstorage/jammy,jammy,now 3.3.1-1 all [installed,automatic]
python3-six/jammy,jammy,now 1.16.0-3ubuntu1 all [installed,automatic]
python3-software-properties/jammy-updates,jammy-updates,now 0.99.22.7 all [installed,automatic]
python3-speechd/now 0.11.1-1ubuntu2 all [installed,upgradable to: 0.11.1-1ubuntu3]
python3-systemd/jammy,now 234-3ubuntu2 amd64 [installed,automatic]
python3-talloc/jammy,now 2.3.3-2build1 amd64 [installed,automatic]
python3-tz/jammy-updates,jammy-updates,now 2022.1-1ubuntu0.22.04.1 all [installed,automatic]
python3-uno/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
python3-update-manager/jammy-updates,jammy-updates,now 1:22.04.10 all [installed,automatic]
python3-urllib3/jammy,jammy,now 1.26.5-1~exp1 all [installed,automatic]
python3-wadllib/jammy,jammy,now 1.3.6-1 all [installed,automatic]
python3-xdg/jammy,jammy,now 0.27-2 all [installed,automatic]
python3-xkit/jammy,jammy,now 0.5.0ubuntu5 all [installed,automatic]
python3-yaml/jammy,now 5.4.1-1ubuntu1 amd64 [installed,automatic]
python3-zipp/jammy,jammy,now 1.0.0-3 all [installed,automatic]
python3.10-minimal/jammy-updates,jammy-security,now 3.10.6-1~22.04.2ubuntu1.1 amd64 [installed,automatic]
python3.10/jammy-updates,jammy-security,now 3.10.6-1~22.04.2ubuntu1.1 amd64 [installed,automatic]
python3/jammy-updates,now 3.10.6-1~22.04 amd64 [installed,automatic]
qml-module-qtquick-window2/jammy,now 5.15.3+dfsg-1 amd64 [installed,automatic]
qml-module-qtquick2/jammy,now 5.15.3+dfsg-1 amd64 [installed,automatic]
qt5-gtk-platformtheme/jammy-updates,now 5.15.3+dfsg-2ubuntu0.2 amd64 [installed,automatic]
qtspeech5-speechd-plugin/jammy,now 5.15.3-1 amd64 [installed,automatic]
qttranslations5-l10n/jammy,jammy,now 5.15.3-1 all [installed,automatic]
qtwayland5/jammy,now 5.15.3-1 amd64 [installed,automatic]
readline-common/jammy,jammy,now 8.1.2-1 all [installed,automatic]
remmina-common/jammy,jammy,now 1.4.25+dfsg-1 all [installed,automatic]
remmina-plugin-rdp/jammy,now 1.4.25+dfsg-1 amd64 [installed,automatic]
remmina-plugin-secret/jammy,now 1.4.25+dfsg-1 amd64 [installed,automatic]
remmina-plugin-vnc/jammy,now 1.4.25+dfsg-1 amd64 [installed,automatic]
remmina/jammy,now 1.4.25+dfsg-1 amd64 [installed,automatic]
rfkill/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
rhythmbox-data/jammy,jammy,now 3.4.4-5ubuntu1 all [installed,automatic]
rhythmbox-plugin-alternative-toolbar/jammy,jammy,now 0.20.2-1 all [installed,automatic]
rhythmbox-plugins/jammy,now 3.4.4-5ubuntu1 amd64 [installed,automatic]
rhythmbox/jammy,now 3.4.4-5ubuntu1 amd64 [installed,automatic]
rsync/jammy-updates,jammy-security,now 3.2.7-0ubuntu0.22.04.2 amd64 [installed,automatic]
rsyslog/jammy-updates,jammy-security,now 8.2112.0-2ubuntu2.2 amd64 [installed,automatic]
rtkit/jammy,now 0.13-4build2 amd64 [installed,automatic]
rygel/jammy,now 0.40.3-1ubuntu2 amd64 [installed,automatic]
samba-libs/jammy-updates,jammy-security,now 2:4.15.13+dfsg-0ubuntu1.2 amd64 [installed,automatic]
sane-airscan/jammy,now 0.99.27-1build1 amd64 [installed,automatic]
sane-utils/jammy,now 1.1.1-5 amd64 [installed,automatic]
sbsigntool/jammy,now 0.9.4-2ubuntu2 amd64 [installed,automatic]
seahorse/jammy,now 41.0-2 amd64 [installed,automatic]
secureboot-db/jammy,now 1.8 amd64 [installed,automatic]
sed/jammy,now 4.8-1ubuntu2 amd64 [installed,automatic]
sensible-utils/jammy,jammy,now 0.0.17 all [installed,automatic]
session-migration/jammy,now 0.3.6 amd64 [installed,automatic]
sgml-base/jammy,jammy,now 1.30 all [installed,automatic]
sgml-data/jammy,jammy,now 2.0.11+nmu1 all [installed,automatic]
shared-mime-info/jammy,now 2.1-2 amd64 [installed,automatic]
shim-signed/jammy-updates,now 1.51.3+15.7-0ubuntu1 amd64 [installed]
shotwell-common/jammy-updates,jammy-updates,now 0.30.14-1ubuntu6 all [installed,automatic]
shotwell/jammy-updates,now 0.30.14-1ubuntu6 amd64 [installed,automatic]
simple-scan/jammy,now 42.0-1 amd64 [installed,automatic]
snapd/jammy-updates,jammy-security,now 2.58+22.04.1 amd64 [installed,automatic]
software-properties-common/jammy-updates,jammy-updates,now 0.99.22.7 all [installed,automatic]
software-properties-gtk/jammy-updates,jammy-updates,now 0.99.22.7 all [installed,automatic]
sonnet-plugins/jammy,now 5.92.0-0ubuntu1 amd64 [installed,automatic]
sound-icons/jammy,jammy,now 0.1-8 all [installed,automatic]
sound-theme-freedesktop/jammy,jammy,now 0.8-2ubuntu1 all [installed,automatic]
speech-dispatcher-audio-plugins/now 0.11.1-1ubuntu2 amd64 [installed,upgradable to: 0.11.1-1ubuntu3]
speech-dispatcher-espeak-ng/now 0.11.1-1ubuntu2 amd64 [installed,upgradable to: 0.11.1-1ubuntu3]
speech-dispatcher/now 0.11.1-1ubuntu2 amd64 [installed,upgradable to: 0.11.1-1ubuntu3]
spice-vdagent/jammy,now 0.22.1-1 amd64 [installed,automatic]
squashfs-tools/jammy,now 1:4.5-3build1 amd64 [installed,automatic]
ssl-cert/jammy,jammy,now 1.1.2 all [installed,automatic]
strace/jammy,now 5.16-0ubuntu3 amd64 [installed,automatic]
sudo/jammy-updates,jammy-security,now 1.9.9-1ubuntu2.4 amd64 [installed,automatic]
switcheroo-control/jammy,now 2.4-3build2 amd64 [installed,automatic]
system-config-printer-common/jammy,jammy,now 1.5.16-0ubuntu3 all [installed,automatic]
system-config-printer-udev/jammy,now 1.5.16-0ubuntu3 amd64 [installed,automatic]
system-config-printer/jammy,jammy,now 1.5.16-0ubuntu3 all [installed,automatic]
systemd-hwe-hwdb/jammy-updates,jammy-updates,now 249.11.3 all [installed,automatic]
systemd-oomd/jammy-updates,now 249.11-0ubuntu3.9 amd64 [installed,automatic]
systemd-sysv/jammy-updates,now 249.11-0ubuntu3.9 amd64 [installed,automatic]
systemd-timesyncd/jammy-updates,now 249.11-0ubuntu3.9 amd64 [installed,automatic]
systemd/jammy-updates,now 249.11-0ubuntu3.9 amd64 [installed,automatic]
sysvinit-utils/jammy,now 3.01-1ubuntu1 amd64 [installed,automatic]
tar/jammy-updates,jammy-security,now 1.34+dfsg-1ubuntu0.1.22.04.1 amd64 [installed,automatic]
tcl8.6/jammy,now 8.6.12+dfsg-1build1 amd64 [installed,automatic]
tcl/jammy,now 8.6.11+1build2 amd64 [installed,automatic]
tcpdump/jammy-updates,now 4.99.1-3ubuntu0.1 amd64 [installed,automatic]
telnet/jammy,now 0.17-44build1 amd64 [installed,automatic]
thermald/jammy-updates,now 2.4.9-1ubuntu0.2 amd64 [installed,automatic]
thunderbird-gnome-support/jammy-updates,jammy-security,now 1:102.13.0+build1-0ubuntu0.22.04.1 amd64 [installed,automatic]
thunderbird-locale-en-us/jammy-updates,jammy-updates,jammy-security,jammy-security,now 1:102.13.0+build1-0ubuntu0.22.04.1 all [installed]
thunderbird-locale-en/jammy-updates,jammy-security,now 1:102.13.0+build1-0ubuntu0.22.04.1 amd64 [installed]
thunderbird/jammy-updates,jammy-security,now 1:102.13.0+build1-0ubuntu0.22.04.1 amd64 [installed,automatic]
time/jammy,now 1.9-0.1build2 amd64 [installed,automatic]
tnftp/jammy,now 20210827-4build1 amd64 [installed,automatic]
totem-common/jammy,jammy,now 42.0-1ubuntu1 all [installed,automatic]
totem-plugins/jammy,now 42.0-1ubuntu1 amd64 [installed,automatic]
totem/jammy,now 42.0-1ubuntu1 amd64 [installed,automatic]
tpm-udev/jammy,jammy,now 0.6 all [installed,automatic]
tracker-extract/jammy,now 3.3.0-1 amd64 [installed,automatic]
tracker-miner-fs/jammy,now 3.3.0-1 amd64 [installed,automatic]
tracker/jammy,now 3.3.0-1 amd64 [installed,automatic]
transmission-common/jammy,jammy,now 3.00-2ubuntu2 all [installed,automatic]
transmission-gtk/jammy,now 3.00-2ubuntu2 amd64 [installed,automatic]
tzdata/jammy-updates,jammy-updates,now 2023c-0ubuntu0.22.04.2 all [installed,automatic]
ubuntu-advantage-desktop-daemon/jammy-updates,now 1.10~22.04.1 amd64 [installed,automatic]
ubuntu-advantage-tools/now 27.14.4~22.04 amd64 [installed,upgradable to: 28.1~22.04]
ubuntu-desktop-minimal/jammy,now 1.481 amd64 [installed,upgradable to: 1.481.1]
ubuntu-desktop/jammy,now 1.481 amd64 [installed,upgradable to: 1.481.1]
ubuntu-docs/jammy-updates,jammy-updates,now 22.04.5 all [installed,automatic]
ubuntu-drivers-common/jammy-updates,now 1:0.9.6.2~0.22.04.4 amd64 [installed,automatic]
ubuntu-keyring/jammy,jammy,now 2021.03.26 all [installed,automatic]
ubuntu-minimal/jammy,now 1.481 amd64 [installed,upgradable to: 1.481.1]
ubuntu-mono/jammy,jammy,now 20.10-0ubuntu2 all [installed,automatic]
ubuntu-release-upgrader-core/jammy-updates,jammy-updates,now 1:22.04.16 all [installed,automatic]
ubuntu-release-upgrader-gtk/jammy-updates,jammy-updates,now 1:22.04.16 all [installed,automatic]
ubuntu-report/jammy,now 1.7.1 amd64 [installed,automatic]
ubuntu-session/jammy,jammy,now 42.0-1ubuntu2 all [installed,automatic]
ubuntu-settings/jammy,jammy,now 22.04.6 all [installed,automatic]
ubuntu-standard/jammy,now 1.481 amd64 [installed,upgradable to: 1.481.1]
ubuntu-wallpapers-jammy/jammy,jammy,now 22.04.4-0ubuntu1 all [installed,automatic]
ubuntu-wallpapers/jammy,jammy,now 22.04.4-0ubuntu1 all [installed]
ucf/jammy,jammy,now 3.0043 all [installed,automatic]
udev/jammy-updates,now 249.11-0ubuntu3.9 amd64 [installed,automatic]
udisks2/jammy,now 2.9.4-1ubuntu2 amd64 [installed,automatic]
ufw/jammy,jammy,now 0.36.1-4build1 all [installed,automatic]
unattended-upgrades/jammy,jammy,now 2.8ubuntu1 all [installed,automatic]
uno-libs-private/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
unzip/jammy-updates,jammy-security,now 6.0-26ubuntu3.1 amd64 [installed,automatic]
update-inetd/jammy,jammy,now 4.51 all [installed,automatic]
update-manager-core/jammy-updates,jammy-updates,now 1:22.04.10 all [installed,automatic]
update-manager/jammy-updates,jammy-updates,now 1:22.04.10 all [installed,automatic]
update-notifier-common/jammy-updates,jammy-updates,now 3.192.54.6 all [installed,automatic]
update-notifier/jammy-updates,now 3.192.54.6 amd64 [installed,automatic]
upower/jammy,now 0.99.17-1 amd64 [installed,automatic]
ure/jammy-updates,jammy-security,now 1:7.3.7-0ubuntu0.22.04.3 amd64 [installed,automatic]
usb-creator-common/jammy,jammy,now 0.3.13 all [installed,automatic]
usb-creator-gtk/jammy,jammy,now 0.3.13 all [installed,automatic]
usb-modeswitch-data/jammy,jammy,now 20191128-4 all [installed,automatic]
usb-modeswitch/jammy,now 2.6.1-3ubuntu2 amd64 [installed,automatic]
usb.ids/jammy,jammy,now 2022.04.02-1 all [installed,automatic]
usbmuxd/jammy,now 1.1.1-2build2 amd64 [installed,automatic]
usbutils/jammy,now 1:014-1build1 amd64 [installed,automatic]
usrmerge/jammy,jammy,now 25ubuntu2 all [installed,automatic]
util-linux/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
uuid-runtime/jammy,now 2.37.2-4ubuntu3 amd64 [installed,automatic]
vim-common/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2:8.2.3995-1ubuntu2.9 all [installed,automatic]
vim-tiny/jammy-updates,jammy-security,now 2:8.2.3995-1ubuntu2.9 amd64 [installed,automatic]
wamerican/jammy,jammy,now 2020.12.07-2 all [installed,automatic]
wbritish/jammy,jammy,now 2020.12.07-2 all [installed,automatic]
wget/jammy,now 1.21.2-2ubuntu1 amd64 [installed,automatic]
whiptail/jammy,now 0.52.21-5ubuntu2 amd64 [installed,automatic]
whoopsie-preferences/jammy,now 23 amd64 [installed,automatic]
whoopsie/jammy,now 0.2.77 amd64 [installed,automatic]
wireless-regdb/jammy-updates,jammy-updates,jammy-security,jammy-security,now 2022.06.06-0ubuntu1~22.04.1 all [installed,automatic]
wireless-tools/jammy,now 30~pre9-13.1ubuntu4 amd64 [installed,automatic]
wpasupplicant/jammy-updates,now 2:2.10-6ubuntu2 amd64 [installed,automatic]
x11-apps/jammy,now 7.7+8build2 amd64 [installed,automatic]
x11-common/jammy,jammy,now 1:7.7+23ubuntu2 all [installed,automatic]
x11-session-utils/jammy,now 7.7+4build2 amd64 [installed,automatic]
x11-utils/jammy,now 7.7+5build2 amd64 [installed,automatic]
x11-xkb-utils/jammy,now 7.7+5build4 amd64 [installed,automatic]
x11-xserver-utils/jammy,now 7.7+9build1 amd64 [installed,automatic]
xauth/jammy,now 1:1.1-1build2 amd64 [installed,automatic]
xbitmaps/jammy,jammy,now 1.1.1-2.1ubuntu1 all [installed,automatic]
xbrlapi/jammy-updates,now 6.4-4ubuntu3 amd64 [installed,automatic]
xcursor-themes/jammy,jammy,now 1.0.6-0ubuntu1 all [installed,automatic]
xcvt/jammy,now 0.1.1-3 amd64 [installed,automatic]
xdg-dbus-proxy/jammy,now 0.1.3-1 amd64 [installed,automatic]
xdg-desktop-portal-gnome/jammy-updates,now 42.1-0ubuntu1 amd64 [installed,automatic]
xdg-desktop-portal-gtk/jammy,now 1.14.0-1build1 amd64 [installed,automatic]
xdg-desktop-portal/jammy-updates,now 1.14.4-1ubuntu2~22.04.1 amd64 [installed,automatic]
xdg-user-dirs-gtk/jammy,now 0.10-3build2 amd64 [installed,automatic]
xdg-user-dirs/jammy,now 0.17-2ubuntu4 amd64 [installed,automatic]
xdg-utils/jammy-updates,jammy-updates,now 1.1.3-4.1ubuntu3~22.04.1 all [installed,automatic]
xfonts-base/jammy,jammy,now 1:1.0.5 all [installed,automatic]
xfonts-encodings/jammy,jammy,now 1:1.0.5-0ubuntu2 all [installed,automatic]
xfonts-scalable/jammy,jammy,now 1:1.0.3-1.2ubuntu1 all [installed,automatic]
xfonts-utils/jammy,now 1:7.7+6build2 amd64 [installed,automatic]
xinit/jammy,now 1.4.1-0ubuntu4 amd64 [installed,automatic]
xinput/jammy,now 1.6.3-1build2 amd64 [installed,automatic]
xkb-data/jammy,jammy,now 2.33-1 all [installed,automatic]
xml-core/jammy,jammy,now 0.18+nmu1 all [installed,automatic]
xorg-docs-core/jammy,jammy,now 1:1.7.1-1.2 all [installed,automatic]
xorg/jammy,now 1:7.7+23ubuntu2 amd64 [installed,automatic]
xserver-common/jammy-updates,jammy-updates,now 2:21.1.4-2ubuntu1.7~22.04.1 all [installed,automatic]
xserver-xephyr/jammy-updates,now 2:21.1.4-2ubuntu1.7~22.04.1 amd64 [installed,automatic]
xserver-xorg-core/jammy-updates,now 2:21.1.4-2ubuntu1.7~22.04.1 amd64 [installed,automatic]
xserver-xorg-input-all/jammy,now 1:7.7+23ubuntu2 amd64 [installed,automatic]
xserver-xorg-input-libinput/jammy,now 1.2.1-1 amd64 [installed,automatic]
xserver-xorg-input-wacom/jammy,now 1:1.0.0-3ubuntu1 amd64 [installed,automatic]
xserver-xorg-legacy/jammy-updates,now 2:21.1.4-2ubuntu1.7~22.04.1 amd64 [installed,automatic]
xserver-xorg-video-all/jammy,now 1:7.7+23ubuntu2 amd64 [installed,automatic]
xserver-xorg-video-amdgpu/jammy-updates,now 22.0.0-1ubuntu0.1 amd64 [installed,automatic]
xserver-xorg-video-ati/jammy-updates,now 1:19.1.0-2ubuntu1 amd64 [installed,automatic]
xserver-xorg-video-fbdev/jammy,now 1:0.5.0-2build1 amd64 [installed,automatic]
xserver-xorg-video-intel/jammy,now 2:2.99.917+git20210115-1 amd64 [installed,automatic]
xserver-xorg-video-nouveau/jammy,now 1:1.0.17-2build1 amd64 [installed,automatic]
xserver-xorg-video-qxl/jammy,now 0.1.5+git20200331-3 amd64 [installed,automatic]
xserver-xorg-video-radeon/jammy-updates,now 1:19.1.0-2ubuntu1 amd64 [installed,automatic]
xserver-xorg-video-vesa/jammy,now 1:2.5.0-1build4 amd64 [installed,automatic]
xserver-xorg-video-vmware/jammy,now 1:13.3.0-3build1 amd64 [installed,automatic]
xserver-xorg/jammy,now 1:7.7+23ubuntu2 amd64 [installed,automatic]
xwayland/jammy-updates,jammy-security,now 2:22.1.1-1ubuntu0.6 amd64 [installed,automatic]
xxd/jammy-updates,jammy-security,now 2:8.2.3995-1ubuntu2.9 amd64 [installed,automatic]
xz-utils/jammy,now 5.2.5-2ubuntu1 amd64 [installed,automatic]
yaru-theme-gnome-shell/jammy,jammy,now 22.04.4 all [installed,automatic]
yaru-theme-gtk/jammy,jammy,now 22.04.4 all [installed,automatic]
yaru-theme-icon/jammy,jammy,now 22.04.4 all [installed,automatic]
yaru-theme-sound/jammy,jammy,now 22.04.4 all [installed,automatic]
yelp-xsl/jammy,jammy,now 42.0-1 all [installed,automatic]
yelp/jammy,now 42.1-1 amd64 [installed,automatic]
zenity-common/jammy-updates,jammy-updates,now 3.42.1-0ubuntu1 all [installed,automatic]
zenity/jammy-updates,now 3.42.1-0ubuntu1 amd64 [installed,automatic]
zerofree/jammy,now 1.1.1-1build3 amd64 [installed,automatic]
zip/jammy,now 3.0-12build2 amd64 [installed,automatic]
zlib1g/jammy-updates,jammy-security,now 1:1.2.11.dfsg-2ubuntu9.2 amd64 [installed,automatic]
zstd/jammy,now 1.4.8+dfsg-3build1 amd64 [installed,automatic]
leo@leo-VirtualBox:~$ systemctl list-units --all --type=service --state=active
  UNIT                                                  LOAD   ACTIVE SUB     D>
  accounts-daemon.service                               loaded active running A>
  acpid.service                                         loaded active running A>
  alsa-restore.service                                  loaded active exited  S>
  apparmor.service                                      loaded active exited  L>
  apport.service                                        loaded active exited  L>
  avahi-daemon.service                                  loaded active running A>
  colord.service                                        loaded active running M>
  console-setup.service                                 loaded active exited  S>
  cron.service                                          loaded active running R>
  cups-browsed.service                                  loaded active running M>
  cups.service                                          loaded active running C>
  dbus.service                                          loaded active running D>
  fwupd.service                                         loaded active running F>
  gdm.service                                           loaded active running G>
  irqbalance.service                                    loaded active running i>
  kerneloops.service                                    loaded active running T>
  keyboard-setup.service                                loaded active exited  S>
  kmod-static-nodes.service                             loaded active exited  C>
  ModemManager.service                                  loaded active running M>
  networkd-dispatcher.service                           loaded active running D>
  NetworkManager-wait-online.service                    loaded active exited  N>
  NetworkManager.service                                loaded active running N>
  openvpn.service                                       loaded active exited  O>
  packagekit.service                                    loaded active running P>
  plymouth-quit-wait.service                            loaded active exited  H>
  plymouth-read-write.service                           loaded active exited  T>
  plymouth-start.service                                loaded active exited  S>
  polkit.service                                        loaded active running A>
  power-profiles-daemon.service                         loaded active running P>
  rsyslog.service                                       loaded active running S>
  rtkit-daemon.service                                  loaded active running R>
  setvtrgb.service                                      loaded active exited  S>
  snapd.apparmor.service                                loaded active exited  L>
  snapd.seeded.service                                  loaded active exited  W>
  snapd.service                                         loaded active running S>
  switcheroo-control.service                            loaded active running S>
  systemd-fsck@dev-disk-by\x2duuid-D1D4\x2dC99C.service loaded active exited  F>
  systemd-journal-flush.service                         loaded active exited  F>
lines 17-39

leo@leo-VirtualBox:~$ 
