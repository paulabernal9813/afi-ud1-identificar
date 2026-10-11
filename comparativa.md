# Comparativa de normas de análisis forense digital

## Tabla comparativa

| Aspecto | RFC 3227 | NIST SP 800-86 | ENFSI |
# Comparativa de normas de análisis forense digital

## Tabla comparativa

| Aspecto | RFC 3227 | NIST SP 800-86 | ENFSI |
|---|---|---|---|
| **Qué entiende por “identificar”** | Identificar dónde puede estar la evidencia: qué sistemas intervinieron, qué datos son relevantes y admisibles, y qué otros elementos pueden aparecer como evidencia durante la actuación. También exige documentar personas, tiempos y acciones realizadas. [RFC 3227 §2, §3.2] | Identificar es la primera fase de la recogida de datos: determinar, etiquetar, registrar y adquirir información de todas las fuentes potencialmente relevantes, preservando su integridad. [NIST SP 800-86 §3.1] | Identificar forma parte de la evaluación del caso: antes y durante la intervención en la escena se determina qué objetos digitales pueden contener evidencia, qué riesgos presentan y qué necesidades tiene la investigación. [ENFSI §9.2] |
| **Fuentes de evidencia que menciona** | Registros y caché; tablas de enrutamiento y ARP; procesos, memoria y estadísticas del núcleo; sistemas de archivos temporales; disco; registros remotos y monitorización; configuración y topología de red; soportes de archivo; personas presentes y sus observaciones. [RFC 3227 §2.1, §3.2] | Archivos y medios de almacenamiento; sistemas operativos; tráfico de red; aplicaciones; equipos de red como routers y cortafuegos; dispositivos móviles, PDA, periféricos, CDs/DVDs, discos extraíbles, cintas de respaldo, memorias flash y otros dispositivos electrónicos. [NIST SP 800-86 §3.1.1] | Sistemas informáticos y teléfonos; dispositivos y sistemas remotos; elementos presentes en la escena y sus riesgos; documentación, registros e informes generados durante el proceso forense. [ENFSI §8.2, §9.1–9.2] |
| **Criterio para decidir qué se protege primero** | El orden de volatilidad: se adquiere primero lo más volátil —registros, caché, memoria, procesos y conexiones activas— y después lo menos volátil, como el disco o los soportes de archivo. Además, se debe recolectar antes de analizar. [RFC 3227 §2.1] | La posible pérdida de datos dinámicos: hay que actuar con rapidez porque pueden desaparecer conexiones de red activas y datos de dispositivos con batería. También se valoran la relevancia para el incidente, la legalidad y la integridad de la evidencia. [NIST SP 800-86 §3.1.1] | La evaluación de riesgos y la priorización: se valora el riesgo de pérdida o alteración, la seguridad de la escena, las condiciones técnicas de cada dispositivo y las necesidades concretas del caso antes de decidir la secuencia de actuación. [ENFSI §9.2] |
