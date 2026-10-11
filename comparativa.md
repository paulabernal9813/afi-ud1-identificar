# Comparativa de normas de análisis forense digital

## Tabla comparativa

| Aspecto | RFC 3227 | NIST SP 800-86 | ENFSI |
|---|---|---|---|
| **Qué entiende por “identificar”** | Identificar dónde puede estar la evidencia: qué sistemas intervinieron, qué datos son relevantes y admisibles, y qué otros elementos pueden aparecer como evidencia durante la realización. También exige documentar personas, tiempos y acciones realizadas. | Identificar es la primera fase de la recogida de datos: determinar, etiquetar, registrar y adquirir información de todas las fuentes potencialmente relevantes, preservando su integridad. | Identificar forma parte de la evaluación del caso: antes y durante la intervención en la escena se determina qué objetos digitales pueden contener evidencia, qué riesgos presentan y qué necesidades tiene la investigación. |
| **Fuentes de evidencia que menciona** | Registros y caché; tablas de enrutamiento y ARP; procesos, memoria y estadísticas del núcleo; sistemas de archivos temporales; disco; registros remotos y monitorización; configuración y topología de red; soportes de archivo; personas presentes y sus observaciones. | Archivos y medios de almacenamiento; sistemas operativos; tráfico de red; aplicaciones; equipos de red como routers y cortafuegos; dispositivos móviles, PDA, periféricos, CDs/DVDs, discos extraíbles, cintas de respaldo, memorias flash y otros dispositivos electrónicos. | Sistemas informáticos y teléfonos; dispositivos y sistemas remotos; elementos presentes en la escena y sus riesgos; documentación, registros e informes generados durante el proceso forense. |
| **Criterio para decidir qué se protege primero** | El orden de volatilidad: se adquiere primero lo más volátil (registros, caché, memoria, procesos y conexiones activas) y después lo menos volátil, como el disco o los soportes de archivo. Además, se debe recolectar antes de analizar. | La posible pérdida de datos dinámicos: hay que actuar con rapidez porque pueden desaparecer conexiones de red activas y datos de dispositivos con batería. También se valoran la relevancia para el incidente, la legalidad y la integridad de la evidencia. | La evaluación de riesgos y la priorización: se valora el riesgo de pérdida o alteración, la seguridad de la escena, las condiciones técnicas de cada dispositivo y las necesidades concretas del caso antes de decidir la secuencia de actuación. |

## En qué coinciden

Las tres normas coinciden en que la identificación debe realizarse antes de alterar el sistema. Todas insisten en documentar cuidadosamente cada acción, conservar la integridad de la evidencia y utilizar procedimientos reproducibles que permitan mantener la cadena de custodia.

También coinciden en que la evidencia no se encuentra únicamente en el ordenador que se tiene delante. Pueden existir datos relevantes en la red, registros remotos, dispositivos móviles, almacenamiento externo, copias de seguridad o incluso en el testimonio de personas presentes en la escena.

Por último, las tres consideran que la recogida debe hacerse de forma ordenada y justificada, evitando modificaciones innecesarias del sistema y priorizando aquello que puede perderse si no se actúa rápidamente.

## En qué se diferencian

La **RFC 3227** es la más práctica para actuar sobre un sistema encendido. Su aportación principal es el **orden de volatilidad**, que indica qué información debe capturarse primero para evitar que desaparezca.

El **NIST SP 800-86** amplía la perspectiva hacia la respuesta a incidentes. No se limita al equipo analizado: obliga a pensar en fuentes distribuidas, como la red, las aplicaciones, los sistemas operativos, los dispositivos móviles y los servicios remotos.

El **manual de ENFSI** añade la visión de un laboratorio forense europeo. Da más importancia a la preparación previa, la evaluación de riesgos, la seguridad en la escena, la validación de los procedimientos y la proporcionalidad de las decisiones respecto al caso.
