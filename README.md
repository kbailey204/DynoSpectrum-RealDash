# DynoSpectrum-RealDash
Configuration and setup instructions for connecting RealDash to the DynoSpectrum DS1 TCP server.

# Description
Among many of the features added by the DynoSpectrum DS1, one of those features is a TCP server broadcast via the DS1 wifi on port 9996. The initial purpose of this server was to feed data to the browser included gauges. This was expanded via later updates to mirror the entire powertrain CAN bus data across the TCP server.

# Requirements
A vehicle flashed with the DynoSpectrum DS1. At the time of this writing, the current platforms are as follows:
- C7 Platform (2012-2017 S6/S7/RS7)
- D4 Platform (2012-2018 A8/S8/S8+)
- 8V Platform RS3 (2013- ***FURTHER WORK IS NEEDED***)
- MK3 Platform TT RS (2016- ***FURTHER WORK IS NEEDED***)
- 8U Platform RS Q3 (2015- ***FURTHER WORK IS NEEDED***)

DS1 software:
- OBD - 1641-g999ed3467 or newer
- Factory - 1634-g551fb882c or newer

A device capable of running RealDash (Android, IOS, and Windows 10).

# Installation
Installation of the RealDash software should be faily straightforward. Any issues should be directed here: [RealDash Forums](https://www.realdash.net/forum/)

# Configuration
The decoding of raw CAN data is possible due to the [RealDash CAN protocol](https://github.com/janimm/RealDash-extras/blob/master/RealDash-CAN/realdash-can-protocol.md). Writing of the XML file used is based on DBC files that define the data structure, information, and conversion math involved for extracting CAN data into readable information.
