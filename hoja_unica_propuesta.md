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

Opcion de almacenamiento:

Dell PowerEdge T160
Servidor Dell PowerEdge T160 Intel Xeon Performance 6333P 48GB DDR5 2x4TB HDD+2x960GB SSD PERC H355

Opcionales:

AC049355 16GB UDIMM ECC 5600
2TB 7.2K RPM SATA 6Gbps 512n 3.5in Hot-plug Hard Drive, CK
4TB 7.2K RPM SATA 6Gbps 512n 3.5in Hot-plug Hard Drive, CK
8TB 7.2K RPM SAS 12Gbps 512n 3.5in Hot-plug Hard Drive, CK
16TB 7.2K RPM SATA 6Gbps 512n 3.5in Hot-plug Hard Drive, CK
Windows Server 2022 / 2025 STD 16 Core
Dell Broadcom 57416 SFP y 57414 RJ45

Costo: $9.231.849,45

Link: https://tienda.datahaus.com.ar/products/servidor-dell-poweredge-t160-intel-xeon-e-2436-16gb-ddr5-2x2tb-hdd-2x240gb-ssd-perc-h355?_pos=13&_fid=4005e6916&_ss=c

Opcion procesamiento:

WORKSTATION - SERVIDOR - GAMER - IA
Intel Core Ultra 7 265K - Z890 - 128GB DDR5 ampliable a 192GB - SSD 1TB NVMe - RTX 5070Ti 16GB - Fuente 1000W - Rack 4U

Equipo de altisimo rendimiento, armado y testeado para inteligencia artificial, workstation profesional, servidor y gaming de alta gama. La placa RTX 5070Ti 16GB junto al Intel Core Ultra 7 265K (reemplaza al Core i7), 192GB de RAM maxima y fuente certificada de 1000W lo hacen ideal para IA / machine learning, renderizado 3D, edicion 4K, virtualizacion y juegos exigentes, en formato rackeable 4U.

Consultanos para sumar Windows, mas memoria, mas discos o una configuracion a medida. Emitimos Factura A.

****************************************

El equipo incluye los siguientes componentes:

* Procesador Intel Core Ultra 7 265K
* Cooler OC para el procesador
* Mother Z890 ( Consultar modelo disponible )
* Memoria RAM 128gb DDR5 expandible a 192gb ( Consultar modelo disponible )
* Disco Solido SSD 1Tb M.2 NVME ( Consultar modelo disponible )
* Gabinete Rackeable 4U ( Consultar modelo disponible )
* Fuente Certificada 1000w ( Consultar modelo disponible )
* Placa de video Gamer y para IA RTX 5070TI 16gb

Costo: $ 13.574.615

Link: https://www.mercadolibre.com.ar/servidor-ia-core-ultra-7-265k-rack/up/MLAU4165740883#polycard_client=search-desktop&be_origin=mixed&overlay_label=not_apply&search_layout=grid&position=12&type=product&tracking_id=c7ebe4fc-5ba1-43e7-95ef-dbfd9c8f66f0&wid=MLA1861586643&sid=search

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