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

**What is currently not supported but might be supported be very soon**

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

**Basic Usage for Windows**

