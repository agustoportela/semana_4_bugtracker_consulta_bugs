
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
**2.3. Ejecutar Script `BugTracker_DB.sql`**

> Editar el archivo BugTracker_DB.sql y reemplazar el nombre de la base de datos BugTracker, agregando el numero de legajo de la siguiente forma:
>  `BugTracker_{{legajo}}`

```sql
USE [master]
-- Importante!!!!!! Reemplazar nombre de base de datos con formato BugTracker_{{legajo}} 
CREATE DATABASE [BugTracker]
GO
-- Importante!!! Reemplazar nombre de base de datos con formato BugTracker_{{legajo}}
USE [BugTracker]
GO
/****** Object:  Table [dbo].[Bugs]    Script Date: 20/8/2019 22:43:37 ******/
SET ANSI_NULLS ON
GO
SET QUOTED_IDENTIFIER ON
GO
CREATE TABLE [dbo].[Bugs](
...
```
## 3. Menú


```csharp

```

## 4. ComboBox

## 5. Agregar Form ConsultaBugs

    