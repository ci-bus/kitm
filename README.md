# Keyboard-In-The-Middle

The project is a proof of concept of utilizing the vulnerability of a [man-in-the-middle attack](https://en.wikipedia.org/wiki/Man-in-the-middle_attack), by impersonating a BLE keyboard and control all traffic in between using Texas Instruments [CC-2650 LP](http://www.ti.com/tool/launchxl-cc2650) evaluation boards.
Submitted by Mattan Serry, Sharon Lifshits and Hila Balahsan as a final project in the [Advanced Computer Systems](https://sivantoledoacademic.wordpress.com/teaching/advanced-computer-systems-fall-2017/) course, The Computer Science Master's Program, Tel-Aviv University, 2018.

![CC-2650 LP](http://www.ti.com/diagrams/med_launchxl-cc2650_launchxl-cc2650.jpg)

Requirements:

1. [Code Composer Studio 7.4.0](http://processors.wiki.ti.com/index.php/Download_CCS#Code_Composer_Studio_Version_7_Downloads) and [BLE SDK 2.02.01.18](http://www.ti.com/tool/ble-stack) with [these modifications](https://github.com/mattans/kitm/tree/master/code/ble_sdk_2_02_01_18/src).
2. CC-2650 LP board running the [Simple Central](https://github.com/ti-simplelink/ble_examples/tree/ble_examples-2.2/examples/cc2650lp/simple_central) application with [these modifications](https://github.com/mattans/kitm/tree/master/code/ble_examples-ble_examples-2.2/src/examples/simple_central/cc26xx/app), acting as fake computer.
3. CC-2650 LP board running the [HID Emu Kbd](https://github.com/ti-simplelink/ble_examples/tree/ble_examples-2.2/examples/cc2650lp/hid_emu_kbd) application with [these modifications](https://github.com/mattans/kitm/tree/master/code/ble_examples-ble_examples-2.2/src/examples/hid_emu_kbd/cc26xx/app), acting as fake keyboard.

Detailed walkthorugh and project presentation can be found [here](https://github.com/mattans/kitm/blob/master/KeyboardInTheMiddle.pdf).

## License:

The original BLE SDK is copyrighted under the [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause) license:
> Copyright (C) 2016 Texas Instruments Incorporated - http://www.ti.com/
Furthermore, every source file begins with a copyrights decleration. 

Our modifications are also under the BSD-3-Clause. If you distribute our source code, please retain all copyrights and licensing information.
