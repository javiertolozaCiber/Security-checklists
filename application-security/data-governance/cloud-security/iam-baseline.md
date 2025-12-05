#  IAM Baseline – Buenas Prácticas Esenciales.

Esta guía establece una línea base (baseline) de seguridad para la gestión de identidades y accesos (IAM) en entornos cloud. Se basa en recomendaciones CIS, NIST y mejores prácticas de la industria.

----------------------------------------------------------

##  Objetivo
Definir controles mínimos para garantizar que el acceso a recursos cloud sea seguro, trazable y administrado bajo el principio de mínimo privilegio.

----------------------------------------------------------

##  Controles de Identidad y Acceso

### 1. Autenticación
- Habilitar **MFA obligatorio** para todas las cuentas.
- Prohibir cuentas sin contraseña o sin rotación.
- Preferir autenticación federada (SSO).

### 2. Gestión de Roles y Permisos
- Utilizar **roles basados en tareas** (RBAC).
- Evitar asignar permisos directamente a usuarios.
- Aplicar **Least Privilege** y revisiones periódicas.

### 3. Cuentas Privilegiadas
- Minimizar el uso de cuentas admin.
- Crear cuentas de break-glass con controles robustos.
- Registrar y monitorear cada acción privilegiada.

### 4. Claves y Credenciales
- Almacenar claves en servicios seguros (Vault / KMS).
- Activar rotación automática de claves y tokens.
- Prohibir credenciales embebidas en código.

----------------------------------------------------------

##  Auditoría y Monitoreo
- Registrar accesos a todos los servicios cloud.
- Configurar alertas de:
  - Inicios de sesión sospechosos
  - Cambios en permisos
  - Uso anormal de claves
- Activar logs inmutables cuando sea posible.

----------------------------------------------------------

##  Buenas Prácticas Generales
- Revisión trimestral de roles y permisos.
- Deshabilitar cuentas inactivas.
- Usar etiquetas (tags) para identificar recursos críticos.
- Documentar flujos de acceso para auditoría.
