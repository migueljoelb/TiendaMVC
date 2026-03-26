# 🛒 TiendaMVC

![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Entity Framework](https://img.shields.io/badge/Entity_Framework_Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap_5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)

> Aplicación web CRUD desarrollada como trabajo final de curso, utilizando el patrón **MVC** con **ASP.NET Core** y **Entity Framework Core** con enfoque **Database First**.

---

## ✨ Funcionalidades

| Operación | Descripción |
|-----------|-------------|
| 📋 **Read** | Lista todos los productos registrados |
| ➕ **Create** | Agrega nuevos productos al sistema |
| ✏️ **Update** | Edita la información de un producto |
| 🔍 **Details** | Muestra el detalle completo de un producto |
| 🗑️ **Delete** | Elimina un producto del sistema |

---

## 🗂️ Estructura del Proyecto

```
TiendaMVC/
├── 📁 Controllers/
│   └── ProductosController.cs     # Lógica CRUD (Index, Create, Edit, Details, Delete)
├── 📁 Models/
│   ├── Producto.cs                # Modelo generado por Scaffold (Database First)
│   └── TiendaDbContext.cs         # Contexto de Entity Framework Core
├── 📁 Views/
│   ├── 📁 Productos/
│   │   ├── Index.cshtml           # Lista de productos
│   │   ├── Create.cshtml          # Formulario de creación
│   │   ├── Edit.cshtml            # Formulario de edición
│   │   ├── Details.cshtml         # Vista de detalle
│   │   └── Delete.cshtml          # Confirmación de eliminación
│   ├── 📁 Home/
│   │   └── Index.cshtml           # Página de inicio
│   └── 📁 Shared/
│       └── _Layout.cshtml         # Layout general con navbar y footer
├── 📁 wwwroot/
│   └── 📁 css/
│       └── site.css               # Estilos personalizados
├── appsettings.json               # Cadena de conexión a SQL Server
└── Program.cs                     # Configuración del DbContext y servicios
```

---

## 🛠️ Tecnologías Utilizadas

- ⚙️ **ASP.NET Core MVC** — Framework web con patrón Modelo-Vista-Controlador
- 🗄️ **Entity Framework Core** — ORM con enfoque Database First
- 🏢 **SQL Server** — Base de datos relacional
- 🎨 **Bootstrap 5** — Diseño visual responsivo
- 🔷 **C#** — Lenguaje de programación principal

---

## ⚙️ Requisitos Previos

- [Visual Studio 2022+](https://visualstudio.microsoft.com/)
- [SQL Server](https://www.microsoft.com/sql-server) o SQL Server Express
- [.NET 8 SDK](https://dotnet.microsoft.com/download)

---

## 🚀 Instalación y Configuración

**1. Clona el repositorio**
```bash
git clone https://github.com/tu-usuario/TiendaMVC.git
```

**2. Crea la base de datos en SQL Server Management Studio**
```sql
CREATE DATABASE TiendaDB;
GO
USE TiendaDB;
GO
CREATE TABLE Productos (
    ProductoID   INT IDENTITY(1,1) PRIMARY KEY,
    Nombre       NVARCHAR(100) NOT NULL,
    Descripcion  NVARCHAR(255),
    Precio       DECIMAL(10,2) NOT NULL,
    Stock        INT NOT NULL,
    FechaIngreso DATE NOT NULL
);
```

**3. Configura la cadena de conexión en `appsettings.json`**
```json
"ConnectionStrings": {
  "TiendaDB": "Server=localhost;Database=TiendaDB;Trusted_Connection=True;TrustServerCertificate=True;"
}
```

**4. Ejecuta el proyecto**
```
Presiona F5 en Visual Studio
```

---

## 📐 Patrón MVC

```
Usuario → Controlador → Modelo → Base de Datos
                ↓
             Vista → Usuario
```

- **Modelo** — `Producto.cs` define la estructura de datos
- **Vista** — Archivos `.cshtml` muestran la interfaz
- **Controlador** — `ProductosController.cs` gestiona las solicitudes

---

## 👨‍💻 Autor

Desarrollado como trabajo final de curso universitario.

---

> 📚 *Proyecto académico — Curso de Desarrollo Web*
