![Logo](admin/vaillant.png)

# ioBroker.vaillant

[![NPM version](http://img.shields.io/npm/v/iobroker.vaillant.svg)](https://www.npmjs.com/package/iobroker.vaillant)
[![Downloads](https://img.shields.io/npm/dm/iobroker.vaillant.svg)](https://www.npmjs.com/package/iobroker.vaillant)
![Number of Installations (latest)](http://iobroker.live/badges/vaillant-installed.svg)
![Number of Installations (stable)](http://iobroker.live/badges/vaillant-stable.svg)
[![Dependency Status](https://img.shields.io/david/TA2k/iobroker.vaillant.svg)](https://david-dm.org/TA2k/iobroker.vaillant)
[![Known Vulnerabilities](https://snyk.io/test/github/TA2k/ioBroker.vaillant/badge.svg)](https://snyk.io/test/github/TA2k/ioBroker.vaillant)

[![NPM](https://nodei.co/npm/iobroker.vaillant.png?downloads=true)](https://nodei.co/npm/iobroker.vaillant/)

## vaillant adapter for ioBroker

Vaillant multiMatic VR900/VR920 Adapter

### Getting started
In den Instanzoptionen mail und password der multimatic /senso  app eingeben.

Configuration können geändert werde in dem sie unter dem Unterpunkt configuration angepasst werden. Manche configuration werden erst angewendet wenn der Modus auf ON oder MANUAL ist und nicht AUTO oder TIME_CONTROLLED

## **Beispiel:**
**Warmwasser**: vaillant.0.serialnummer.systemcontrol/tli.dhw.hotwater.configuration.hotwater_temperature_setpoint
**Heizung**:
Erst auf MANUELL
vaillant.0.serialnummber.systemcontrol/tli.zones03.heating.configuration.operation_mode
MANUELL
Dann die Temperatur
vaillant.0.serial.systemcontrol/tli.zones03.heating.configuration.manual_mode_temperature_setpoint
Und am Ende operation_mode auf TIME_CONTROLLED

Parameter können über den Punkt parameterValue angepasst werden dabei beachten welche Werte im Objekt definition erlaubt sind.

## Changelog
### 0.0.15

-   bugfixes
### 0.0.14

-   add rooms support
### 0.0.13

-   fix livereport order
### 0.0.11

-   fix issue with js-controller 3.2
### 0.0.10

-   fix issue with js-controller 3

### 0.0.8

-   (TA2k) Fix Authorization problem and missing configuration states

### 0.0.6

-   (TA2k) initial release

## License

MIT License

Copyright (c) 2020 TA2k <tombox2020@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
