
Dada los problemas de librerías y  versiones de PY se diseño los entornos virtuales, una forma de mantener entornos de Py aislados.

un entorno virtual se compone del interprete y la librerías requeridas para ele programa asegurándose que la instalación de cualquier paquete no afecte a el sistema operativo 


Pip tiene  Herramientas que ayudan a gestionar decencias 


```python
pip freeze > requirements.txt
pip install -U -r requirements.txt
```

El comando freeze guarda la salida en un fichero  para después poder instalar las mismas dependencias de manera automática utilizando las opciones -r y -U

## venv

venv es un módulo de Python que permite crear entornos virtuales para aislar versiones de Python y bibliotecas de software. 
Venv es útil para: 

    - Aislar dependencias específicas de un proyecto
    - Evitar que actualizaciones de paquetes rompan códigos
    - Prevenir conflictos de dependencia
    - Permitir la reproducibilidad
    - Instalar y administrar diferentes versiones de Python
    - Instalar bibliotecas y dependencias para cada proyecto 

Venv se incluye en la biblioteca estándar de Python y no requiere una instalación independiente. 
Algunas características de venv son: 

    -Crea entornos virtuales ligeros
    -Tiene sus propios directorios de ubicación
    -Puede aislarse opcionalmente de los directorios de ubicación del sistema
    -Cada entorno virtual tiene su propio binario Python
    -Puede tener su propio conjunto independiente de paquetes Python instalados


**Comandados mas usados:** 

crear un entorno virtual

```python

python -m venv nombre_del_entorno

```

activar entorno virtual
```python 
source nombre_del_entorno/bin/activate

```

