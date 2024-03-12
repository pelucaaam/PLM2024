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

## Instalar Gurobi
**Nota:** Este paso es necesario hacerlo desde la red de la universidad sea directamente con el Wi-Fi o un VPN (instrucciones en el siguiente link https://www.cec.uchile.cl/2019-11-12-11-52-00-vpn/)

### Descargar Gurobi Optimizer

### Obtener licencia
Entrar a la página https://www.gurobi.com/ y crear una cuenta con el correo institucional (@ing.uchile.cl)

En el portal de usuario ingresar a licencias y elegir la opción de solicitar/request y generar licencia en la opción 'named-user academic', debiera entregar
directamente una licencia


## Instalar Julia 
Para instalar julia se tiene que correr el siguiente comando en la consola de comandos:

Si se tiene sistema operativo Windows
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
