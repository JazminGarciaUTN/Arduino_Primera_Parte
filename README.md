# ♾️ Arduino Primera Parte ♾️
![pc17](https://github.com/JazminGarciaUTN/Arduino_Primera_Parte/assets/123723038/8ba8486c-bb16-4676-ae9f-7377216a77f1)

# 👥 INTEGRANTES:
- Garcia Jazmín
- Levy Santiago

# 🔢 PROYECTO: Contador
![Smooth Amberis-Hillar](https://github.com/JazminGarciaUTN/Arduino_Primera_Parte/assets/123723038/aa16dec2-f350-4c51-a9c9-39341c42c36c)

# DESCRIPCIÓN :
Este proyecto consta de dos display de 7 segmentos que funcionarán como contadores en los que se podrá interactuar por medio de botones subiendo o bajando los números entre 0 y 99, al igual que la opción de resetearlos y volver a 0 si así lo desea.

# FUNCIÓN PRINCIPAL: 
Enciende y apaga de manera sincrónica los display para que se actualicen los números y sea visible al ojo humano.
~~~ C
// -------- ENCIENDO LOS DISPLAY -------
void prendeDigito(int digito)
{
  if(digito == UNIDAD)
  {
  	digitalWrite(UNIDAD, HIGH);
    digitalWrite(DECENA, LOW);
    delay(DELAY);
  }
  else if(digito == DECENA)
  {
    digitalWrite(UNIDAD, LOW);
    digitalWrite(DECENA, HIGH);
    delay(DELAY);
  }
  else
  {
  	digitalWrite(UNIDAD, HIGH);
    digitalWrite(DECENA, HIGH);
    delay(DELAY);
  }  
}
~~~
# 🖇️ LINK DEL PROYECTO:
- [PROYECTO](https://www.tinkercad.com/things/2rwoUAirYrQ-smooth-amberis-hillar/editel?sharecode=Q74UVF8LYI02YmwaxbSn2L-J8bWsNQjCkKLJrrmFOMg)
#
