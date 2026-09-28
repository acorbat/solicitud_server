# Análisis de imágenes asistido por inteligencia artificial para la extracción de información cuantitativa

## 1) Propuesta
Las tecnologías de adquisición de imágenes científicas han avanzado considerablemente en los últimos años. Como resultado, **algunos experimentos generan imágenes multidimensionales con volúmenes de datos de cientos de GB e incluso de varios TB por experimento**. Esta situación limita las posibilidades de trabajo de algunos grupos de investigación, tanto por capacidad de almacenamiento como por dificultades para compartir y procesar los datos.

**Además, la gestión de formatos de archivo, el almacenamiento y la preservación de datos a largo plazo representan un problema frecuente para equipos que no cuentan con experiencia técnica específica en infraestructura de datos. Una vez generadas las imágenes, surge un segundo desafío: cómo procesarlas de manera eficiente para extraer información cuantitativa**.

Para abordar estos problemas, se propone centralizar estas capacidades en un servidor institucional de la Universidad de Buenos Aires, en el marco del proyecto **“Análisis de imágenes asistido por inteligencia artificial para la extracción de información cuantitativa”**.

La propuesta incluye:
- Adquisición e instalación de un servidor de alto rendimiento (HPC), preparado para incorporación futura de GPU.
- Implementación de OMERO (o sistema análogo) para la gestión centralizada de imágenes científicas.
- Configuración del almacenamiento inicial, políticas de backup y esquema de permisos por grupos.
- Puesta en marcha operativa y coordinación con el área de IT institucional.
- Acceso remoto y compartido para grupos de investigación, docencia y servicios de análisis de imágenes.
- Impacto directo en los servicios actuales de microscopía de la Facultad de Ciencias Exactas y Naturales, donde la adopción de OMERO resultaría especialmente ventajosa para ordenar, resguardar y compartir datos.

## 2) Presupuesto aproximado y uso de fondos (USD)

Para esta propuesta se presentan **dos referencias comerciales** a modo orientativo, únicamente para establecer órdenes de magnitud de costos. **No constituyen opciones cerradas ni definitivas de compra**.

- Referencia 1 (perfil servidor para almacenamiento/servicios): **$9.231.849,45 ARS**  
  Link: https://tienda.datahaus.com.ar/products/servidor-dell-poweredge-t160-intel-xeon-e-2436-16gb-ddr5-2x2tb-hdd-2x240gb-ssd-perc-h355?_pos=13&_fid=4005e6916&_ss=c

- Referencia 2 (perfil procesamiento con GPU): **$13.574.615 ARS**  
  Link: https://www.mercadolibre.com.ar/servidor-ia-core-ultra-7-265k-rack/up/MLAU4165740883#polycard_client=search-desktop&be_origin=mixed&overlay_label=not_apply&search_layout=grid&position=12&type=product&tracking_id=c7ebe4fc-5ba1-43e7-95ef-dbfd9c8f66f0&wid=MLA1861586643&sid=search

Con base en estas referencias, se estima un costo total del proyecto del orden de **USD 15.000** (sujeto a cotización, disponibilidad y configuración final).

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