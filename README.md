# python-arduino

import pyanexo

retardo = 1
puerto = pyanexo.Arduino.AUTODETECT
placa = pyanexo.Arduino(puerto)

while True:
        placa.digital[1].write(1)
        placa.pass_time(retardo)
        placa.digital[1].write(0)
        placa.pass_time(retardo)
