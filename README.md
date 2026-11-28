# Hi, I'm Roman

I'm an embedded engineer working primarily with C, C++, Rust and Python across
Linux, RTOS, hypervisors, heterogeneous systems and SoCs, developing low-latency
complex systems for various platforms. 

## What I work on now

At my day job, I work on Linux BSPs and automotive HiL infrastructure,
designing and developing test rigs that integrate VHI, chip emulation and
FMI-based simulation components for [Toyota's ARENE platform](https://woven.toyota/en/technology/arene) 🚗.

Outside work I mostly design small boards and the firmware that runs on them:

- [fanny](https://github.com/rmskkn/fanny): a four-channel USB PWM fan
  controller on an STM32F103 Blue Pill. I did the schematic and PCB in KiCad,
  the 3D-printed case in FreeCAD, the C firmware, and a Python host tool.
- [chunky_mcu_updater](https://github.com/rmskkn/chunky_mcu_updater): a
  remote firmware updater for small MCUs. It sends only the flash sectors that
  changed, keeps A/B partitions, and can always roll back to the image that
  was running before the update.
- [cypm1111_pd](https://github.com/rmskkn/cypm1111_pd): firmware for the
  Infineon CYPM1111 USB-PD controller that builds with plain `make` and
  `arm-none-eabi-gcc`, no ModusToolbox needed.
- [proxy-registry](https://github.com/rmskkn/proxy-registry): a caching
  HTTP/HTTPS proxy in Go that splits downloads into parallel streams, so
  pulling container images from a far-away registry stops crawling.

Lately I spend a lot of time on LLM agents for hardware work: driving KiCad
and FreeCAD through MCP servers, autorouting PCBs, and checking that the
results pass DRC. I send patches upstream when I hit bugs, for example to
[KiCAD-MCP-Server](https://github.com/mixelpixx/KiCAD-MCP-Server),
[KiCadRoutingTools](https://github.com/drandyhaas/KiCadRoutingTools) and
[hermes-agent](https://github.com/rmskkn/hermes-agent).

For fun I keep a Klipper config for my
[Ender-3 V3 SE](https://github.com/rmskkn/ender3se_klipper_config), and I
maintain my own [QMK](https://github.com/rmskkn/qmk_firmware) and
[ZMK](https://github.com/rmskkn/zmk) keyboard firmware and
[zmk-config](https://github.com/rmskkn/zmk-config), including a Cirque ⌨️
touchpad driver. My desktop runs patched dwm, st and slstatus on Arch.

## Where I've worked before

- Wi-Fi routers and mesh: OpenSync and RDK OneWifi features, 802.11be
  support, Qualcomm QSDK in Yocto, trusted boot with CMS and OP-TEE.
- Automotive: secure domain boot for the Xen hypervisor, OSTree updates,
  AGL bring-up on i.MX8QM, and kernel patches sent to mainline.
- Video on RISC-V: a MIPI ISP driver on V4L2, RTP streaming, and OpenAMP
  IPC between cores, debugged with a scope and a logic analyzer next to the
  ASIC team.


## Skills

| Area | Tools and tech |
|---|---|
| Languages | C, C++, Rust, Python, Zig, Go, Bash |
| OS and RTOS | Linux, FreeRTOS, Zephyr, bare metal |
| Concurrency and real time | multithreading, pthreads, RTOS scheduling, worst-case execution time, IRQ and DMA design, OpenAMP IPC |
| Linux kernel | drivers, mm, IRQs, DMA, perf, kprobes, kgdb, tracing |
| Build and distros | Yocto, Buildroot, OpenWRT, Debos, CMake, Make, Autotools |
| Boot and security | U-Boot, ARM-TF, OP-TEE, secure boot, AppArmor, seccomp, OpenSSL, HSM |
| Virtualization | Xen, KVM, QEMU, Docker |
| Architectures | ARMv7, ARMv8, Cortex-M, RISC-V |
| Wireless | Wi-Fi (802.11ax/be), BLE, LoRa |
| Buses | USB, USB-PD, PCI, SPI, I2C, I2S, MIPI, CAN, LIN, Modbus |
| Networking | TCP/IP, UDP, RTP, TLS, IPsec, Open vSwitch, MQTT, Protobuf |
| Hardware | KiCad, Altium, FreeCAD, oscilloscope, logic analyzer, JTAG/SWD |
| Testing and CI | GTest, CMocka, HIL tests, GitHub Actions, GitLab CI, Jenkins |

## Hobbies

Outside work I hack on things, build local AI setups, tinker with hardware,
go hiking, and spend time with my family.

## Contact

Find me on GitHub as [@rmskkn](https://github.com/rmskkn) or reach me at rm.skakun@gmail.com.
