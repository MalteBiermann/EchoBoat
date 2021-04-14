Dieses Repository ist in Bearbeitung! // Work in progress!
===
# EchoBoat Dokumentation
Ein manuell gesteuertes USV wird zu einem autonomen Fahrzeug (ASV) für bathymetrische Aufgaben umgerüstet. Das Seafloor Echoboat-160 ist eine Multi-Sensor Plattform für Bathymetrie / Gewässervermessung. Dieses Projekt ist eine Darstellung der Systeme und Peripherie des Echoboats und dazugehöriger Anleitungen und Beschreibungen. Im Rahmen der Praxisphase des Studiums der angewandten Geodäsie an der Jade HS Oldenburg.
![Echoboat](./img/echoboat3.jpg)
## Inhalt
### Pläne
- Übersichtsplan
- Steuerung
- Sensoren
### Beschreibungen
#### Komponenten
- Steuerung
    - FrySky Empfänger (Transmitter)
    - Holybro Pixhawk 4
- Antrieb
    - Holybro Power Module PM02 (2*)
    - ESC (2*)
    - Motore Bluerov Thruster T100 (2*)
- Energie
    - LiPo 4S1P 14000mAh (2*2) Turnigy für Antrieb
    - LiPo 6S1P 22000mAh (2*) Venom für Vermessung
- Sensoren
    - Lidar (???)
    - ODOM Einstrahl-Echolot
    - SBG Ellipse IMU
    - Leica GNSS GS15
    - Leica GNSS Controller
    - Webcam Logitech C270
- Industrie-PC
- An Land
    - FrSky Fernsteuerung
    - Wlan-Antenne Mikrotik
    - Laptop
- Lade-Segment
    - ISDT P30
    - ISDT SP3060
    - ISDT FD-200

### Anleitungen
## Danksagung
Vielen Dank für die eingeräumten Freiheiten, das Feedback und die praktische und technische Unterstützung an 
- Harry Wirth,
- Thorsten Roelfs, 
- Stefan Scheidweiler und 
- Tobias Berndt. 

## Links
## Lizenz
Der vollständige Lizenztext befindet sich in [LICENSE][1].
```
Copyright (C) 2020 - 2021 Malte Biermann

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
```
[1]: https://github.com/MalteBiermann/EchoBoat/LICENSE