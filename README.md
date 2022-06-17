BKM-68X Alternative HV Sync Add-on

This small experimental board is meant to wired to the BKM-68X Alternative Rev. E1 (or earlier that has the HD_SD_X pad) to
provide a discrete VSYNC input, and thus support RGBHV signals. The FPGA needs to be programmed with at least version 1.3 of
the firmware, and using the Quartus project where the HD_SD_X pin has been reconfigured to discrete VSYNC in.

Since the board cannot easily be soldered and fastened to the BKM-68X Alternative board, it is meant to be fastened to the
bracket, so the bracket needs to be replaced with bracket that has the appropriate hole. The Keystone 7794 is not mandatory
but will provide further support of the board if used. The BNC jack needs to be rather low profile to avoid the THT pins
touching the board, seemingly the Molex 73171-0702 is appropriate.

The board needs 5 connections, two going to the "analog part" of the board, that being the 5V and GNDA, two going to the
"digital part" being 3.3V and GND. FPGA SYNC pad then needs to be wired to the HD_SD_X pad. As the VSYNC signal is rather
low speed (so 50/60Hz) routing/wiring shouldn't be extremely important, but try to keep the wire close to the "digital"
ground part. C103 is as such optional, if chosen it should most likely be in the 1nF range. It is there to help the return
path of the signals.

Use at your own risk, very untested :)

(2022) Martin Hejnfelt (martin@hejnfelt.com)
www.immerhax.com 

