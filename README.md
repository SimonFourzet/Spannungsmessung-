# Spannungsmessung-
Der Code verbindet einen ESP8266 mit dem lokalen WLan und dem Mosquitto-Broker auf dem Raspi in diesem WLan
Dazu wird ein Topic gesetzt, für das der Raspi unterschrieben hat (subscribe)
Der Code misst eine Spannung am Eingang A0 des ESP8266 und nutzt einen Kalibrierungsfaktor, um Widerstandstoleranzen und Messfehler im ADC-Wandler des ESP8266 zu minimieren.
Die Referenz ist ein hohcpräzises Labormessgerät
Der Kalibrierungsfaktor muss für jede neue Umsetzung des Projekts individuell ermittelt werden.

Der Node-Red-Flow wertet auch die Daten einen DHT22 aus, da eines der Breadboards auch diesen Sensor enthält. Damit wird geprüft, ob die von den Ballastwiderständen erzeugte Hitze die Schaltung gefährdet und ob die Box trocken geblieben ist. Diese Kontrolldaten werdern im Video nicht erwähnt.
