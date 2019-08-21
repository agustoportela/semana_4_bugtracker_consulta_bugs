

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

La `MenuStrip` clase proporciona un sistema de menús para formularios.

La  `ToolStripMenuItem` clase proporciona propiedades que le permiten configurar la apariencia y la funcionalidad de un elemento de menú. Para que se muestre `ToolStripMenuItem` un objeto, debe agregarlo a un `MenuStrip`objeto


### 3.1. Como crear un menú estándar

El Diseñador de Windows Forms puede rellenar automáticamente un  [MenuStrip](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.menustrip)  control con elementos de menú estándar.

1.  Desde el  **cuadro de herramientas**, arrastre un  [MenuStrip](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.menustrip)  control al formulario.
    
2.  Haga clic en el  [MenuStrip](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.menustrip)  glifo de etiqueta inteligente del control (![glifo de etiqueta inteligente](https://docs.microsoft.com/es-es/dotnet/framework/winforms/controls/media/vs-winformsmttagglyph.gif "VS_WinFormSmtTagGlyph")) y seleccione  **insertar elementos estándar**.
    
    El  [MenuStrip](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.menustrip)  control se rellena con los elementos de menú estándar.
    
3.  Haga clic en el  **Archivo**  elemento de menú para ver sus elementos de menú predeterminados y los iconos correspondientes.
**![](https://lh4.googleusercontent.com/X2FSHd0WcB5z0EUsGpIr9c3h5zG_9L4WbwdfVm9DDSdNR2dzjDPV-0q1pTmCOCZKhMzrbOXnh5_RCdF6uFVq8VynYZ5c4LQb1444NTKeKwDTq6u_nxWMECNWgmcNEgGem2MN3aA0)**
### 3.3. Elementos de un MenuStrip

- MenuItem ([ToolStripMenuItem](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.toolstripmenuitem?view=netframework-4.8))
- ComboBox ([ToolStripComboBox](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.toolstripcombobox?view=netframework-4.8))
- TextBox ([ToolStripTextBox](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.toolstriptextbox?view=netframework-4.8))

**![](https://lh6.googleusercontent.com/iN-tD4oRHPZF3kJGubFZEsHBByqVQVIfYFSFlrL_tJzhuDwbQbl1TvkLNVCL_tFQP6xTEnBP3_RDWRObmy7S1G1WBwEs_lIdhykFJhbIH1xQaF_UeP3IHIXHxZrLM6j9zFfSiqXc)**

### 3.3. Como crear un control StatusStrip

Use el  [StatusStrip](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.statusstrip)  control para mostrar el estado de las aplicaciones de Windows Forms.  En el ejemplo actual, se muestran los elementos de menú seleccionados por el usuario en un  [StatusStrip](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.statusstrip)control.

1.  Desde el  **cuadro de herramientas**, arrastre un  [StatusStrip](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.statusstrip)  control al formulario.
    
    El  [StatusStrip](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.statusstrip)  control se acopla automáticamente a la parte inferior del formulario.
    
2.  Haga clic en el  [StatusStrip](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.statusstrip)  del control de botón de lista desplegable y seleccione  **StatusLabel como**  para agregar un  [ToolStripStatusLabel](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.toolstripstatuslabel)  el control a la  [StatusStrip](https://docs.microsoft.com/es-es/dotnet/api/system.windows.forms.statusstrip)  control.

**![](https://lh3.googleusercontent.com/BrbD9NOg2P9UDPpr-kT4skERlWwxSaZdl_OiGG4M17YdVRkNUApKYiTJIcURxLzvi-Op8v9P269GxoeQy1wiIXR6QZic-o8OVwpDfE2aXm1QOCLfdcGCaK3uT_bs3yWwCw3Gpsjc)**
#

## 4. Actividad sobre el Menú

4.1. Agregar al menú **Consultar Bugs** de **frmPrincipal**, el evento **Click()** para abrir el formulario **frmConsultaBugs**   
```csharp

        private void consultarBugsToolStripMenuItem_Click(object sender, EventArgs e)
        {
            frmConsultaBugs frmDetalle = new frmConsultaBugs();
            frmDetalle.ShowDialog();
        }
```

4.2. Agregar al menú **Salir** de **frmPrincipal**,  el evento **Click()** que ejecute el cierre de la aplicación.

```csharp
	    private void salirToolStripMenuItem_Click(object sender, EventArgs e)
        {
            this.Close();
        }

```

```csharp

```
## 5. Completar ComboBox (Filtros Busqueda)

En esta actividad vamos a trabajar con el formulario **frmConsultaBugs**, vamos a cargar los diferentes combos (que van a ser el filtro de búsqueda de bugs) que hay en el formulario con datos de la base de datos:
**![](https://lh3.googleusercontent.com/qkUsfmsSbcNK3_UJTJKEv5VVdTrzsIUpFQBJBfKokSElexvd53caYVj_FHBioAMGUMbLXzbQ4Vdv7sFsBG6Iep-RbcHTcS4mSpss7vsFviBgT4EzeODKKrFkuCqal7BilH6WftDH)**

5.1. En la clase **frmConsultaBugs** agregar el siguiente método:

```csharp
		 private void llenarCombo(ComboBox cbo, Object source, string display, String value)
        {
            cbo.DataSource = source;
            cbo.DisplayMember = display;
            cbo.ValueMember = value;
            cbo.SelectedIndex = -1;
        }
```
5.2. Agregar al formulario el evento Load(), y en dicho evento se procederá a cargar los combos de la siguiente forma:
```csharp
        private void frmBugs_Load(object sender, EventArgs e)
        {

            //LLenar combos y limpiar grid
            LlenarCombo(cboEstados, DBHelper.GetDBHelper().ConsultaSQL("Select * from Estados"), "nombre", "id_estado");

            LlenarCombo(cboPrioridades, DBHelper.GetDBHelper().ConsultaSQL("Select * from Prioridades"), "nombre", "id_prioridad");

            LlenarCombo(cboCriticidades, DBHelper.GetDBHelper().ConsultaSQL("Select * from Criticidades"), "nombre", "id_criticidad");

            LlenarCombo(cboAsignadoA, DBHelper.GetDBHelper().ConsultaSQL("Select * from Usuarios"), "n_usuario", "nombre");

            LlenarCombo(cboProductos, DBHelper.GetDBHelper().ConsultaSQL("Select * from Productos"), "nombre", "nombre");

        }
```
## 6. Consultar Bugs

6.1. Agregar al botón **Consultar** el evento **Click()**, para que construya la consulta sql que busque los bugs registrados en la base de datos, con los filtros cargados en el formulario:

```csharp
		private void btnConsultar_Click(object sender, EventArgs e)
        {
            string strSql = "SELECT TOP 20 * FROM bugs WHERE 1=1 ";
            Dictionary<string, object> parametros = new Dictionary<string, object>();

            DateTime fechaDesde;
            DateTime fechaHasta;
            if (DateTime.TryParse(txtFechaDesde.Text, out fechaDesde) &&
                DateTime.TryParse(txtFechaHasta.Text, out fechaHasta))
            {
                strSql += " AND (fecha_alta>=@fechaDesde AND fecha_alta<=@fechaHasta) ";
                parametros.Add("fechaDesde", txtFechaDesde.Text);
                parametros.Add("fechaHasta", txtFechaHasta.Text);
            }


            if (!string.IsNullOrEmpty(cboEstados.Text))
            {
                var idEstado = cboEstados.SelectedValue.ToString();
                strSql += "AND (id_estado=@idEstado) ";
                parametros.Add("idEstado", idEstado);
            }

            if (!string.IsNullOrEmpty(cboAsignadoA.Text))
            {
                var asignadoA = cboAsignadoA.SelectedValue.ToString();
                strSql += "AND (asignado_a=@asignadoA) ";
                parametros.Add("asignadoA", asignadoA);
            }

            if (!string.IsNullOrEmpty(cboPrioridades.Text))
            {
                var prioridad = cboPrioridades.SelectedValue.ToString();
                strSql += "AND (id_prioridad=@idPrioridad) ";
                parametros.Add("idPrioridad", prioridad);
            }

            if (!string.IsNullOrEmpty(cboCriticidades.Text))
            {
                var criticidad = cboCriticidades.SelectedValue.ToString();
                strSql += "AND (id_criticidad=@idCriticidad) ";
                parametros.Add("idCriticidad", criticidad);
            }

            if (!string.IsNullOrEmpty(cboProductos.Text))
            {
                var producto = cboProductos.SelectedValue.ToString();
                strSql += "AND (id_producto=@idProducto) ";
                parametros.Add("idProducto", producto);
            }

            strSql += " ORDER BY fecha_alta DESC";
            dgvBugs.DataSource = DBHelper.GetDBHelper().ConsultaSQLConParametros(strSql, parametros);
            if (dgvBugs.Rows.Count == 0)
            {
                MessageBox.Show("No se encontraron coincidencias para el/los filtros ingresados", "Aviso", MessageBoxButtons.OK, MessageBoxIcon.Information);
            }

        }
```
