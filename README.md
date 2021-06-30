Hola,
Soy estudiande de Ing. Civil en Informática en la Universidad De Los Lagos (2016-Presente):bowtie:.

```python
# yo.py

import datetime 
import sys


class Persona:
    def __init__(self, nombre, apellido, fecha_nacimiento, ciudad, email):
        self._nombre = nombre
        self._apellido = apellido
        self._fn = datetime.date.fromisoformat(fecha_nacimiento)
        self._ciudad = ciudad
        self._email = email

    @property    
    def edad(self):
        hoy = datetime.date.today()
        edad = hoy.year - self._fn.year     
        if hoy < datetime.date(hoy.year, self._fn.month, self._fn.day):
            edad -= 1
        return edad
        
    def __str__(self):
        evpo = ["Nombre: ", "Apellido: ", "Ciudad: ", "eMail: "]
        vi = [self._nombre, self._apellido, self._ciudad, self._email]
        imprimir = "Mis datos: "
        for i, x in zip(evpo, vi):
            imprimir += ("\n" + i + x)
        return imprimir  
        

def main():
    yo = Persona(sys.argv[1], sys.argv[2], sys.argv[3], sys.argv[4],
                 sys.argv[5]) 
    print(yo)
    print("Edad: " + str(yo.edad))


if __name__ == "__main__":
    main()

```
```shell
$ python3 yo.py "Juan Pablo" "Nahuelpán" "1991-06-25" "Osorno" "juanpablonahuelpan@gmail.com"
Mis datos: 
Nombre: Juan Pablo
Apellido: Nahuelpán
Ciudad: Osorno
eMail: juanpablonahuelpan@gmail.com
Edad: 30
$
```
# Estadísticas
<p>
<a href="https://github.com/jpnahuelpan">
  <img height="150em" src="https://github-readme-stats.vercel.app/api?username=jpnahuelpan&show_icons=true&theme=flag-india" />
  <img height="150em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=jpnahuelpan&theme=flag-india&layout=compact" />
</a>
</p>

<!---
jpnahuelpan/jpnahuelpan is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
