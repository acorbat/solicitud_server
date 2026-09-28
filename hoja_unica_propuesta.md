# Hoja única de propuesta: Servidor OMERO para la UBA

## 1) Propuesta
Las tecnologías de adquisición de imágenes científicas han avanzado considerablemente en los últimos años. Como resultado, algunos experimentos generan imágenes multidimensionales con volúmenes de datos de cientos de GB e incluso de varios TB por experimento. Esta situación limita las posibilidades de trabajo de algunos grupos de investigación, tanto por capacidad de almacenamiento como por dificultades para compartir y procesar los datos.

Además, la gestión de formatos de archivo, el almacenamiento y la preservación de datos a largo plazo representan un problema frecuente para equipos que no cuentan con experiencia técnica específica en infraestructura de datos. Una vez generadas las imágenes, surge un segundo desafío: cómo procesarlas de manera eficiente para extraer información cuantitativa.

Para abordar estos problemas, se propone centralizar estas capacidades en un servidor institucional de la Universidad de Buenos Aires, en el marco del proyecto **“Análisis de imágenes asistido por inteligencia artificial para la extracción de información cuantitativa”**.

La propuesta incluye:
- Adquisición e instalación de un servidor de alto rendimiento (HPC), preparado para incorporación futura de GPU.
- Implementación de OMERO (o sistema análogo) para la gestión centralizada de imágenes científicas.
- Configuración del almacenamiento inicial, políticas de backup y esquema de permisos por grupos.
- Puesta en marcha operativa y coordinación con el área de IT institucional.
- Acceso remoto y compartido para grupos de investigación, docencia y servicios de análisis de imágenes.
- Impacto directo en los servicios actuales de microscopía de la Facultad de Ciencias Exactas y Naturales, donde la adopción de OMERO resultaría especialmente ventajosa para ordenar, resguardar y compartir datos.

## 2) Presupuesto aproximado y uso de fondos (USD)

| Rubro | Monto estimado (USD) | En qué se gastaría |
|---|---:|---|
| Chasis + motherboard + fuentes redundantes | 2.500 - 4.000 | Plataforma de servidor 2U, expansión y estabilidad eléctrica |
| CPU (32 núcleos) | 3.500 - 6.000 | Capacidad de procesamiento para gestión y análisis de imagen |
| RAM 128 GB DDR5 | 1.200 - 2.000 | Manejo fluido de datasets de gran tamaño |
| Almacenamiento base SSD/NVMe | 800 - 1.500 | Sistema operativo y datos activos de trabajo |
| **Total estimado del proyecto** | **8.000 - 13.500** | **Infraestructura inicial completa** |

**Referencia comercial (Argentina):**
- Datahaus Argentina (ejemplo de servidor de clase equivalente, 2U y escalable):
  https://tienda.datahaus.com.ar/products/servidor-dell-poweredge-r570-xeon-6-performance-6730p-32c-64t-288mb-256gb-4x-1-92tb-ssd-sata-4x10-25-sfp-2x-10gb-rj45

## 3) Impacto esperado

### Impacto institucional (UBA)
- Consolidación de un **repositorio central** de imágenes con trazabilidad y metadatos.
- Reducción del riesgo de pérdida de datos (discos externos y almacenamiento disperso).
- Mejora de gobernanza de datos: permisos, auditoría de acceso y políticas de preservación.

### Impacto científico y académico
- Acceso remoto seguro para múltiples laboratorios y plataformas de microscopía.
- Mayor reproducibilidad y reutilización de datasets entre grupos.
- Base para servicios de análisis de imagen e integración progresiva de IA/Deep Learning (vía GPU futura o workstation dedicada).

### Impacto operativo y económico
- Menor duplicación de almacenamiento y mejor uso de recursos compartidos.
- Disminución de tiempos de transferencia y organización de datos.
- Escalabilidad a mediano plazo sin reinvertir en una arquitectura nueva desde cero.

## 4) Resultado esperado en 12 meses
- OMERO operativo para usuarios institucionales.
- Políticas de backup y acceso implementadas.
- Adopción por plataformas de imagen y grupos de investigación prioritarios.
- Capacidad instalada para crecimiento y futuras etapas de análisis avanzado.