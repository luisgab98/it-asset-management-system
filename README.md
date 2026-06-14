# IT Asset Management System (Sistema de Control de Activos de TI) 🖥️📊

Un sistema web robusto de nivel empresarial diseñado para centralizar, administrar y auditar la asignación de equipos de cómputo y activos tecnológicos dentro de una organización multi-plaza.

Desarrollado con **Laravel**, este sistema optimiza el control logístico del departamento de TI, vinculando dinámicamente equipos, colaboradores, jerarquías de mando y ubicaciones geográficas.

---

## 🚀 Módulos y Características Clave

El sistema cuenta con una arquitectura relacional sólida que gestiona los siguientes módulos integrados:

- **📋 Panel de Asignaciones (Dashboard Principal):** Control central con buscador y paginación para rastrear qué equipo está asignado a qué colaborador, incluyendo folios, números de serie, marcas y estatus en tiempo real (*Activo / Baja*).
- **💻 Gestión Detallada de Equipos:** Registro exhaustivo de las especificaciones de hardware (Procesador, RAM, Almacenamiento SSD, Marca, Modelo, Número de Serie), credenciales técnicas (AnyDesk, Usuario de Admin) y enlaces directos a expedientes en la nube (Google Drive).
- **👥 Administración de Personal e Infraestructura Relacional:**
  - **Empleados:** Registro y control de colaboradores vinculados directamente a sus herramientas de trabajo.
  - **Jefes de Departamento:** Control de la estructura organizacional enlazando líderes con sus respectivos colaboradores.
  - **Plazas:** Segmentación geográfica de los activos y el personal por sucursales o corporativos (ej. Ciudad de México, Pachuca, Tijuana).
- **📉 Historial de Bajas:** Registro histórico y auditoría de equipos y personal dados de baja para mantener la integridad del inventario activo.
- **📥 Exportación de Datos:** Herramientas nativas para exportar reportes instantáneos a formatos **Excel** y **PDF**.

---

## 🛠️ Stack Tecnológico

- **Backend:** PHP / Laravel Framework (Arquitectura MVC, Eloquent ORM)
- **Frontend:** Blade Templates, JavaScript (Bootstrap / Tailwind CSS para diseño responsivo)
- **Base de Datos:** MySQL (Relaciones avanzadas Uno a Muchos y Muchos a Muchos)

---

## 📐 Arquitectura de la Base de Datos (Relaciones)

El backend implementa un diseño relacional estricto mediante migraciones de Laravel para asegurar la integridad referencial:

1. **Plazas ➡️ Jefes:** Una plaza puede albergar múltiples jefes de departamento.
2. **Jefes ➡️ Empleados:** Estructura jerárquica donde cada empleado está enlazado a un supervisor directo.
3. **Empleados 🔄 Equipos:** Relación directa que vincula las especificaciones técnicas del hardware con su usuario responsable.

---

## 💡 Habilidades Demostradas en este Proyecto

- Diseño de bases de datos relacionales complejas y optimización de consultas con Eloquent ORM.
- Desarrollo de interfaces de usuario limpias, funcionales y orientadas a la experiencia del usuario (UX) para entornos corporativos.
- Implementación de lógica de negocio para la generación de reportes descargables (Excel/PDF).
- Gestión de seguridad en la autenticación y control de accesos de usuarios al panel administrativo.
