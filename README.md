# Lora-TTN-Vegawell52-Water-level-meter
LORA Vegawell52 with Ursalink UC11-N1 868MHz

Hardware
Sensor: Vegawell 52
Node: Ursalink UC11-N1 868MHz
Netzteil: Omron S8VK-C12024

Vorbereitungen:

Node vorbereiten
Einstellen AI2 input = 4-20mA
Einstellen Vout Interface2 = 12 Volt

Spannungsversorgung Kabel anschließen
Spannungsversorgung Node UC11-N1   Standard M12/4 Kabel
Ansicht Stecker vom Node
Pin 1 = GND (-)
Pin 2 = USB D+
Pin 3 = USB D-
Pin 4 = VCC (5-24 Volt DC)
--------------------------
Kabel (Standard Sensor Kabel M12/4 (Buchse wird benötigt)
1 = weiss
2 = blau
3 = schwarz
4 = braun

damit wird der Node angeschlossen am Netzteil mit
braun = GND
weiss = 24 VDC

Sensor Vegawell anschließen
blau   = Signal 4-20mA
braun  = VDC+
shield = GND

damit ergeben sich für das Kabel zum Node
blau vom Sensor wird gürn zum Node
braun vom Sensor wird orange zum Node
shield vom Sensorkabel wird schwarz zum Node

der Node wird per mitgelieferten USB Kabel am PC eingerichtet, dafür benötigt man die Software URSALINK Toolbox in der aktuellen Version
die erstmalige Einrichtung und Anbindung in eine TTN Application ist sehr gut in der Bedienungsanleitung vom Node beschrieben

Nach der Einrichtung wird der NOde mit dem Netzteil betrieben, damit auch der Sensor mit ausreichend Spannung (12 Volt) versorgt werden kann

Die Umrechnung der Stromstärke in Wassertiefe ist einfach und wird nach folgenden Überlegungen gemacht:
