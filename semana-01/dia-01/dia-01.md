# Día 01 - DevOps y la Importancia de Linux

## 1. 🧠 Reflexión personal: ¿Qué significa DevOps para mi?

Es una cultura que une dos mundos: desarrolladores y operadores, con el objetivo de trabajar juntos desde un inicio, para crear sistemas más rápidos, estables y eficientes.

### Beneficios clave de DevOps:

* 🚀 Entregas más rápidas gracias a la automatización.
* 🧪 Mejor calidad con pruebas continuas (reducción de bugs).
* 📉 Mayor estabilidad con monitoreo constante (menos caídas).
* 💡 Más innovación por ciclos cortos de desarrollo (se puede experimentar sin preocupaciones).
* 🤝 Mejor colaboración entre equipos (se comparten responsabilidades).

### ¿Por qué Linux es esencial en DevOps?

Linux es la base de la mayoría de herramientas y servidores en entornos DevOps. Su dominio se debe a que:

* Es el sistema preferido en la nube (AWS, Azure, Google Cloud).
* Funciona mejor con herramientas clave: Docker, Kubernetes, Jenkins, Ansible, etc.
* Permite una automatización poderosa con Bash y comandos de terminal.
* Brinda alto nivel de seguridad.
* Es el entorno natural de los contenedores y la infraestructura como código.

Se debe destacar que **todo ingeniero DevOps debe aprender Linux**, ya que gran parte del trabajo se hace desde la terminal, automatizando procesos, gestionando servidores y desplegando contenedores.

### Herramientas DevOps

* **Conocidas (había oido hablar de ellas)**
    * Docker
    * Jenkins
    * Terraform
* **Nuevas para mi**
    * Kubernetes
    * Ansible

## 2. 🖥️ Primeros Pasos en Linux

### Herramientas utilizados:
* VirtualBox Ver. 7.1.10 → Software de Virtualización
* Linux Ubuntu Server 24.04 LTS → Sistema Operativo
* MobaXterm Ver. 23.6 → Software multiprotocolo para acceso remoto (en este caso SSH)

En virtualBox creé una máquina virtual (MV) con 2 GB de memoria RAM, 2 núcleos de procesamiento y almacenamiento de 25 GB e instalé el sistema operativo Linux Ubuntu Server 24.04 LTS.

* Configuración virtualbox

![virtualbox](/assets/dia-01/virtualbox.png "virtualbox")

* Sistema operativo instalador en la MV (comando **uname -a** para obtener el dato en la terminal)

![uname](/assets/dia-01/uname.png "Ubuntu Server 24.04 LTS")

Una vez realizada la configuración del sistema operativo, se realizó la actualización de todo el sistema operativo con los comandos **sudo apt-get update** y **sudo apt-get upgrade**.

### Prueba de comandos básicos

#### Tabla de comandos básicos en Linux

| # | Comando  | Descripción                                                                 |
|---|----------|------------------------------------------------------------------------------|
| 1 | `whoami` | Muestra el nombre del usuario actual que está ejecutando la terminal.       |
| 2 | `pwd`    | **Print Working Directory**. Muestra la ruta absoluta del directorio actual. |
| 3 | `ls -lah`| Lista el contenido del directorio actual, incluyendo archivos ocultos y detalles. **[*]** |
| 4 | `mkdir`  | **Make Directory**. Crea un nuevo directorio (carpeta).                     |
| 5 | `cd`     | **Change Directory**. Cambia de directorio (navegación).                    |
| 6 | `echo`   | Muestra un mensaje o el valor de una variable.                              |
| 7 | `cat`    | Muestra el contenido de un archivo de texto en la terminal.                |

[*]: Detalle de `ls -lah`:  
- `-l`: listado largo (permisos, tamaño, propietario, etc.)  
- `-a`: incluye archivos ocultos (los que comienzan con `.`)  
- `-h`: muestra tamaños legibles (como `5.2K`, `1M`)

### Ejercicio realizado:

```bash
1. mkdir day-01                   # Crea una carpeta nueva llamada 'day-01'
2. cd day-01                      # Ingresa a la carpeta nueva 'day-01'
3. echo "Hola DevOps" > hola.txt  # Toma el mensaje mostrado "Hola DevOps" y lo almacena dentro un archivo nuevo con el nombre 'hola.txt'
4. cat hola.txt                   # Muestra el texto contenido dentro del archivo 'hola.txt'
```

![primerospasos](/assets/dia-01/PrimerosPasos.png "Primeros Pasos (comandos básicos)")

## 3. 🎯 Desafío: ¡Linux Detectives!

* ¿Cuánto tiempo lleva encendido tu sistema? (Comando **uptime**)

![uptime](/assets/dia-01/uptime.png "uptime")

* ¿Qué procesos están consumiendo más recursos? (Comando **top**)

![top](/assets/dia-01/top.png "top")

* ¿Cuánta memoria disponible tenés? (Comado **free -h**)

![free](/assets/dia-01/free-h.png "free -h")


## Comentarios finales

Este primer acercamiento me ha recordado conocimientos que creía olvidados, ha despertado mi curiosidad por aprender y me entusiasma saber que adquiriré cosas nuevas durante este laboratorio DevOps.

## Recurso recomendado

Como parte de ampliación de conceptos para la cultura DevOps, el recurso recomendado, es el siguiente video explicativo: 
https://www.youtube.com/watch?v=_I94-tJlovg&ab_channel=RackspaceTechnology