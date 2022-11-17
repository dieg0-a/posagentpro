# POS Agent PRO
## Motivation

If you came to this site it's probably because you're aware of the excellent POS (Point of Sale) interface featured
in the Odoo (Open Source ERP/CRM) suite.
Now there's a drawback to this solution, and it lies in the fact that since it is a javascript application running in a browser
sandbox, there's no built-in way to interface with traditional point of sale hardware devices, namely, receipt printers,
cash drawers, electronic scales, customer facing screens, etc.
Instead, Odoo offers a paid, subscription based addon, which includes a physical box (IoTBOx), essentially a Raspberry PI
running a secondary version of the Odoo backend to interface with the hardware. Furthermore, this is only available for
the enterprise edition of Odoo.

This project aims to provide a software alternative to this IoTBox, that works for Community Edition and runs on desktop OS's
such that it interfaces with the devices that are connected directly to your Desktop computer.

Currently, only ESC/POS receipt printers and Cash Drawers are supported, but in the near future support for other devices
is planned (Scales, and, based on demand, Customer facing screens).

**What is Currently supported**

Windows 10/11

Thermal ESC/POS Printers (Windows printer driver) mainly USB printers

Cash Drawers

**What is currently not supported but might be supported very soon**

STAR Printers

Linux

Older Windows Versions/32 bit

Electronic Scales

More printer drivers (Windows serial port, TCP/IP (network))

Enhanced printer output, filters

Text mode (this would result in immensely better print quality), currently Odoo sends an image file to the IoTBox

**What might be supported in the future, if there's enough demand for it**

Enterprise Edition

**Is this program free?**

You can freely download and use this tool, however it'll run in demo mode unless you purchase and install the corresponding
Odoo server addon listed in the Odoo App Store. I do this to support this project and be able to continue working on it.

**Will you make a free/open source version?**

Maybe, if you help me by buying enough copies of my Module :)
Meanwhile you can take advantage of the convenience of direct-printing and other IoTBox features for a price that beats the
official solution and other competing approaches.

**What can I do in demo mode**

You can print one receipt normally then it'll print diagonal stripes on it, with the Legend "DEMO" on them.

**Features**

Very fast and lightweight, made in native C++

Very easy to set up, you only need to configure it once and it'll remember your settings and printer

Silent, unintrusive, can run and start in the system tray

Demo mode, you can test it in an unmodified Community Edition Odoo server

**Basic Usage for Windows**

**General Settings Tab**

![The General Settings Page](/assets/images/windows2.png)

From this tab you can adjust the network proxy port, be sure it matches the setting in Odoo, if you change it click Restart Network for it to take effect
You can also enable start minimized (run in the system tray) mode.

**The Printer Settings Page**

![The Printer Settings Page](/assets/images/windows1.png)

In this screen you can configure your printer, select their printer in the "Name" dropdown menu and click Set

Adjust the width in pixels to match that of your printer, typically 80mm printers are 576 pixels wide and 58mm printers are 384 pixels wide.
You can also enable or disable paper cutter and cash drawer.
Finally there's a setting for adding a set amount of lines at the end of the print job, useful for getting the paper to roll to the cut position.

**Setting up Odoo**

Just set up your server as such, use IP 127.0.0.1 if you're going to run PosAgent PRO from the same computer as the browser (most likely scenario) and use the same port you chose in network settings

![Odoo POS Configuration 1](/assets/images/odoo1.png)
![Odoo POS Configuration 2](/assets/images/odoo1.png)


**Contact**

diegoandino@gmail.com

Copyright © 2022 All rights reserved.
