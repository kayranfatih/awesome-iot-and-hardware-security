# Awesome IoT and Hardware Security [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A collection of awesome tools, books, resources, software, documents and cool stuff about Internet of Things (IoT) and Hardware Security.

Thanks to all [contributors](https://github.com/kayranfatih/awesome-iot-and-hardware-security/graphs/contributors). The goal is to build community-driven collection of well-known resources.

## Contents
- [**Testing Tools**](#testing-tools)
  - [Debugging Tools](#debugging-tools)
  - [Logic Analyzer and Oscilloscope](#logic-analyzer-and-oscilloscope)
  - [SDR](#sdr)
  - [RFID and NFC](#rfid-and-nfc)
  - [Bluetooth and BLE](#bluetooth-and-ble)
  - [Wi-Fi](#wi-fi)
  - [Zigbee](#zigbee)
  - [LoRaWAN, Thread and Cellular](#lorawan-thread-and-cellular)
  - [MQTT](#mqtt)
  - [USB](#usb)
  - [Automotive and CAN Bus](#automotive-and-can-bus)
  - [Fault Injection - Glitching and Side Channel Analysis](#fault-injection---glitching-and-side-channel-analysis)
  - [Firmware Analysis and Exploit Frameworks](#firmware-analysis-and-exploit-frameworks)
  - [Reverse Engineering](#reverse-engineering)
  - [Silicon Reverse Engineering](#silicon-reverse-engineering)
  - [Fuzzing](#fuzzing)
  - [Misc Tools](#misc-tools)
- [**Penetration Test Use-Cases**](#penetration-test-use-cases)
- [**Standards and Regulations**](#standards-and-regulations)
- [**Books**](#books)
- [**Useful Websites**](#useful-websites)
- [**YouTube Channels**](#youtube-channels)
- [**Twitter Accounts**](#twitter-accounts)
- [**Blogs**](#blogs)
- [**Trainings**](#trainings)
- [**Practice Targets and CTFs**](#practice-targets-and-ctfs)
- [**Conferences**](#conferences)
- [**Awesome Lists**](#awesome-lists)

## Testing Tools
### Debugging Tools
- [Bus Pirate](https://buspirate.com/) - Open-source multi-protocol tool for talking to chips over 1-Wire, I2C, SPI, UART, and other buses from a serial terminal.
- [SEGGER J-Link Debug Probes](https://www.segger.com/products/debug-probes/j-link/) - Widely used commercial JTAG/SWD debug probes with broad CPU and IDE support.
- [Flipper Zero](https://flipper.net/) - Portable, open-source multi-tool for sub-GHz radio, RFID, NFC, infrared, and GPIO hardware hacking.
- [FTDI FT2232H](https://www.ftdichip.com/old2020/Products/ICs/FT2232H.html) - USB 2.0 Hi-Speed dual-channel chip whose MPSSE engines can drive JTAG, SPI, and I2C; the basis of many hardware hacking adapters.
- [Tigard](https://www.crowdsupply.com/securinghw/tigard) - Open-source FT2232H-based, multi-protocol, multi-voltage tool for hardware hacking.
- [JTAGulator](https://github.com/grandideastudio/jtagulator) - Open-source hardware tool that helps identify JTAG and UART interfaces on unknown targets.
- [OpenOCD: Open On-Chip Debugger](https://openocd.org/) - Open-source JTAG/SWD debugger and in-system programmer supporting a wide range of targets and probes.
- [Glasgow Interface Explorer](https://glasgow-embedded.org/en/intro.html) - Digital interface multitool for interacting with, analyzing, and bridging a wide range of low-speed interfaces used in embedded systems.
- [GreatFET](https://github.com/greatscottgadgets/greatfet) - Open-source hardware hacking tool for interfacing with and instrumenting embedded devices over USB.
- [Black Magic Probe](https://black-magic.org/) - JTAG/SWD debug probe with a built-in GDB server, so no OpenOCD is needed.
- [Raspberry Pi Debug Probe](https://www.raspberrypi.com/products/debug-probe/) - Low-cost RP2040-based CMSIS-DAP probe with SWD and UART.
- [probe-rs](https://probe.rs/) - Rust-based toolkit for flashing and debugging embedded targets with CMSIS-DAP, ST-Link, J-Link, and other probes.
- [pyOCD](https://pyocd.io/) - Python-based debugger and programmer for Arm Cortex-M microcontrollers.
- [HydraBus](https://hydrabus.com/) - Open-source STM32-based multi-tool for hardware hacking, debugging, and protocol bridging.
- [PCBite](https://sensepeek.com/) - Hands-free probe and PCB holder system for measuring and tapping signals on small boards.

### Logic Analyzer and Oscilloscope
- [Saleae Logic Analyzer](https://www.saleae.com/) - USB logic analyzers with decoders for SPI, I2C, serial, and many other protocols, plus support for custom analyzers.
- [Pico Oscilloscope](https://www.picotech.com/products/oscilloscope) - PC-based oscilloscopes, a compact alternative to traditional benchtop scopes.
- [sigrok](https://sigrok.org/wiki/Main_Page) - Open-source signal analysis suite, including the PulseView GUI, that supports many low-cost logic analyzers and protocol decoders.
- [DSLogic](https://www.dreamsourcelab.com/) - USB logic analyzers from DreamSourceLab with the open-source DSView software.

### SDR
- [GNURadio](https://github.com/gnuradio/gnuradio) - Free and open-source toolkit of signal processing blocks for building software-defined radios, with or without RF hardware.
- [RTL-SDR](https://www.rtl-sdr.com/) - Ultra-cheap SDR based on RTL2832U DVB-T dongles, usable as a wideband radio scanner.
- [HackRF One](https://greatscottgadgets.com/hackrf/one/) - Open-source SDR peripheral from Great Scott Gadgets that can transmit and receive from 1 MHz to 6 GHz.
- [BladeRF](https://www.nuand.com/bladerf-1/) - Full-duplex SDR platform from Nuand for RF experimentation and development.
- [rtl_433](https://github.com/merbanan/rtl_433) - Decoder for 433/868/315/915 MHz ISM band devices such as sensors, remotes, and meters.
- [inspectrum](https://github.com/miek/inspectrum) - Tool for visualizing and analyzing captured radio signals.
- [SDR++](https://www.sdrpp.org/) - Cross-platform, lightweight SDR receiver software.
- [YARD Stick One](https://greatscottgadgets.com/yardstickone/) - Sub-1 GHz wireless transceiver controlled by RfCat for analyzing and transmitting digital radio protocols.
- [PortaPack Mayhem](https://github.com/portapack-mayhem/mayhem-firmware) - Feature-rich firmware for the HackRF One with PortaPack for standalone RF analysis.
- [Signal Identification Wiki](https://www.sigidwiki.com/wiki/Signal_Identification_Guide) - Reference database for identifying radio signals by frequency, modulation, and waterfall appearance.

### RFID and NFC
- [Proxmark Platform](https://github.com/RfidResearchGroup/proxmark3) - RFID swiss-army tool for low- and high-level interaction with the vast majority of RFID tags and systems, and the de facto standard for RFID analysis.
- [HydraNFC](https://hydrabus.com/hydranfc-1-0-specifications) - NFC shield for HydraBus to sniff, read, write, and emulate 13.56 MHz NFC tags.
- [ChameleonUltra](https://github.com/RfidResearchGroup/ChameleonUltra) - Open-source NFC emulation and research platform for low-frequency and high-frequency RFID work.
- [libnfc](https://github.com/nfc-tools/libnfc) - Platform-independent NFC library and tools for working with readers and tags.
- [MIFARE Classic Tool](https://github.com/ikarus23/MifareClassicTool) - Android app for reading, writing, analyzing, and cloning MIFARE Classic tags.

### Bluetooth and BLE
- [bettercap](https://github.com/bettercap/bettercap) - Extensible Go framework for reconnaissance and attacks on Wi-Fi networks, BLE devices, wireless HID devices, and Ethernet networks.
- [Btlejack](https://github.com/virtualabs/btlejack) - Sniff, jam, and hijack Bluetooth Low Energy connections with low-cost nRF51 hardware such as the BBC micro:bit.
- [Ubertooth One](https://greatscottgadgets.com/ubertoothone/) - Open-source 2.4 GHz wireless development platform for Bluetooth experimentation.
- [nRF51 DK](https://www.nordicsemi.com/Products/Development-hardware/nRF51-DK) - Bluetooth Low Energy development kit for the nRF51 series.
- [ESP32](https://www.espressif.com/en/products/socs/esp32) - Wi-Fi and Bluetooth MCU found in many IoT products and useful as a low-cost research platform.
- [Sniffle](https://github.com/nccgroup/Sniffle) - Sniffer for Bluetooth 5 and 4.x LE using TI CC1352/CC26x2 hardware.
- [nRF Sniffer for Bluetooth LE](https://www.nordicsemi.com/Products/Development-tools/nRF-Sniffer-for-Bluetooth-LE) - Nordic's sniffer firmware and Wireshark plugin for capturing BLE traffic with nRF52 hardware.
- [Mirage](https://github.com/RCayre/mirage) - Python framework for auditing wireless protocols such as BLE, Zigbee, Enhanced ShockBurst, and infrared.
- [WHAD](https://github.com/whad-team/whad-client) - Wireless Hacking Devices framework providing a common protocol and tools for BLE, Zigbee, ESB, and other radios.
- [InternalBlue](https://github.com/seemoo-lab/internalblue) - Bluetooth experimentation framework for Broadcom and Cypress chips that enables low-level firmware analysis and patching.

### Wi-Fi
- [aircrack-ng](https://www.aircrack-ng.org/) - Suite for monitoring, attacking, testing, and cracking Wi-Fi networks.
- [Kismet](https://www.kismetwireless.net/) - Wireless network and device detector, sniffer, and WIDS that also supports Bluetooth, Zigbee, and SDR sources.
- [ESP32 Marauder](https://github.com/justcallmekoko/ESP32Marauder) - Offensive and defensive Wi-Fi and Bluetooth toolkit running on ESP32 boards.

### Zigbee
- [RaspBee](https://phoscon.de/en/raspbee/) - Zigbee gateway board for the Raspberry Pi.
- [nRF52840 Dongle](https://www.nordicsemi.com/Products/Development-hardware/nRF52840-Dongle) - Low-cost USB dongle supporting Bluetooth LE, Thread, Zigbee, and IEEE 802.15.4, often used as a sniffer.
- [ZigDiggity](https://github.com/BishopFox/zigdiggity) - Zigbee hacking toolkit from Bishop Fox.
- [KillerBee](https://github.com/riverloopsec/killerbee) - Framework and tools for sniffing, injecting, and auditing Zigbee and IEEE 802.15.4 networks.

### LoRaWAN, Thread and Cellular
- [LoRaWAN Auditing Framework](https://github.com/IOActive/laf) - Tools to craft, parse, send, analyze, and crack LoRaWAN packets during security audits.
- [ChirpOTLE](https://github.com/seemoo-lab/chirpotle) - LoRaWAN security evaluation framework for practical attacks on real networks.
- [OpenThread](https://openthread.io/) - Open-source implementation of the Thread networking protocol, useful for building Thread and Matter test networks.
- [QCSuper](https://github.com/P1sec/QCSuper) - Captures 2G/3G/4G radio frames from Qualcomm-based phones and modems into Wireshark.
- [LTESniffer](https://github.com/SysSec-KAIST/LTESniffer) - Open-source LTE downlink and uplink eavesdropper.
- [srsRAN Project](https://www.srsran.com/) - Open-source 4G and 5G software radio suite for building cellular test networks.

### MQTT
- [Nmap MQTT Library](https://nmap.org/nsedoc/lib/mqtt.html) - NSE library for interacting with MQTT brokers from Nmap scripts.
- [MQTT-PWN](https://mqtt-pwn.readthedocs.io/en/latest/) - One-stop shop for IoT broker penetration testing that combines enumeration, supportive functions, and exploitation modules in a shell-like CLI.
- [Eclipse Mosquitto](https://mosquitto.org/) - Lightweight open-source broker implementing MQTT 5.0, 3.1.1, and 3.1, handy for building test setups.

### USB
- [Cynthion](https://greatscottgadgets.com/cynthion/) - Open-source USB test instrument from Great Scott Gadgets for analyzing and emulating USB devices.
- [Facedancer](https://github.com/greatscottgadgets/facedancer) - Python framework for emulating and fuzzing USB devices with GreatFET or Cynthion hardware.

### Automotive and CAN Bus
- [can-utils](https://github.com/linux-can/can-utils) - Linux SocketCAN user-space utilities for dumping, sending, and replaying CAN traffic.
- [SavvyCAN](https://github.com/collin80/SavvyCAN) - Cross-platform tool for capturing, visualizing, and reverse engineering CAN bus traffic.
- [Caring Caribou](https://github.com/CaringCaribou/caringcaribou) - Automotive security exploration tool for discovering ECUs and services over CAN, UDS, and XCP.
- [python-can](https://github.com/hardbyte/python-can) - Python library providing a common interface to many CAN hardware adapters.
- [ICSim](https://github.com/zombieCraig/ICSim) - Instrument cluster simulator for practicing CAN bus hacking with SocketCAN.

### Fault Injection - Glitching and Side Channel Analysis
- [An Introduction to Fault Injection by NCC Group](https://www.nccgroup.com/research/an-introduction-to-fault-injection-part-13/) - First part of a series introducing fault injection techniques and their impact on embedded devices.
- [One Glitch to Rule Them All: Fault Injection Attacks against AMD's Secure Processor](https://i.blackhat.com/EU-21/Wednesday/EU-21-Buhren-One-Glitch-to-Rule-them-All-Fault-Injection-Attacks-Against-AMDs-Secure-Processor.pdf) - Black Hat Europe 2021 research on voltage glitching AMD's Secure Processor.
- [ChipWhisperer Kit](https://www.newae.com/chipwhisperer) - Open-source, low-cost ecosystem for side-channel power analysis and glitching attacks.
- [ChipSHOUTER Kit](https://rtfm.newae.com/ChipSHOUTER/ChipSHOUTER/) - Fully featured electromagnetic fault injection (EMFI) platform for discovering and characterizing vulnerabilities in embedded systems.
- [ChipSHOUTER-PicoEMP Kit](https://github.com/newaetech/chipshouter-picoemp) - Lower-cost PicoEMP build for self-study and hobbyist EMFI research from the NewAE ecosystem.
- [RP2040: Pico Glitcher](https://github.com/ZeusWPI/pico-glitcher) - Low-cost voltage glitcher based on the Raspberry Pi Pico.
- [ICEStick ICE40 FPGA Glitcher](https://github.com/SySS-Research/icestick-glitcher) - Simple voltage glitcher built on the Lattice iCEstick evaluation kit.
- [Curious Bolt](https://bolt.curious.supplies/) - Low-cost voltage glitcher, logic analyzer, and differential power analysis tool on a single board.
- [Faultier](https://github.com/hextreeio/faultier) - Fault injection framework for the Raspberry Pi Pico combined with Hextree's Faultier hardware.
- [Faulty Cat](https://github.com/ElectronicCats/faultycat) - Low-cost EMFI tool from Electronic Cats for self-study and hobbyist research.
- [Lascar](https://github.com/Ledger-Donjon/lascar) - Ledger's Python library for side-channel analysis of power and electromagnetic traces.
- [Rainbow](https://github.com/Ledger-Donjon/rainbow) - Unicorn-based simulator for generating side-channel traces and testing fault injection on code.
- [SCAred](https://gitlab.com/eshard/scared) - Open-source Python side-channel analysis library from eShard.

### Firmware Analysis and Exploit Frameworks
- [EMBA The security analyzer for firmware of embedded devices](https://github.com/e-m-b-a/emba) - Central firmware analysis tool for penetration testers and product security teams, covering extraction, static analysis, emulation-based dynamic analysis, and web reporting.
- [Binwalk](https://github.com/ReFirmLabs/binwalk) - Fast, easy to use tool for analyzing, reverse engineering, and extracting firmware images.
- [Unblob](https://github.com/onekey-sec/unblob) - Accurate extraction suite that recursively unpacks dozens of archive, compression, and file-system formats and carves out unknown chunks.
- [Firmware Mod Kit](https://github.com/rampageX/firmware-mod-kit) - Scripts to deconstruct and rebuild firmware images, mainly Linux-based router images using TRX/uImage and SquashFS/CramFS.
- [Panda.re](https://panda.re/) - Platform for Architecture-Neutral Dynamic Analysis built on QEMU, with record and replay for deep whole-system analyses.
- [The Firmware Analysis and Comparison Tool (FACT)](https://fkie-cad.github.io/FACT_core/) - Automates firmware security analysis of routers, IoT devices, UEFI, webcams, and drones, with a web UI, plugin system, and REST API.
- [FirmWire](https://github.com/FirmWire/FirmWire) - Full-system baseband firmware emulation platform for dynamic analysis of embedded and mobile firmware.
- [FIRMADYNE](https://github.com/firmadyne/firmadyne) - Automated system for emulating and dynamically analyzing Linux-based embedded firmware.
- [FirmAE](https://github.com/pr0v3rbs/FirmAE) - Scalable firmware emulation framework that improves analysis coverage for Linux-based IoT firmware.
- [HAL - The Hardware Analyzer](https://github.com/emsec/hal) - Comprehensive netlist reverse engineering and manipulation framework.
- [EXPLIoT Framework](https://gitlab.com/expliot_framework/expliot) - Extensible framework of plugins for security testing and exploiting IoT products and infrastructure.
- [RouterSploit](https://github.com/threat9/routersploit) - Open-source exploitation framework dedicated to embedded devices.
- [IoTSecFuzz(ISF)](https://gitlab.com/invuls/iot-projects/iotsecfuzz) - Combines many utilities for comprehensive IoT security testing at all implementation levels, usable as a console or a Python library.
- [HomePwn - Swiss Army Knife for Pentesting of IoT Devices](https://github.com/Telefonica/HomePWN) - Framework for discovering and auditing IoT devices in home and office environments. Archived by its maintainers.
- [QEMU](https://www.qemu.org/) - Generic, open-source machine emulator and virtualizer.
- [Renode](https://antmicro.com/platforms/renode/) - Antmicro's open-source framework for simulating MCUs, SoCs, and multi-node embedded systems.
- [Qiling](https://github.com/qilingframework/qiling) - Binary emulation framework built on Unicorn with operating system and firmware awareness.
- [Unicorn](https://www.unicorn-engine.org/) - Lightweight multi-architecture CPU emulator framework.
- [avatar2](https://github.com/avatartwo/avatar2) - Orchestration framework for dynamic firmware analysis that combines emulators with real hardware.
- [Fuzzware](https://github.com/fuzzware-fuzzer/fuzzware) - Automated, self-configuring fuzzing framework for microcontroller firmware.
- [Greenhouse](https://github.com/sefcom/greenhouse) - Single-service rehosting of Linux-based firmware in user-space emulation.
- [Penguin](https://github.com/rehosting/penguin) - Target-centric rehosting framework for running and analyzing Linux-based firmware.
- [cwe_checker](https://github.com/fkie-cad/cwe_checker) - Detects common bug classes such as buffer overflows and integer issues in binaries using Ghidra.
- [binbloom](https://github.com/quarkslab/binbloom) - Finds the load address and endianness of raw firmware images.
- [Jefferson](https://github.com/onekey-sec/jefferson) - JFFS2 file system extractor.
- [UBI Reader](https://github.com/onekey-sec/ubi_reader) - Tools for extracting UBI and UBIFS images.
- [EMBArk](https://github.com/e-m-b-a/embark) - Web-based enterprise frontend for EMBA.
- [UEFITool](https://github.com/LongSoft/UEFITool) - Viewer and editor for UEFI firmware images.
- [fwhunt-scan](https://github.com/binarly-io/fwhunt-scan) - Binarly's scanner for detecting vulnerabilities in UEFI firmware with FwHunt rules.

### Reverse Engineering
- [Ghidra](https://github.com/NationalSecurityAgency/ghidra) - Software reverse engineering suite developed by the NSA Research Directorate.
- [IDA Pro](https://hex-rays.com/ida-pro/) - Commercial interactive disassembler and decompiler supporting a wide range of processor architectures.
- [Binary Ninja](https://binary.ninja/) - Modern reverse engineering platform with strong automation support for interactive binary analysis.
- [Radare2](https://radare.org/n/radare2.html) - Free/libre toolchain for forensics, software reverse engineering, exploiting, and debugging.
- [Cutter](https://cutter.re/) - Free and open-source reverse engineering GUI powered by Rizin.
- [GDB: The GNU Project Debugger](https://www.sourceware.org/gdb/) - Standard debugger for inspecting running programs, widely used with OpenOCD and QEMU for embedded targets.
- [Rizin](https://rizin.re/) - Portable reverse engineering framework and radare2 fork that powers Cutter.
- [angr](https://angr.io/) - Python binary analysis framework with symbolic execution support.
- [Frida](https://frida.re/) - Dynamic instrumentation toolkit for hooking and tracing code on Linux, Android, and other platforms.
- [ImHex](https://imhex.werwolv.net/) - Hex editor with a pattern language for parsing binary formats, well suited to firmware work.
- [SVD-Loader for Ghidra](https://github.com/leveldown-security/SVD-Loader-Ghidra) - Loads CMSIS-SVD peripheral definitions into Ghidra to label memory-mapped MCU registers.

### Silicon Reverse Engineering
- [Degate](https://github.com/DegateCommunity/Degate) - Tool for reverse engineering digital logic from chip die images.
- [siliconpr0n](https://siliconpr0n.org/) - Wiki and archive of decapped integrated circuit die photos.

### Fuzzing
- [AFL++](https://github.com/AFLplusplus/AFLplusplus) - Community-maintained successor to Google's AFL with faster execution, better mutations and instrumentation, and QEMU/Unicorn modes for firmware.
- [Boofuzz: Network Protocol Fuzzing for Humans](https://github.com/jtpereyda/boofuzz) - Extensible network protocol fuzzing framework and successor to Sulley.
- [LibAFL](https://github.com/AFLplusplus/LibAFL) - Rust library for building custom, high-performance fuzzers.

### Misc Tools
- [Dumpflash](https://github.com/ohjeongwook/dumpflash) - Low-level NAND flash dump and parsing utility.
- [Flashrom](https://github.com/flashrom/flashrom) - Utility for detecting, reading, writing, verifying, and erasing flash chips, both in-system and through external programmers.
- [JTAGenum](https://github.com/cyphunk/JTAGenum) - Scans pins with an Arduino-compatible board or Raspberry Pi to find JTAG and enumerate undocumented instructions.
- [CHIPSEC](https://github.com/chipsec/chipsec) - Platform security assessment framework for analyzing the security of PC hardware, firmware, and low-level platform components.
- [Hak5 Packet Squirrel](https://shop.hak5.org/products/packet-squirrel-mark-ii) - Ethernet tap for capturing device traffic.
- [esptool](https://github.com/espressif/esptool) - Espressif's utility for talking to the ROM bootloader to read and write flash and eFuses on ESP chips.
- [IMSProg](https://github.com/bigbigmdm/IMSProg) - Open-source programmer software for CH341A-based SPI and I2C flash and EEPROM programmers.

## Penetration Test Use-Cases
- [Getting Root on Philips Hue Bridge 2.0 by Colin O'Flynn](https://colinoflynn.com/2016/07/getting-root-on-philips-hue-bridge-2-0/) - Hardware attack walkthrough on the Philips Hue Bridge 2.0.
- [How I hacked a hardware crypto wallet and recovered $2 million by Joe Grand](https://youtu.be/dT9y-KQbqi4?si=k1Zwfd0KIZgRZb-j) - Recovering a locked Trezor One wallet through voltage glitching.
- [How the Apple AirTags were hacked by Thomas Roth](https://www.youtube.com/watch?v=_E0PWQvW-14) - Glitching the nRF52 in Apple AirTags to dump and modify their firmware.
- [Bosch Smart Home Hacks by Sebastien Leger](https://github.com/vegantransistor/BoschSmartHome) - Hardware attacks and firmware analysis on the Bosch Smart Home Controller.
- [Glitched on Earth by Humans: A Black-Box Security Evaluation of the SpaceX Starlink User Terminal by Lennert Wouters](https://www.youtube.com/watch?v=NXqLMmGwJm0) - Voltage glitching the Starlink user terminal with a custom modchip.
- [SECGlitcher - Reproducible Voltage Glitching on STM32 Microcontrollers by SEC Consult](https://sec-consult.com/blog/detail/secglitcher-part-1-reproducible-voltage-glitching-on-stm32-microcontrollers/) - Building a reproducible voltage glitching setup against STM32 microcontrollers.
- [Fault Injection Attacks against the ESP32-C3 and ESP32-C6 by Kevin Courdesses](https://courk.cc/esp32-c3-c6-fault-injection) - Practical glitching of Espressif's RISC-V chips to defeat their security features.
- [Breaking the Flash Encryption Feature of Espressif's Parts by Kevin Courdesses](https://courk.cc/breaking-flash-encryption-of-espressif-parts) - Attack on the flash encryption feature of recent Espressif chips.
- [RP2350 Hacking Challenge Results by Raspberry Pi](https://www.raspberrypi.com/news/security-through-transparency-rp2350-hacking-challenge-results-are-in/) - Winning attacks against the RP2350's secure boot and OTP protections, including glitching and laser fault injection.
- [Shedding too much Light on a Microcontroller's Firmware Protection by Johannes Obermaier and Stefan Tatschner](https://www.usenix.org/conference/woot17/workshop-program/presentation/obermaier) - WOOT '17 paper bypassing STM32F0 readout protection with cold-boot stepping and UV-C attacks.

## Standards and Regulations
- [ETSI EN 303 645 - Cyber Security for Consumer Internet of Things: Baseline Requirements](https://www.etsi.org/deliver/etsi_en/303600_303699/303645/03.01.03_60/en_303645v030103p.pdf) - European baseline security requirements for consumer IoT devices (V3.1.3).
- [ETSI TS 103 701 - Cyber Security for Consumer Internet of Things: Conformance Assessment of Baseline Requirements](https://www.etsi.org/deliver/etsi_ts/103700_103799/103701/02.01.01_60/ts_103701v020101p.pdf) - Test cases and assessment criteria for checking conformance with ETSI EN 303 645.
- [UK Code of Practice for Consumer IoT Security](https://www.gov.uk/government/publications/code-of-practice-for-consumer-iot-security) - UK government guidelines for securing consumer IoT products, the basis for ETSI EN 303 645.
- [EU Cyber Resilience Act](https://digital-strategy.ec.europa.eu/en/policies/cyber-resilience-act) - EU regulation setting cybersecurity requirements for products with digital elements across their lifecycle.
- [Radio Equipment Directive (RED)](https://eur-lex.europa.eu/eli/reg_del/2022/30/oj) - Delegated Regulation (EU) 2022/30 adding cybersecurity, privacy, and fraud-protection requirements to the Radio Equipment Directive, applicable since 1 August 2025.
- [EN 18031-1/-2/-3 Harmonised Standards for RED](https://eur-lex.europa.eu/eli/dec_impl/2025/138/oj) - Implementing Decision (EU) 2025/138 citing the EN 18031 series as harmonised standards for the RED cybersecurity requirements, with restrictions.
- [USA IoT Cybersecurity Improvement Act of 2020](https://www.congress.gov/bill/116th-congress/house-bill/1668) - US law setting minimum security requirements for IoT devices procured by federal agencies.
- [US Cyber Trust Mark](https://www.fcc.gov/CyberTrustMark) - FCC's voluntary cybersecurity labeling program for consumer wireless IoT products.
- [The UK Product Security and Telecommunications Infrastructure (Product Security) regime](https://www.gov.uk/government/publications/the-uk-product-security-and-telecommunications-infrastructure-product-security-regime) - UK consumer connectable product security regime, in force since 29 April 2024, for everyone in the supply chain of these products.
- [Common Criteria](https://www.commoncriteriaportal.org/index.cfm) - International framework for independent, lab-based security evaluation and certification of IT products.
- [NISTIR 8259: Recommendations for IoT Device Manufacturers: Foundational Activities](https://www.nist.gov/itl/applied-cybersecurity/nist-cybersecurity-iot-program/nistir-8259-series) - NIST guidance on foundational cybersecurity activities and device capabilities for IoT manufacturers.
- [ARM PSA IoT Security Framework and Certification](https://www.psacertified.org/) - Security framework and certification scheme for IoT chips, platforms, and devices.
- [China CCRC: Implementation Rules on the Compulsory Certification of Information Technology Equipment](https://www.tuvsud.com/en/knowledge-hub/technical-updates/consumer-products-and-retail-essentials/china-implementation-rules-ccrc-c09-001-2022-for-compulsory-certification-of-it-equipment) - Summary of China's compulsory certification rules for IT equipment (CCRC-C09-001:2022).
- [The C2 Consensus on CSDE - IoT Device Security Baseline Capabilities](https://csde.org/projects/c2-consensus/) - Industry consensus on baseline security capabilities for IoT devices.
- [Information and Communication Security Guide by TUBITAK BILGEM OKTEM](https://oktem.bilgem.tubitak.gov.tr/en/information-and-communication-security-guide/) - English overview of Turkiye's Information and Communication Security Guide and its supporting programme.
- [NIST Recommended Criteria for Cybersecurity Labeling for Consumer Internet of Things (IoT) Products](https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.02042022-2.pdf) - NIST's recommended criteria for a consumer IoT cybersecurity labeling program.
- [ISO/IEC 27402:2023 Cybersecurity - IoT security and privacy: Device baseline requirements](https://www.iso.org/obp/ui/#iso:std:iso-iec:27402:ed-1:v1:en) - International baseline security and privacy requirements for IoT devices.
- [Cybersecurity Labelling Scheme (CLS) by Cyber Security Agency of Singapore](https://www.csa.gov.sg/our-programmes/certification-and-labelling-schemes/cybersecurity-labelling-scheme/about/) - Tiered label that indicates the security level of network-connected smart devices to help consumers choose.
- [IASME IoT Cyber](https://iasme.co.uk/iasme-iot-cyber/) - IASME's certification scheme for internet-connected devices, covering both baseline and assurance levels aligned to UK legislation and ETSI EN 303 645.
- [Global Platform Security Evaluation Standard for IoT Platforms(SESIP)](https://globalplatform.org/sesip/) - Methodology for security evaluation of IoT platforms that certification schemes can reuse.
- [JC-STAR](https://www.ipa.go.jp/en/security/jc-star/) - Japan's IoT product security labeling scheme operated by IPA.
- [ioXt](https://ioxt.com/) - Industry certification program for IoT device security based on ioXt profiles.
- [ISA/IEC 62443](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) - Industrial automation security standards, with IEC 62443-4-2 defining requirements for embedded and IoT components.
- [ISO/SAE 21434](https://www.iso.org/standard/70918.html) - Cybersecurity engineering standard for road vehicle electrical and electronic systems.
- [UN Regulation No. 155](https://unece.org/transport/documents/2021/03/standards/un-regulation-no-155-cyber-security-and-cyber-security) - UNECE regulation requiring a cyber security management system for vehicle type approval.
- [UN Regulation No. 156](https://unece.org/transport/documents/2021/03/standards/un-regulation-no-156-software-update-and-software-update) - UNECE regulation on software update management systems for vehicles.

## Books
- [Microcontroller Exploits](https://nostarch.com/microcontroller-exploits) - 2024, Publisher: No Starch Press, Author(s): Travis Goodspeed.
- [Arm Assembly Internals and Reverse Engineering: Blue Fox Edition](https://www.wiley.com/en-be/Blue+Fox:+Arm+Assembly+Internals+and+Reverse+Engineering-p-9781119745303) - 2023, Publisher: Wiley, Author(s): Maria Markstedter aka Azeria.
- [Practical Hardware Pentesting, Second edition](https://www.packtpub.com/product/practical-hardware-pentesting-second-edition-second-edition/9781803249322) - 2023, Publisher: Packt, Author(s): Jean-Georges Valle.
- [Hardware Security Training, Hands-on!](https://link.springer.com/book/10.1007/978-3-031-31034-8) - 2023, Publisher: Springer, Author(s): Mark Tehranipoor, N. Nalla Anandakumar, Farimah Farahmandi.
- [Practical IoT Hacking](https://nostarch.com/practical-iot-hacking) - 2021, Publisher: No Starch Press, Author(s): Fotios Chantzis, Ioannis Stais, Paulino Calderon, Evangelos Deirmentzoglou, Beau Woods.
- [The Hardware Hacking Handbook: Breaking Embedded Security with Hardware Attacks](https://nostarch.com/hardwarehacking) - 2021, Publisher: No Starch Press, Author(s): Jasper van Woudenberg, Colin O'Flynn.
- [The Hacker's Hardware Toolkit: The best collection of hardware gadgets for red team hackers, pentesters and security researchers](https://github.com/yadox666/The-Hackers-Hardware-Toolkit/blob/master/TheHackersHardwareToolkit.pdf) - 2020, Publisher: N/A, Author(s): Yago Hansen.
- [The IoT Hacker's Handbook: A Practical Guide to Hacking the Internet of Things](https://www.oreilly.com/library/view/the-iot-hackers/9781484243008/) - 2019, Publisher: Apress, Author(s): Aditya Gupta.
- [Hardware Security: A Hands-on Learning Approach](https://shop.elsevier.com/books/hardware-security/bhunia/978-0-12-812477-2) - 2018, Publisher: Morgan Kaufmann, Author(s): Swarup Bhunia, Mark M. Tehranipoor.
- [The Hardware Hacker](https://nostarch.com/hardwarehackerpaperback) - 2017, Publisher: No Starch Press, Author(s): Andrew "bunnie" Huang.
- [IoT Penetration Testing Cookbook](https://www.packtpub.com/product/iot-penetration-testing-cookbook/9781787280571) - 2017, Publisher: Packt, Author(s): Aaron Guzman, Aditya Gupta.
- [The Car Hacker's Handbook](https://nostarch.com/carhacking) - 2016, Publisher: No Starch Press, Author(s): Craig Smith.
- [Hacking the Xbox](https://bunniefoo.com/nostarch/HackingTheXbox_Free.pdf) - 2003, Publisher: No Starch Press, Author(s): Andrew "bunnie" Huang. Free PDF released by the author.

## Useful Websites
- [The MITRE EMB3D Threat Model](https://emb3d.mitre.org/) - Knowledge base of cyber threats to embedded devices, with security mechanisms to mitigate them.
- [OWASP Embedded Application Security Project](https://owasp.org/projects/embedded-application-security) - Technical guidance for manufacturers on building secure embedded devices.
- [OWASP Internet of Things Project](https://owasp.org/projects/internet-of-things) - Helps manufacturers, developers, and consumers understand IoT security issues and make better security decisions.
- [ETSI Cybersecurity, Privacy and Users](https://www.etsi.org/technologies/cybersecurity-privacy-users/) - ETSI's hub for cybersecurity standardization, including its consumer IoT security work.
- [Godbolt Compiler Explorer](https://godbolt.org/) - Online tool for comparing the assembly generated by many compilers and architectures.
- [Dogbolt Decompiler Explorer](https://dogbolt.org/) - Online tool for comparing output from multiple decompilers side by side.
- [Instruction Reference for x86 and amd64](https://www.felixcloutier.com/x86/index.html) - Searchable x86 and amd64 instruction set reference.
- [Hardware Hacking Lab Guide](https://voidstarsec.com/hw-hacking-lab/vss-lab-guide) - Beginner's guide to building a hardware hacking lab.
- [FCC ID Search](https://fccid.io/) - Search FCC filings for internal photos, test reports, and manuals of wireless devices.
- [Octopart](https://octopart.com/) - Electronic component search engine for finding datasheets and part details.
- [Azeria Labs](https://azeria-labs.com/) - Tutorials on Arm assembly, exploitation, and reverse engineering.

## YouTube Channels
- [Colin O'Flynn](https://www.youtube.com/@ColinOFlynn) - Fault injection, side-channel analysis, and ChipWhisperer demos.
- [Joe Grand aka kingpin](https://www.youtube.com/@JoeGrand) - Hardware hacking projects, including crypto wallet recoveries.
- [stacksmashing](https://www.youtube.com/@stacksmashing) - Hardware hacking and reverse engineering of consumer devices.
- [LiveOverflow](https://www.youtube.com/@LiveOverflow) - Security research and CTF videos, including a hardware security series.
- [hackaday](https://www.youtube.com/@hackaday) - Conference talks and videos on electronics and hardware hacking.
- [RECESSIM](https://www.youtube.com/@RECESSIM) - Hardware reverse engineering videos and livestreams.
- [IoTVillage](https://www.youtube.com/@IoTVillage) - Talks from the DEF CON IoT Village.
- [Flashback Team](https://www.youtube.com/@FlashbackTeam) - IoT and router exploitation, including Pwn2Own research.
- [Matt Brown](https://www.youtube.com/@mattbrwn) - IoT hacking, firmware extraction, and bug hunting walkthroughs.
- [Hextree](https://www.youtube.com/@hextreeio) - Hardware and mobile security videos from the Hextree training team.

## Twitter Accounts
- [Xeno Kovah](https://twitter.com/XenoKovah) - Founder of OpenSecurityTraining2, focused on firmware and Bluetooth security.
- [LiveOverflow](https://twitter.com/LiveOverflow) - Security researcher and educator.
- [Colin O'Flynn](https://twitter.com/colinoflynn) - Creator of ChipWhisperer and founder of NewAE Technology.
- [Hash](https://twitter.com/BitBangingBytes) - Hardware reverse engineering and hacking.
- [Cesar Cerrudo](https://twitter.com/cesarcer) - IoT and smart city security researcher.
- [stacksmashing](https://twitter.com/ghidraninja) - Hardware hacker known for the AirTag and Game & Watch hacks.
- [Ken Munro](https://twitter.com/TheKenMunroShow) - Founder of Pen Test Partners, researching IoT, automotive, and aviation security.
- [Travis Goodspeed](https://twitter.com/travisgoodspeed) - Author of Microcontroller Exploits and creator of the GoodFET.
- [Michael Ossmann](https://twitter.com/michaelossmann) - Founder of Great Scott Gadgets and creator of HackRF.
- [Azeria](https://twitter.com/Fox0x01) - Arm reverse engineering and exploitation researcher, author of Blue Fox.
- [Cybergibbons](https://twitter.com/cybergibbons) - Embedded and IoT security researcher.
- [Slawomir Jasek](https://twitter.com/slawekja) - Bluetooth LE and smart lock security researcher.
- [Aseem Jakhar](https://twitter.com/aseemjakhar) - Founder of Payatu and nullcon, creator of EXPLIoT.
- [Kate Temkin](https://twitter.com/ktemkin) - Hardware and USB security researcher, known for Fusée Gelée and USB tooling.
- [Joe Fitz](https://twitter.com/securelyfitz) - Hardware security trainer at SecuringHardware.com.
- [Stephen A. Ridley](https://twitter.com/s7ephen) - Embedded security researcher and hardware hacking trainer.
- [Charlie Miller](https://twitter.com/0xcharlie) - Automotive security researcher known for the remote Jeep Cherokee hack.
- [Samy Kamkar](https://twitter.com/samykamkar) - Hardware and RF hacker behind projects such as OpenSesame and KeySweeper.
- [/dev/ttyS0](https://twitter.com/devttyS0) - Embedded security researcher and original author of binwalk.

## Blogs
- [Cybergibbons](https://cybergibbons.com/) - Embedded and IoT security research.
- [Hackaday](https://hackaday.com/) - Daily hardware hacking news and projects.
- [VoidStar Security Research and Blog Wiki](https://voidstarsec.com/hw-hacking-lab/) - Wiki articles on hardware hacking and other hardware security related content.
- [Riscure's Blog](https://www.riscure.com/blog/) - Side-channel, fault injection, and embedded security research.
- [Quarkslab's Blog](https://blog.quarkslab.com/) - Reverse engineering, vulnerability, and hardware security research.
- [SRLabs' Blog](https://www.srlabs.de/blog) - Research on embedded, telecom, and payment security.
- [Wrongbaud's Blog](https://wrongbaud.github.io/) - Practical hardware hacking tutorials and teardowns.
- [Pen Test Partners Security Blog](https://www.pentestpartners.com/security-blog/) - IoT, automotive, and maritime security research.
- [Limited Results' Blog](https://limitedresults.com/) - Fault injection research on SoCs such as the ESP32 and nRF52.
- [embeddedsecurity.io](https://embeddedsecurity.io/) - Embedded systems security and TrustZone e-book.
- [Ledger Donjon](https://donjon.ledger.com/) - Hardware wallet, side-channel, and fault injection research from Ledger's security team.
- [NCC Group Research](https://www.nccgroup.com/research/) - Hardware, embedded, and cryptography research publications.
- [Synacktiv Publications](https://www.synacktiv.com/publications) - Research on embedded devices, Pwn2Own targets, and reverse engineering.
- [Raelize Blog](https://raelize.com/blog/) - Fault injection research and techniques.
- [bunnie's blog](https://www.bunniestudios.com/) - Andrew "bunnie" Huang's writing on hardware, supply chains, and open hardware.
- [Midnight Blue Research](https://www.midnightblue.nl/knowledge?type=Research) - Embedded and radio protocol security research, including TETRA:BURST.
- [Binarly Blog](https://www.binarly.io/blog) - UEFI and firmware supply chain security research.
- [Eclypsium Blog](https://eclypsium.com/blog/) - Firmware and hardware supply chain security research.
- [Claroty Team82](https://claroty.com/team82) - Research on OT, IoT, and medical device vulnerabilities.
- [Nozomi Networks Labs](https://www.nozominetworks.com/labs) - OT and IoT vulnerability research.

## Trainings
- [OpenSecurityTraining2](https://ost2.fyi/) - Free in-depth security courses, including firmware, x86, and Arm topics.
- [Cyberpath: Practical IoT Hacking](https://cyberpath.training/) - Hands-on IoT hacking training.
- [Hextree.io](https://www.hextree.io/) - Online courses on hardware hacking and mobile security.
- [Attify Offensive IoT Exploitation](https://www.attify-store.com/collections/training) - IoT exploitation training covering firmware, radio, and hardware attacks.
- [Introduction to Reverse Engineering with Ghidra](https://hackaday.io/course/172292-introduction-to-reverse-engineering-with-ghidra) - Four-session course that walks through the basics of reverse engineering software with Ghidra.
- [VoidStar Security Training](https://voidstarsec.com/training) - Hardware hacking and reverse engineering courses.
- [SecuringHardware.com](https://securinghardware.com/) - Joe FitzPatrick's hardware security trainings.

## Practice Targets and CTFs
- [IoTGoat](https://github.com/OWASP/IoTGoat) - Deliberately insecure OpenWrt-based firmware for learning and practicing IoT security testing.
- [DVRF: Damn Vulnerable Router Firmware](https://github.com/praetorian-inc/DVRF) - Vulnerable router firmware image for hands-on embedded web and firmware exploitation practice. Archived by its maintainers.
- [EMUX](https://github.com/therealsaumil/emux) - Embedded device emulation framework for building reproducible firmware-analysis labs.
- [RHme-2015](https://github.com/Riscure/RHme-2015) - Riscure Hack Me hardware CTF challenge.
- [RHme-2016](https://github.com/Riscure/Rhme-2016) - Riscure Hack Me 2 hardware CTF challenge.
- [RHme-2017/2018](https://github.com/Riscure/Rhme-2017) - Riscure Hack Me 3 hardware CTF challenge.
- [Microcorruption](https://microcorruption.com/) - Browser-based embedded exploitation CTF against simulated MSP430 smart locks.
- [DVID](https://github.com/Vulcainreo/DVID) - Damn Vulnerable IoT Device, a purpose-built board for practicing hardware and firmware attacks.
- [BLE CTF](https://github.com/hackgnar/ble_ctf) - Bluetooth Low Energy capture-the-flag that runs on an ESP32.

## Conferences
- [Hardwear.io Security Trainings and Conference](https://hardwear.io/) - Hardware security trainings and conference held in Europe and the USA.
- [HITB Security Conference](https://conference.hitb.org/) - Hack In The Box security conference with hardware and IoT content.
- [IoT Security Foundation Conference](https://iotsecurityfoundation.org/conference/) - Annual conference of the IoT Security Foundation.
- [CHES: Cryptographic Hardware and Embedded Systems](https://ches.iacr.org/) - IACR conference on the design and analysis of cryptographic hardware and embedded systems.
- [HASP Hardware and Architectural Support for Security and Privacy Workshop](https://www.haspworkshop.org/) - Workshop on hardware and architecture-level security and privacy.
- [SILM Security of Software/Hardware Interfaces Workshop](https://silm-workshop.github.io/) - Workshop on the security of software and hardware interfaces.
- [HACK@DAC](https://archive.dac.com/conference/hackdac.html) - Hardware security challenge co-located with the Design Automation Conference where teams find, exploit, and patch vulnerabilities in an open-source SoC.
- [DEF CON Hardware Hacking Village](https://dchhv.org/) - Hardware hacking talks, contests, and hands-on activities at DEF CON.
- [IoT Village](https://www.iotvillage.org/) - IoT hacking talks, contests, and workshops at DEF CON and other events.
- [Car Hacking Village](https://www.carhackingvillage.com/) - Automotive security talks, CTFs, and hands-on activities.
- [REcon](https://recon.cx/) - Reverse engineering conference in Montreal with strong hardware content.
- [TROOPERS](https://troopers.de/) - IT security conference in Heidelberg with hardware and embedded tracks.
- [Chaos Communication Congress](https://events.ccc.de/) - Annual CCC congress with many hardware and embedded security talks.
- [OffensiveCon](https://www.offensivecon.org/) - Offensive security conference in Berlin focused on vulnerability research and exploitation.
- [nullcon](https://nullcon.net/) - Security conference in India and Germany with a hardware village.
- [escar](https://escar.info/) - Automotive cyber security conference.

## Awesome Lists
- [TEE Reversing](https://github.com/enovella/TEE-reversing) - Curated list of public TEE resources for learning how to reverse engineer and achieve trusted code execution on Arm devices.
- [Awesome Connected Things Security](https://github.com/V33RU/awesome-connected-things-sec) - Curated list of IoT and connected-things security resources.
- [Awesome Bluetooth Security (BR, EDR, LE, and Mesh)](https://github.com/engn33r/awesome-bluetooth-security) - Curated Bluetooth Classic, Low Energy, and mesh security resources.
- [Awesome Embedded and IoT Security](https://github.com/fkie-cad/awesome-embedded-and-iot-security) - Curated embedded and IoT security resources from Fraunhofer FKIE.
- [Awesome Embedded Linux](https://github.com/fkromer/awesome-embedded-linux) - Curated embedded Linux resources. Archived by its maintainers.
- [Awesome IoT Hacks](https://github.com/nebgnahz/awesome-iot-hacks) - Collection of documented hacks against IoT devices.
- [Awesome Embedded Linux Security](https://github.com/kayranfatih/awesome-embedded-linux-security) - Companion list on embedded Linux and platform security.
- [Awesome Vehicle Security](https://github.com/jaredthecoder/awesome-vehicle-security) - Curated vehicle and automotive security resources.
- [Awesome Industrial Control System Security](https://github.com/hslatman/awesome-industrial-control-system-security) - Curated ICS security resources.
- [Awesome Fuzzing](https://github.com/secfigo/Awesome-Fuzzing) - Curated fuzzing books, courses, tools, and tutorials.
- [Awesome Hardware and IoT Hacking](https://github.com/JoasASantos/Awesome-Hardware-and-IoT-Hacking) - Curated hardware and IoT hacking resources.
