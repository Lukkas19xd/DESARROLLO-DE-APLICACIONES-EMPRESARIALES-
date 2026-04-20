# Sistema de Gestión de Clientes Corporativo

Aplicación web  para la gestión integral de clientes, con autenticación de usuarios y roles diferenciados.

## Características Principales

- **Autenticación Segura**: Sistema de login con roles de administrador y cliente.
- **Registro de Clientes**: Formulario para ingresar datos de nuevos clientes (Nombre, RUT, Correo, Teléfono).
- **Base de Datos SQLite**: Almacenamiento persistente de información en archivo local `clientes.db`.
- **Interfaz Moderna**: Diseño profesional con tema corporativo, animaciones sutiles y responsive.
- **Roles y Permisos**:
  - **Cliente**: Acceso limitado al registro de clientes.
  - **Administrador**: Acceso completo a registro, reportes, estadísticas y administración de datos.
- **Reportes y Estadísticas**: Visualización de métricas en tiempo real y exportación a CSV.
- **Mantenimiento**: Funcionalidades de eliminación de registros.

## Tecnologías Utilizadas

- **Interfaz**: Streamlit (Python)
- **Base de Datos**: SQLite
- **Estilos**: CSS personalizado 
- **Librerías**: Pandas para manipulación de datos

## Credenciales de Acceso

Para iniciar sesión en la aplicación:

- **Usuario Administrador**:
  - Nombre de usuario: `admin`
  - Contraseña: `admin123`

- **Usuario Cliente**:
  - Nombre de usuario: `cliente`
  - Contraseña: `cliente123`

## Instalación y Ejecución

1. **Instalar dependencias**:
   ```powershell
   pip install -r requirements.txt
   ```

2. **Ejecutar la aplicación**:
   ```powershell
   py -m streamlit run app.py
   ```

## Archivos del Proyecto

- `app.py` — Código fuente principal de la aplicación.
- `requirements.txt` — Lista de dependencias Python.
- `clientes.db` — Base de datos SQLite (creada automáticamente).
- `README.md` — Documentación del proyecto.

## Funcionalidades por Rol

### Rol Cliente
- Registro de nuevos clientes
- Acceso limitado a funciones básicas

### Rol Administrador
- Todas las funciones del cliente
- Visualización de reportes y estadísticas
- Exportación de datos a CSV
- Administración y eliminación de registros

## Notas de Desarrollo

- La aplicación utiliza sesiones de Streamlit para mantener el estado de autenticación.
- La base de datos se crea automáticamente al ejecutar la aplicación por primera vez.