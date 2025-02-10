Documentacion e instalacion en windows de Python:
WINDOWS
Descargar el instalador de Python desde https://www.python.org/

Ejecutar el instalador y marcar la opcion de "Add Python to PATH"

Verificar version con: "python --version" en la terminal

Verificar si pip esta instalado: "pip --version"

Si no se instalo usa: " python -m pip install"

LINUX
Instalacion python
"sudo apt update && sudo apt install python3 -y

Verificar instalacion : "python3 --version"

verificar pip instalado : " pip3 --version"





Creacion y Activacion de un Entorno Vitual:

Para crear un entorno creamos una carpeta donde instalarlo desde el terminal o en tu entorno de desarrollo

Para crearlo usamos en windows: "python -m venv "nombre-entorno" "
Para crearlo usamos en linux: "python3 -m venv "nombre-entorno" "

Para activarlo usamos: " "nombre-entorno"\Scripts\activate "
Para activarlo usamos: " source "nombre-entorno"/bin/activate "

Para desactivar el comando: "deactivate"


Instalacion de dependencias:

Dentro de nuestro entorno activado instalamos el PySide6
"pip install PySide6"



Creacion de la aplicacion Hola Mundo
Creamos un main.py y con el codigo para mostrar una ventana "hola mundo"
```python
import sys
from PySide6.QtWidgets import QApplication, QLabel

app = QApplication(sys.argv)
window = QLabel("Hola Mundo")
window.show()
sys.exit(app.exec())
```
Ejecutar la aplicacion

Usamos el comando python main.py en windows
Usamos el comando python3 main.py en Linux




