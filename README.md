

# BugTracker - Form Consulta Bugs


## 1. Clonar Repositorio (Clone/Checkout)

**1.1. Ejecutar comando clone para descargar repositorio:** 
```sh
$ git clone https://github.com/utn-frc-pav1-3k5-2019/semana_4_bugtracker_consulta_bugs.git
```
**1.2. Crear un nuevo branch (rama)**

Para crear una nueva rama (branch) y saltar a ella, en un solo paso, puedes utilizar el comando  `git checkout`  con la opción  `-b`:

```sh
$ git checkout -b branch_{{legajo}}
Switched to a new branch "..."
```
Y para que se vea reflejada en GitHub:
```sh
$ git push --set-upstream origin branch_{{legajo}}
```

## 2. Ejecutar Script Base de datos
**2.1. Iniciar la aplicación `Sql Server Management Studio`**

Solicitará ingresar los datos de la base de datos para generar una conexión, completar los datos y hacer click en **Connect**. Los datos del servidor del labsis son:

 - **Tipo Servidor:** Database Engine
 - **Nombre Servidor:** maquis
 - **Autenticación:** SQL Server Authentication.
 - **Nombre de Usuario:** avisuales1
 - **Contraseña:** ******
 
 
 **2.2. Abrir archivo `BugTracker_DB.sql`**
 Ir a la opción `Archivo -> Abrir -> Archivo` (o combinación de teclas `Ctrl + O`) y buscar el archivo BugTracker_DB.sql en el disco local.
  
**2.3. Editar Script** 
> Antes de ejecutar editar el archivo BugTracker_DB.sql y reemplazar el nombre de la base de datos BugTracker, agregando el numero de legajo de la siguiente forma:
>  `BugTracker_{{legajo}}`

**2.4. Ejecutar Script** 
Para ejecutar el script hacer click sobre el botón `Ejecutar` (o usar la tecla `F5`)

## 3. Menú



## 4. Agregar Form ConsultaBugs

    
```csharp

```
## 5. ComboBox
