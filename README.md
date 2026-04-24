Custom Modded BIOS Repository

This repository hosts customized BIOS firmware files designed to unlock advanced hardware functionality, remove vendor-imposed restrictions, and improve system privacy. These modifications are intended for power users and enthusiasts looking to extend the capabilities of workstation and desktop hardware.

Dell Precision Tower 7910

File: T7910-unlocked-rebar.bin

Modifications

Resizable BAR (ReBar) Enabled: Patched to support Resizable BAR, allowing the CPU full access to the GPU frame buffer for improved performance in modern graphical workloads.

Flash Lock Removal: Region locks and write protections have been removed to allow for easier firmware management and descriptor overrides.

Intel Management Engine (ME) Disabled: The Intel ME has been neutralized and disabled.

Flashing Instructions

[!CAUTION]

FLASH AT YOUR OWN RISK. Modding BIOS firmware is a high-risk operation that can result in a permanent brick of your motherboard. This software is provided "as-is" without any warranty or guarantee of functionality.

Initial Flash (External)

For the transition from stock firmware to modded firmware, you must use an external hardware programmer.


Software: Use flashrom on a Linux-based system.

Power Note: External programmers typically do not provide sufficient current to power the chipset. You must perform the flash with the machine plugged into AC power but in a powered-off state.


Subsequent Flashes (Internal)

Once the modded BIOS is installed and the flash locks are removed, future updates can be performed directly from the host machine using flashrom within Linux.

Credits
UEFITool by CodeRush

ReBarState by xander-mamba

me_cleaner for Intel ME neutralization
