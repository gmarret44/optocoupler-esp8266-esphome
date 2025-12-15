# optocoupler-esp8266-esphome
how to use an optocoupler as a relay with an esp8266 in esphome.


The advantage of optocouplers is that they are much smaller and cheaper than relays. I recommend the 4n37, which are quite robust.
First, you need to assemble the circuit shown below. The LED requires a voltage of 1.2V. The GPIO ports on the ESP8266 provide 3.3V. Once the calculation has been made, this gives us a resistance of 390 ohms. Be careful, the voltage passing through the optocoupler must not exceed 30V! (Otherwise, you will need a real relay).

![4n37](https://github.com/user-attachments/assets/ca3c7680-a1ee-4087-a4e1-70528c6e7655)



Then flash the ESP with the YAML code in the file. You now have a functional 30V relay.


