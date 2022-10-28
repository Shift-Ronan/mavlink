[![Build Status](https://github.com/ArduPilot/mavlink/workflows/Test%20and%20deploy/badge.svg)](https://github.com/ArduPilot/mavlink/actions?query=branch%3Amaster)

> MAVLink Relay Script (mav_link_relay.py) is in the root folder of this project: https://github.com/Shift-Environmental/shift-platform

## MAVLink ##

MAVLink -- Micro Air Vehicle Message Marshalling Library.

MAVLink is a very lightweight, header-only message library for communication between drones and/or ground control stations. It consists primarily of message-set specifications for different systems ("dialects") defined in XML files, and Python tools that convert these into appropriate source code for [supported languages](https://mavlink.io/en/#supported_languages). There are additional Python scripts providing examples and utilities for working with MAVLink data.

> **Tip** MAVLink is very well suited for applications with very limited communication bandwidth. Its reference implementation in C is highly optimized for resource-constrained systems with limited RAM and flash memory. It is field-proven and deployed in many products where it serves as interoperability interface between components of different manufacturers.

Key Links:
* Development Website: https://ardupilot.org/dev/
* Source: [Mavlink Generator](https://github.com/ArduPilot/pymavlink)
* Discussion: [Discord Mavlink Channel](https://discord.com/channels/674039678562861068/728017546313466047)
* Discussion: [Discord pymavlink Channel](https://discord.com/channels/674039678562861068/930641827592306718)
* [Documentation/Website](https://mavlink.io/en/) (mavlink.io/en/)
* [Discussion/Support](https://mavlink.io/en/#support) (Slack)
* [Contributing](https://mavlink.io/en/contributing/contributing.html)

## Building MAVLink ##
To run the Python examples and take advantage of the pymavlink, it has to be built.<br>
1. Follow the docs for generating a custom dialect: [mavlink.io](https://mavlink.io/en/mavgen_python/#generate-a-custom-mavlink-dialect)
2. Add the path to the pymavlink library's root directory to the PYTHONPATH system environment variable. (Create the environment variable if it doesn't exist)

For C++ the CPLUS_INCLUDE_PATH environment variable should include the path to the generated header files.

### License ###

MAVLink is licensed under the terms of the Lesser General Public License (version 3) of the Free Software Foundation (LGPLv3). The C-language version of MAVLink is a header-only library which is generated as MIT-licensed code. MAVLink can therefore be used without limits in any closed-source application without publishing the source code of the closed-source application.

See the *COPYING* file for more info.
