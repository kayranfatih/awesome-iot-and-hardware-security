# Awesome IoT and Hardware Security 
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A collection of awesome tools, books, resources, software, documents and cool stuff about Internet of Things (IoT) and Hardware Security.

Thanks to all [contributors](https://github.com/kayranfatih/awesome-iot-and-hardware-security/graphs/contributors). The goal is to build community-driven collection of  well-known resources.

## Contents
- [**Testing Tools**](#Testing-Tools)
  - [Debugging Tools](#Debugging-Tools)
  - [Logic Analyzer and Oscilloscope](#Logic-Analyzer-and-Oscilloscope)
  - [SDR](#SDR)
  - [RFID and NFC](#RFID-and-NFC)
  - [Bluetooth and BLE](#Bluetooth-and-BLE)
  - [MQTT](#MQTT)
  - [Zigbee](#Zigbee)
  - [Fault Injection - Glitching and Side Channel Analysis](#Fault-Injection---Glitching-and-Side-Channel-Analysis)
  - [Firmware Analysis and Exploit Frameworks](#Firmware-Analysis-and-Exploit-Frameworks)
  - [Reverse Engineering](#Reverse-Engineering)
  - [Fuzzing](#Fuzzing)
- [**Penetration Test Use-Cases**](#Penetration-Test-Use-Cases)
- [**Standarts and Regulations**](#Standarts-and-Regulations)
- [**Books**](#Books)
- [**Useful Websites**](#Useful-Websites)
- [**Youtube Channels**](#Youtube-Channels)
- [**Twitter Accounts**](#Twitter-Accounts)
- [**Blogs**](#Blogs)
- [**Trainings**](#Trainings)
- [**Conferences**](#Conferences)
- [**Awesome Lists**](#Awesome-Lists)

## Testing Tools
### Debugging Tools
- [Buspirate](https://www.sparkfun.com/products/12942) - The Bus Pirate is a troubleshooting tool that communicates between a PC and any embedded device over 1-wire, 2-wire, 3-wire, UART, I2C, SPI, and HD44780 LCD protocols - all at voltages from 0-5.5VDC
- [SEGGER J-Link Debug Probes](https://www.segger.com/products/debug-probes/j-link/) - SEGGER J-Links are the most widely used line of debug probes on the market. They have provided solid value to embedded development for over a decade. Unparalleled performance, an extensive feature set, many supported CPUs and compatibility with popular environments all make J-Link an unbeatable choice
- [Flipper Zero](https://flipperzero.one/) - Flipper Zero is a portable multi-tool for pentesters and geeks in a toy-like body. It loves hacking digital stuff, such as radio protocols, access control systems, hardware, and more. It's fully open-source and customizable, so you can extend it in whatever way you like
- [FTDI FT2232H](https://www.ftdichip.com/old2020/Products/ICs/FT2232H.html) - The FT2232H is FTDI’s 5th generation of USB devices.  The FT2232H is a USB 2.0 Hi-Speed (480Mb/s) to UART/FIFO IC.  It has the capability of being configured in a variety of industry standard serial or parallel interfaces. The FT2232H has two multi-protocol synchronous serial engines (MPSSEs) which allow for communication using JTAG, I2C and SPI on two channels simultaneously.
- [Hak5 Packet Squirrel](https://shop.hak5.org/products/packet-squirrel-mark-ii) - Ethernet Tap for capturing device traffic
  
### Logic Analyzer and Oscilloscope
- [Saleae Logic Analyzer](https://www.saleae.com/) - Effortlessly decode protocols like SPI, I2C, Serial, and many more. Leverage community created analyzers or build your own low-level or high-level protocol analyzer
- [Pico Oscilloscope](https://www.picotech.com/products/oscilloscope) - PC Oscilloscopes: the modern alternative to the traditional benchtop oscilloscope

### SDR 
- [GNURadio](https://github.com/gnuradio/gnuradio) - GNU Radio is a free & open-source software development toolkit that provides signal processing blocks to implement software radios. It can be used with readily-available, low-cost external RF hardware to create software-defined radios, or without hardware in a simulation-like environment
- [RTL-SDR](https://www.rtl-sdr.com/) - The RTL-SDR is an ultra cheap software defined radio based on DVB-T TV tuners with RTL2832U chips. The RTL-SDR can be used as a wide band radio scanner. It may interest ham radio enthusiasts, hardware hackers, tinkerers and anyone interested in RF
- [HackRF One](https://greatscottgadgets.com/hackrf/one/) - HackRF One from Great Scott Gadgets is a Software Defined Radio peripheral capable of transmission or reception of radio signals from 1 MHz to 6 GHz. Designed to enable test and development of modern and next generation radio technologies, HackRF One is an open source hardware platform that can be used as a USB peripheral or programmed for stand-alone operation
- [BladeRF](https://www.nuand.com/bladerf-1/) - bladeRF is a Software Defined Radio (SDR) platform designed to enable a community of hobbyists, and professionals to explore and experiment with the multidisciplinary facets of RF communication

### RFID and NFC
- [Proxmark Platform](https://proxmark.com/) - The Proxmark is an RFID swiss-army tool, allowing for both high and low level interactions with the vast majority of RFID tags and systems world-wide. Originally built by Jonathan Westhues over 10 years ago, the device has progressively evolved into the industry standard tool for RFID Analysis

### Bluetooth and BLE
- [bettercap](https://github.com/bettercap/bettercap) - bettercap is a powerful, easily extensible and portable framework written in Go which aims to offer to security researchers, red teamers and reverse engineers an easy to use, all-in-one solution with all the features they might possibly need for performing reconnaissance and attacking WiFi networks, Bluetooth Low Energy devices, wireless HID devices and Ethernet networks
- [Btlejack](https://github.com/virtualabs/btlejack) - Btlejack provides everything you need to sniff, jam and hijack Bluetooth Low Energy devices
- [Ubertooth One](https://greatscottgadgets.com/ubertoothone/) - Ubertooth One is an open source 2.4 GHz wireless development platform suitable for Bluetooth experimentation
- [nRF51 DK](https://www.nordicsemi.com/Products/Development-hardware/nrf51-dk) - Bluetooth Low Energy development kit for the nRF51 Series
- [ESP32](https://www.espressif.com/en/products/socs/esp32) - A feature-rich MCU with integrated Wi-Fi and Bluetooth connectivity for a wide-range of applications
 
### MQTT
- [Nmap MQTT Library](https://nmap.org/nsedoc/lib/mqtt.html) - Nmap MQTT Library
- [MQTT-PWN](https://mqtt-pwn.readthedocs.io/en/latest/) - MQTT-PWN intends to be a one-stop-shop for IoT Broker penetration-testing and security assessment operations, as it combines enumeration, supportive functions and exploitation modules while packing it all within command-line-interface with an easy-to-use and extensible shell-like environment
- [Eclipse Mosquitto](https://mosquitto.org/) - Eclipse Mosquitto is an open source (EPL/EDL licensed) message broker that implements the MQTT protocol versions 5.0, 3.1.1 and 3.1. Mosquitto is lightweight and is suitable for use on all devices from low power single board computers to full servers

### Zigbee
- [RaspBee](https://phoscon.de/en/raspbee/) - The universal Raspberry Pi Zigbee gateway
- [nRF52840 Dongle](https://www.nordicsemi.com/Products/Development-hardware/nrf52840-dongle) - The nRF52840 Dongle is a small, low-cost USB dongle that supports Bluetooth 5.4, Bluetooth mesh, Thread, Zigbee, 802.15.4, ANT and 2.4 GHz proprietary protocols
- [ZigDiggity](https://github.com/BishopFox/zigdiggity) - ZigBee Hacking Toolkit

### Fault Injection - Glitching and Side Channel Analysis
- [An Introduction to Fault Injection by NCCGroup](https://research.nccgroup.com/2021/07/07/an-introduction-to-fault-injection-part-1-3/)
- [One Glitch to Rule Them All: Fault Injection Attacks against AMD’s Secure Processor](https://i.blackhat.com/EU-21/Wednesday/EU-21-Buhren-One-Glitch-to-Rule-them-All-Fault-Injection-Attacks-Against-AMDs-Secure-Processor.pdf)
- [Chip.fail](https://chip.fail/) - With chip.fail, we attempt to bring fault-injection (aka glitching) attacks to the masses by providing a very affordable, off-the-shelf toolkit for conducting FI-susceptibility testing 
- [Chipwhisperer Kit](https://www.newae.com/chipwhisperer) - The ChipWhisperer® ecosystem presents the first open-source, low-cost solution to expose weaknesses that exist in embedded systems all around us
- [ChipSHOUTER Kit](https://www.newae.com/products/nae-cw520) - The ChipSHOUTER® (CW520) is a fully-featured Electromagnetic Fault Injection (EMFI) platform that can be used to discover and characterize vulnerabilities in embedded systems
- [ChipSHOUTER-PicoEMP Kit](https://store.newae.com/chipshouter-picoemp) - Little brother to the lab-grade, high performance ChipSHOUTER tool, our PicoEMP "Build Your Own" Kit is a low-cost Electromagnetic Fault Injection (EMFI) tool, designed specifically for self-study and hobbyist research
- [RP2040: Pico Glitcher](https://github.com/ZeusWPI/pico-glitcher) - Low-cost, Raspberry Pi Pico chip based voltage glitcher
- [ICEStick ICE40 FPGA Glitcher](https://github.com/SySS-Research/icestick-glitcher) - The iCEstick Glitcher is a simple voltage glitcher for a Lattice iCEstick Evaluation Kit

### Firmware Analysis and Exploit Frameworks
- [EMBA The security analyzer for firmware of embedded devices](https://github.com/e-m-b-a/emba) - EMBA is designed as the central firmware analysis tool for penetration testers and product security teams. It supports the complete security analysis process starting with firmware extraction, doing static analysis and dynamic analysis via emulation and finally generating a web report
- [Binwalk](https://github.com/ReFirmLabs/binwalk) - Binwalk is a fast, easy to use tool for analyzing, reverse engineering, and extracting firmware images
- [Unblob](https://github.com/onekey-sec/unblob) - Unblob is an accurate, fast, and easy-to-use extraction suite. It parses unknown binary blobs for more than 30 different archive, compression, and file-system formats, extracts their content recursively, and carves out unknown chunks that have not been accounted for
- [Panda.re](https://panda.re/) - PANDA is an open-source Platform for Architecture-Neutral Dynamic Analysis. It is built upon the QEMU whole system emulator, and so analyses have access to all code executing in the guest and all data. PANDA adds the ability to record and replay executions, enabling iterative, deep, whole system analyses
- [EXPLIoT Framework](https://gitlab.com/expliot_framework/expliot) - A Framework for security testing and exploiting IoT products and IoT infrastructure. It provides a set of plugins (test cases) which are used to perform the assessment and can be extended easily with new ones
- [RouterSploit](https://github.com/threat9/routersploit) - The RouterSploit Framework is an open-source exploitation framework dedicated to embedded devices
- [IoTSecFuzz(ISF)](https://gitlab.com/invuls/iot-projects/iotsecfuzz) - IoTSecFuzz(ISF) was created with the aim of combining the maximum number of utilities for comprehensive testing of IoT device security at all levels of implementation. It has a convenient console in order to use it as a stand-alone application, as well as the ability to import it as a library
- [HomePwn - Swiss Army Knife for Pentesting of IoT Devices](https://github.com/Telefonica/HomePWN) - HomePwn is a framework that provides features to audit and pentesting devices that company employees can use in their day-to-day work and inside the same working environment. It is designed to find devices in the home or office, take advantage of certain vulnerabilities to read or send data to those devices
- [QEMU](https://www.qemu.org/) - A generic and open source machine emulator and virtualizer

### Reverse Engineering
- [Ghidra](https://ghidra-sre.org/) - A software reverse engineering (SRE) suite of tools developed by NSA's Research Directorate in support of the Cybersecurity mission
- [IDA Pro](https://hex-rays.com/ida-pro/) - IDA Pro as a disassembler is capable of creating maps of their execution to show the binary instructions that are actually executed by the processor in a symbolic representation (assembly language)
- [Radare2](https://rada.re/n/radare2.html) - A free/libre toolchain for easing several low level tasks like forensics, software reverse engineering, exploiting, debugging
- [Cutter](https://cutter.re/) - An open-source GUI for Radare2 framework, Cutter's goal is to be an advanced FREE and open-source reverse-engineering platform while keeping the user experience at mind
- [GDB: The GNU Project Debugger](https://www.sourceware.org/gdb/) - GDB allows you to see what is going on inside another program while it executes or what another program was doing at the moment it crashed
- [x64dgb](https://x64dbg.com/) - An open-source x64/x32 debugger for windows

### Fuzzing
- [AFL++](https://github.com/AFLplusplus/AFLplusplus) - AFL++ is a superior fork to Google's AFL - more speed, more and better mutations, more and better instrumentation, custom module support
- [Boofuzz: Network Protocol Fuzzing for Humans](https://github.com/jtpereyda/boofuzz) - Boofuzz is a fork of and the successor to the venerable Sulley fuzzing framework. Besides numerous bug fixes, boofuzz aims for extensibility

## Penetration Test Use-Cases
- [Getting Root on Philips Hue Bridge 2.0 by Colin O'Flynn](https://colinoflynn.com/2016/07/getting-root-on-philips-hue-bridge-2-0/)
- [How I hacked a hardware crypto wallet and recovered $2 million by Joe Grand](https://youtu.be/dT9y-KQbqi4?si=k1Zwfd0KIZgRZb-j)
- [How the Apple AirTags were hacked by Thomas Roth](https://www.youtube.com/watch?v=_E0PWQvW-14)
- [Bosch Smart Home Hacks by Sebastien Leger](https://github.com/vegantransistor/BoschSmartHome)
- [Glitched on Earth by Humans: A Black-Box Security Evaluation of the SpaceX Starlink User Terminal by Lennert Wouters](https://www.youtube.com/watch?v=NXqLMmGwJm0)
- [SECGlitcher - Reproducible Voltage Glitching on STM32 Microcontrollers by SEC Consult](https://sec-consult.com/blog/detail/secglitcher-part-1-reproducible-voltage-glitching-on-stm32-microcontrollers/)
- [Fault Injection Attacks against the ESP32-C3 and ESP32-C6 by Kévin Courdesses](https://courk.cc/esp32-c3-c6-fault-injection)
- [Breaking the Flash Encryption Feature of Espressif’s Parts by Kévin Courdesses](https://courk.cc/breaking-flash-encryption-of-espressif-parts)

## Standarts and Regulations
- [ETSI EN 303 645 - Cyber Security for Consumer Internet of Things: Baseline Requirements](https://www.etsi.org/deliver/etsi_en/303600_303699/303645/02.01.00_30/en_303645v020100v.pdf) 
- [UK Code of Practice for Consumer IoT Security](https://www.gov.uk/government/publications/code-of-practice-for-consumer-iot-security)
- [EU Cyber Resilience Act](https://digital-strategy.ec.europa.eu/en/policies/cyber-resilience-act)
- [Radio Equipment Directive (RED)](https://eur-lex.europa.eu/eli/reg_del/2022/30/oj) - On the 12th January 2022, the European Commission updated the Radio Equipment Directive (RED), which establishes a regulatory framework for placing radio equipment on the market, to include additional legislation related to security (2022/30/EU)
- [USA IoT Cybersecurity Improvement Act of 2020](https://www.congress.gov/bill/116th-congress/house-bill/1668)
- [Common Criteria](https://www.commoncriteriaportal.org/index.cfm) - The Common Criteria for Information Technology Security Evaluation (CC) ensures that products can be evaluated by competent and independent licensed laboratories so as to determine the fulfilment of particular security properties, to a certain extent or assurance
- [NISTIR 8259: Recommendations for IoT Device Manufacturers: Foundational Activities](https://www.nist.gov/itl/applied-cybersecurity/nist-cybersecurity-iot-program/nistir-8259-series)
- [ARM PSA IoT Security Framework and Certification](https://www.psacertified.org/) - ARM PSA Certified is providing a common language for the industry, allowing the entire value chain to work to the same requirements. The PSA Certified framework offers a standardized approach from initial IoT security design and implementation to security evaluation
- [China CCRC: Implementation Rules on the Compulsory Certification of Information Technology Equipment](https://www.tuvsud.com/en/e-ssentials-newsletter/consumer-products-and-retail-essentials/e-ssentials-4-2023/china-implementation-rules-ccrc-c09-001-2022-for-compulsory-certification-of-it-equipment)
- [The C2 Consensus on CSDE - IoT Device Security Baseline Capabilities](https://csde.org/projects/c2-consensus/)
- [Digital Transformation Office of the Presidency of Türkiye - Information and Communication Security Guide(Türkiye Cumhurbaşkalığı Dijital Dönüşüm Ofisi - Bilgi ve İletişim Güvenliği Rehberi)](https://cbddo.gov.tr/bigrehber/)
- [Türkiye TR-Test Cyber Security Tests IoT Criterias(Türkiye TR-Test Siber Güvenlik Testleri IoT Kriterleri)](https://tr-test.com.tr/trtest/views/portalHeader/detay-56) - The criteria for cybersecurity in IoT products, developed through meetings and workshops involving the Presidency of Defense Industries, TRTEST, and participants from relevant IoT device manufacturers, laboratories, and academia, have been established based on ETSI 303 645
- [NIST Recommended Criteria for Cybersecurity Labeling for Consumer Internet of Things (IoT) Products](https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.02042022-2.pdf)
- [ISO/IEC 27402:2023 Cybersecurity — IoT security and privacy : Device baseline requirements](https://www.iso.org/obp/ui/#iso:std:iso-iec:27402:ed-1:v1:en)
- [Cybersecurity Labelling Scheme (CLS) by Cyber Security Agency of Singapore](https://www.csa.gov.sg/docs/default-source/our-programmes/certification-and-labelling-scheme/cls/publications/pub-cls-pub-2-scheme-specifications-v12.pdf?sfvrsn=27154727_0) - The cybersecurity label would provide an indication of the level of security in the network-connected smart devices. It aims to improve security awareness by making such provisions more transparent to consumers and empowers consumers to make informed purchasing decisions for products with better security using the information on the cybersecurity label
- [IASME IoT Cyber Baseline and Cyber Assurance](https://iasme.co.uk/internet-of-things/get-iot-cyber-assurance-level1/) - The IASME IoT Cyber Baseline and Cyber Assurance scheme certifies internet connected devices against the most important security controls and demonstrates commitment to best practice security
- [Finland’s National Consumer IoT Certification Scheme - The Finnish Cybersecurity Label(NCSC-FI)](https://tietoturvamerkki.fi/sites/default/files/media/file/cybersecurity_label_presentation-280920.pdf) - The label guarantees to consumers that the labelled devices have basic information security features. The Cybersecurity label can be awarded to networking smart devices if the devices meet the certification criteria, which are based on EN 303 645
- [Global Platform Security Evaluation Standard for IoT Platforms(SESIP)](https://globalplatform.org/sesip/) - GlobalPlatform is here to support IoT device makers and certification bodies to adopt the Security Evaluation Standard for IoT Platforms (SESIP) methodology and establish their own IoT device security certification schemes

## Books
- [Arm Assembly Internals and Reverse Engineering: Blue Fox Edition](https://www.wiley.com/en-be/Blue+Fox:+Arm+Assembly+Internals+and+Reverse+Engineering-p-9781119745303) - 2023, Publisher: Wiley, Author(s): Maria Markstedter aka Azeria
- [Practical Hardware Pentesting, Second edition](https://www.packtpub.com/product/practical-hardware-pentesting-second-edition-second-edition/9781803249322) - 2023, Publisher: Packt, Author(s): Jean-Georges Valle
- [Hardware Security Training, Hands-on!](https://link.springer.com/book/10.1007/978-3-031-31034-8) - 2023, Publisher: Springer, Author(s): Mark Tehranipoor, N. Nalla Anandakumar, Farimah Farahmandi
- [The Hardware Hacking Handbook: Breaking Embedded Security with Hardware Attacks](https://nostarch.com/hardwarehacking) - 2021, Publisher: No Starch Press, Author(s): Jasper van Woudenberg, Colin O'Flynn 
- [The Hacker's Hardware Toolkit: The best collection of hardware gadgets for red team hackers, pentesters and security researchers](https://github.com/yadox666/The-Hackers-Hardware-Toolkit/blob/master/TheHackersHardwareToolkit.pdf) - 2020, Publisher: N/A, Author(s): Yago Hansen
- [The IoT Hacker's Handbook: A Practical Guide to Hacking the Internet of Things](https://www.oreilly.com/library/view/the-iot-hackers/9781484243008/) - 2019, Publisher: Apress, Author(s):  Aditya Gupta
- [Hardware Security: A Hands-on Learning Approach](https://shop.elsevier.com/books/hardware-security/bhunia/978-0-12-812477-2) - 2018, Publisher: Morgan Kaufmann, Author(s): Swarup Bhunia, Mark M. Tehranipoor
- [IoT Penetration Testing Cookbook](https://www.packtpub.com/product/iot-penetration-testing-cookbook/9781787280571) - 2017, Publisher: Packt, Author(s): Aaron Guzman, Aditya Gupta

## Useful Websites
- [OWASP Embedded Application Security Project](https://owasp.org/www-project-embedded-application-security/) - Produces a document that will provide a detailed technical pathway for manufacturers to build secure devices for an increasingly insecure world.
- [OWASP Internet of Things Project](https://owasp.org/www-project-internet-of-things/) -  Is designed to help manufacturers, developers, and consumers better understand the security issues associated with the Internet of Things, and to enable users in any context to make better security decisions when building, deploying, or assessing IoT technologies.
- [ETSI Consumer IoT security](https://etsi.org/technologies/consumer-iot-security) - The Consumer IoT Security Road Map provides an overview of ETSI's world-leading work in consumer IoT security
- [Godbolt Compiler Explorer](https://godbolt.org/) - Online compiler for all purposes
- [Dogbolt Decompiler Explorer](https://dogbolt.org/) - Online decompiler for all purposes
- [Instruction Reference for x86 and amd64](https://www.felixcloutier.com/x86/index.html)
- [Hardware Hacking Lab Guide](https://voidstarsec.com/hw-hacking-lab/vss-lab-guide) - Beginners guide to building a hardware hacking Lab

## Youtube Channels
- [Colin O'Flynn](https://www.youtube.com/@ColinOFlynn)
- [Joe Grand aka kingpin](https://www.youtube.com/@JoeGrand)
- [stacksmashing](https://www.youtube.com/@stacksmashing)
- [LiveOverflow](https://www.youtube.com/@LiveOverflow)
- [hackaday](https://www.youtube.com/@hackaday)
- [GuidedHacking](https://www.youtube.com/@GuidedHacking)
- [RECESSIM](https://www.youtube.com/@RECESSIM)
- [IoTVillage](https://www.youtube.com/@IoTVillage)

## Twitter Accounts
- [Xeno Kovah](https://twitter.com/XenoKovah)
- [LiveOverflow](https://twitter.com/LiveOverflow)
- [Colin O'Flynn](https://twitter.com/colinoflynn)
- [Hash](https://twitter.com/BitBangingBytes)
- [Cesar Cerrudo](https://twitter.com/cesarcer)
- [stacksmashing](https://twitter.com/ghidraninja)
- [Ken Munro](https://twitter.com/TheKenMunroShow)
- [Travis Goodspeed](https://twitter.com/travisgoodspeed)
- [Michael Ossmann](https://twitter.com/michaelossmann)
- [Azeria](https://twitter.com/Fox0x01)
- [Cybergibbons](https://twitter.com/cybergibbons)
- [Slawomir Jasek](https://twitter.com/slawekja)
- [Aseem Jakhar](https://twitter.com/aseemjakhar)
- [Kate Temkin](https://twitter.com/ktemkin)
- [Joe Fitz](https://twitter.com/securelyfitz)
- [Stephen A. Ridley](https://twitter.com/s7ephen)
- [Charlie Miller](https://twitter.com/0xcharlie)
- [Samy Kamkar](https://twitter.com/samykamkar)
- [/dev/ttyS0](https://twitter.com/devttyS0)

## Blogs
-  [Cybergibbons](https://cybergibbons.com/)
-  [Hackaday](https://hackaday.com/)
-  [VoidStar Security Research and Blog Wiki](https://voidstarsec.com/hw-hacking-lab/) - Wiki articles on hardware hacking and other hardware security related content
-  [Riscure's Blog](https://www.riscure.com/blog/)
-  [Quarkslab's Blog](https://blog.quarkslab.com/)
-  [SRLabs' Blog](https://www.srlabs.de/blog)

## Trainings
- [OpenSecurityTraining2](https://ost2.fyi/) - OpenSecurityTraining2's mission is to provide the world's deepest and best cybersecurity training
- [Cyberpath: Practical IoT Hacking](https://cyberpath.training/) - Hands-on IoT hacking training
- [Hextree.io](https://www.hextree.io/) - Introduction to hardware hacking training
- [Attify Offensive IoT Exploitation](https://www.attify-store.com/collections/training) - Offensive IoT Exploitation
- [Introduction to Reverse Engineering with Ghidra](https://hackaday.io/course/172292-introduction-to-reverse-engineering-with-ghidra) - Learn how to reverse engineer software using Ghidra! This four-session course will walk you through the basics.

## Conferences
- [Hardwear.io Security Trainings and Conference](https://hardwear.io/)
- [HITB Security Conference](https://conference.hitb.org/)
- [IoT Security Foundation Conference](https://iotsecurityfoundation.org/conference/)
- [COSADE: Constructive Side-Channel Analysis and Secure Design](https://www.cosade.org/cosade24/)
- [HASP Hardware and Architectural Support for Security and Privacy Workshop](https://haspworkshop.org/)
- [SILM Security of Software/Hardware Interfaces Workshop](https://silm-workshop.github.io/)

## Awesome Lists
- [TEE Reversing](https://github.com/enovella/TEE-reversing) - A curated list of public TEE resources for learning how to reverse-engineer and achieve trusted code execution on ARM devices
- [A Collection for IoT Security Resources](https://github.com/V33RU/IoTSecurity101) - A Curated list of IoT Security Resources
- [Awesome Bluetooth Security (BR, EDR, LE, and Mesh)](https://github.com/engn33r/awesome-bluetooth-security)
  
