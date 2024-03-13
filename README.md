# PLM2024

## Instalar Conda
Entrar a la página https://www.anaconda.com/download/ y descargar la versión correspondiente al sistema operativo
de tu computador. 

Corre el programa descargado sin cambiar ninguna de las configuraciones propuestas por el instalador (es decir, lo
único que se tiene que hacer es apretar siguiente y estar de acuerdo con el acuerdo de licencia).

Una vez instalado, busca la consola de anaconda que debiera aparecer como anaconda prompt (anaconda3) y abrela.

Para instalar jupyter notebook, corre el siguiente comando en la consola de anaconda:
```
conda install jupyter
```
Y con esto se tiene instalado anaconda y Jupyter Notebook.

En caso de que se necesite instalar una nueva librería en anaconda, es cosa de repetir el comando anterior cambio jupyter por la nueva librería
``` 
conda install %nombre-de-librería%
```

## Instalar Gurobi
**Nota:** Este paso es necesario hacerlo desde la red de la universidad sea directamente con el Wi-Fi o un VPN (instrucciones en el siguiente link https://www.cec.uchile.cl/2019-11-12-11-52-00-vpn/)

### Descargar Gurobi Optimizer

Entrar a la página https://www.gurobi.com/ y seleccionar Gurobi Software
![imagen](https://github.com/pelucaaam/PLM2024/assets/52426349/adefe3ed-cda3-45b5-afba-f2ae1a6cd2ea)

En la nueva pestaña, seleccionar la versión que corresponde al sistema operativo del computador.

Corre el programa descargado sin cambiar ninguna de las configuraciones propuestas por el instalador (es decir, lo
único que se tiene que hacer es apretar siguiente y estar de acuerdo con el acuerdo de licencia).

Y con esto se tiene instalado Gurobi

### Obtener licencia
Entrar a la página https://www.gurobi.com/ y crear una cuenta con el correo institucional (@ing.uchile.cl)

En el portal de usuario ingresar a licencias y elegir la opción de solicitar/request 
![imagen](https://github.com/pelucaaam/PLM2024/assets/52426349/d132eba2-360d-4577-a524-0c4f86e30277)


Generar licencia en la opción 'named-user academic'

![imagen](https://github.com/pelucaaam/PLM2024/assets/52426349/6105e12d-831d-48a7-9eec-45f6b7d0b57c)

Una vez generada entregara un comando que se debera ingresar en la consola de comandos 

![imagen](https://github.com/pelucaaam/PLM2024/assets/52426349/8bfe603b-340c-406f-963a-bcb812b628b7)

Y con esto ya se tiene instalada la licencia de Gurobi

## Instalar Julia 
Para instalar julia se tiene que correr el siguiente comando en la consola de comandos:

Si se tiene sistema operativo Windows:
```
winget install julia -s msstore
```

Si se tiene sistema operativo MacOS o Linux:
```
curl -fsSL https://install.julialang.org | sh
```
**Nota:** Si se tiene instalado un package manager se tiene que instalar con dicho manager, por ejemplo, si se tiene chocolatey:
```
choco install julia
```

Una vez instalado Julia debieras ser capaz de tipear julia en la consola de comandos, pasando a la consola de comandos de Julia.
Debiera aparecer de la siguiente manera

```
               _
   _       _ _(_)_     |  Documentation: https://docs.julialang.org
  (_)     | (_) (_)    |
   _ _   _| |_  __ _   |  Type "?" for help, "]?" for Pkg help.
  | | | | | | |/ _` |  |
  | | |_| | | | (_| |  |  Version 1.10.2 (2024-03-01)
 _/ |\__'_|_|_|\__'_|  |  Official https://julialang.org/ release
|__/                   |

julia>
```

Luego se tienen que ingresar el siguiente comando en la consola de comandos de julia para dar paso a la instalación de las librerías que serán necesarias para los laboratorios
```
using Pkg
```
Y se ingresan los siguientes comandos
```
Pkg.add("IJulia")
Pkg.add("JuMP")
Pkg.add("Gurobi")
```
Y con esto y todo lo anterior ya esta todo configurado para poder hacer un laboratorio de PLM.

En caso de tener fallas en el proceso de instalación que no son posibles de resolver en un tiempo razonable, favor de contactar al equipo docente.
