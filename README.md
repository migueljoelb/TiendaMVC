# 🛒 TiendaMVC

![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Entity Framework](https://img.shields.io/badge/Entity_Framework_Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap_5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)

> Aplicación web CRUD desarrollada como trabajo final de la universidad, utilizando el patrón **MVC** con **ASP.NET Core** y **Entity Framework Core** con enfoque **Database First**.

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
- [SQL Server](https://www.microsoft.com/sql-server)
- [.NET 8 SDK](https://dotnet.microsoft.com/download)

---

## 👨‍💻 Autor

Desarrollado como trabajo final de curso universitario.

---

> 📚 *Proyecto académico — Programacion III*
