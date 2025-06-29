# Boot Methods Best Practices

> This document explains various methods to boot a computer, especially when the normal startup process fails or when you want to use a different operating system.

## The Boot Process

- When powered on, the BIOS/UEFI runs diagnostics and selects a boot device based on a configured boot order.

- The BIOS searches for a bootloader on attached devices (hard drives, USB, CD, etc.) and executes it to load the OS.

## Configuring Boot Options

- Enter the BIOS/UEFI during startup (using keys like DEL, F2, F12, or Option for macOS) to set the boot order.

- The boot order determines which device is checked first for a bootloader

## Boot Method Options

### External Options

- USB Drive: Boot from a USB with a bootable OS.
- Optical Media: Boot from a CD, DVD, or Blu-ray with boot resources.
- Solid State Boot Drive: Boot from an internal or external SSD.
- External Hot-swappable Drive: Boot from a removable external hard drive.
- Network Boot: Boot from a local network using PXE, useful when no OS is installed.
- Internet-based Boot: Boot from an internet source, useful for remote server management Can use:
    - Remote Access Controller (IPMI/IDRAC): Requires BIOS support and hardware.
    - Wake on LAN (WoL): Requires BIOS and network card support.

### Internal Options

- Disk Partitions: Partition a drive to run different operating systems (dual booting). Useful for troubleshooting if one OS fails.

## Quick Reference Table

| **Boot Method**         | **Description/Use Case**                                      |
|-------------------------|---------------------------------------------------------------|
| USB Drive               | Boot from USB, useful for recovery or alternate OS            |
| Optical Media           | Boot from CD/DVD/Blu-ray, for recovery or install             |
| SSD                     | Boot from solid state drive, internal or external             |
| Hot-swappable Drive     | Boot from removable external hard drive                       |
| Network Boot (PXE)      | Boot from LAN, often for OS-less systems                      |
| Internet-based Boot     | Remote boot, server management (IPMI, WoL)                    |
| Disk Partitions         | Dual boot multiple OSes on one drive                          |
