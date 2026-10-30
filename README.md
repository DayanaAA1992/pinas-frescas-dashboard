# Piñas Frescas de Costa Rica S.A. · Dashboard ejecutivo

Prototipo interactivo de análisis agrícola desarrollado en HTML, CSS, JavaScript y SVG. Presenta una experiencia de exploración inspirada en Power BI, con nueve páginas para analizar producción, calidad, empaque, finanzas, personal, insumos, comercialización y planificación.

> Prototipo ejecutivo con identidad ficticia y datos sintéticos para capacitación. No representa resultados reales de ninguna empresa.

## Propósito

Mostrar cómo una herramienta gerencial puede ayudar a comparar fincas y lotes, identificar desviaciones respecto del plan y concentrar la atención en los resultados que requieren seguimiento.

## Páginas

1. Resumen general.
2. Producción agrícola.
3. Calidad.
4. Cosecha y empaque.
5. Finanzas.
6. Recursos humanos.
7. Insumos agrícolas.
8. Comercial y exportación.
9. Planificación.

## Funciones

- Cuatro KPIs por página y 41 visuales en total, incluyendo tablas de detalle.
- Filtros por fechas, meses, semanas, finca, lote y variedad.
- Selección cruzada de datos; Ctrl, ⌘ o Mayús permiten selección múltiple.
- Filtros conservados al cambiar de página.
- Comparaciones con el plan base disponible y panel para registrar metas originales faltantes.
- Semáforo con tolerancia del 5 %, con criterio invertido para costos y criterio de meta exacta cuando corresponde.
- Captura de metas por el conjunto exacto de registros seleccionado, sin prorrateos inventados.
- Descarga de una copia del HTML que incorpora las metas registradas.
- Formato numérico de Costa Rica y valores financieros en USD.
- Diseño responsive y adaptación al modo claro u oscuro del sistema.

## Abrir el dashboard

Descargue el repositorio y abra index.html con un navegador moderno. El archivo incluye los datos, el código, la tipografía Montserrat y la imagen de la piña; puede utilizarse sin conexión y no requiere instalación ni compilación.

La identidad usa azul marino, turquesa y tipografía de alto peso. Los KPIs emplean colores de cumplimiento con etiquetas explícitas. Las metas faltantes aparecen como «Sin plan disponible» hasta que el usuario las registre.

## Datos y cálculos

Los datos semanales abarcan del 1 de enero al 29 de octubre de 2026: tres fincas, 12 lotes, 44 semanas y ocho tablas operativas de 528 filas cada una. El HTML integra exclusivamente las tablas utilizadas en el reporte.

Los flujos se suman entre semanas. Las áreas, plantas y dotación usan el último registro disponible por lote en la selección. Los cruces entre tablas usan la clave lote + semana; no se multiplican los hechos mediante uniones cartesianas. Las semanas parciales se identifican y los denominadores cero no generan porcentajes ficticios. El resultado operativo estimado se distingue de medidas contables como EBITDA.

Las metas aportadas por el usuario se identifican por su fuente y alcance. El almacenamiento local del navegador puede variar; para conservarlas o compartirlas se recomienda «Descargar HTML con metas».

## Verificación y límites

Se aprobaron 33 comprobaciones locales del motor de cálculos y sus controladores en un entorno JavaScript simulado. Cubren totales, conciliaciones, filtros, saldos, ponderaciones, semáforos, alcance de las metas, persistencia y exportación. Se verificó la sintaxis JavaScript y la incrustación de recursos.

La revisión completa en Chrome, Edge, Firefox y Safari, la consola real y la distribución CSS en dispositivos permanecen pendientes. Las limitaciones y definiciones también están documentadas dentro del reporte.

## Tecnologías

HTML · CSS · JavaScript puro · SVG · recursos incrustados en Base64. Sin CDN, servicios de mapas ni APIs de ejecución.

## Recursos de terceros

Montserrat se distribuye bajo SIL Open Font License. Consulte [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md). La piña es una imagen generada con IA para este ejemplo.

## Sobre este proyecto

Demostración de desarrollo de herramientas de análisis y apoyo a la toma de decisiones empresariales. La adaptación a una empresa requiere acordar indicadores, validar fuentes, conciliar datos y definir responsables de actualización.
