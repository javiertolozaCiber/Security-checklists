#  Clasificacion de datos – Guía Básica

La clasificación de datos permite identificar el nivel de sensibilidad de la información y aplicar los controles adecuados según su criticidad. Esta guía sigue buenas prácticas de ISO 27001 y NIST SP 800-60.

-----------------------------------------

##  Objetivo.
Establecer un criterio simple y claro para clasificar datos dentro de una organización y asegurar su protección según el nivel de riesgo.

-----------------------------------------

##  Niveles de Clasificación.

### 1. Público.
Información que puede ser divulgada sin riesgo.
- Ejemplos: contenido del sitio web, material educativo general, comunicados públicos.

### 2. Interno.
Información de uso interno que no debe divulgarse fuera de la organización.
- Ejemplos: políticas internas, documentos operacionales, instructivos.

### 3. Confidencial.
Información sensible que requiere controles estrictos de acceso.
- Ejemplos: datos de clientes, datos personales, información financiera interna.

### 4. Sensible / Crítica.
Información altamente sensible cuyo acceso debe ser extremadamente limitado.
- Ejemplos: llaves de cifrado, secretos de API, credenciales privilegiadas, información estratégica.

-----------------------------------------

##  Controles sugeridos por nivel.

| Nivel | Controles mínimos |
| Público | Acceso libre, sin restricciones. |
| Interno | Autenticación básica, acceso por rol. |
| Confidencial | Cifrado en tránsito y en descanso, MFA, logs de acceso. |
| Secreta | Almacenamiento seguro (HSM o vault), rotación de claves, monitoreo continuo. |

-----------------------------------------

##  Buenas prácticas.
- Clasificar datos al momento de crearlos.
- Revisar periódicamente las clasificaciones.
- Evitar que datos sensibles aparezcan en entornos de pruebas.
- Aplicar principio de mínimo privilegio en todo acceso.
