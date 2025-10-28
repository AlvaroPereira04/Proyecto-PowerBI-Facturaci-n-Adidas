# Proyecto-PowerBI-Facturaci-n-Adidas
Dashboard de facturación y rentabilidad (Adidas) en Power BI con modelo estrella, tabla de fechas en DAX, medidas KPI y páginas: Portada, Hipótesis, Informe, Mensuales, Conclusiones y Tooltip.

Análisis de facturación y rentabilidad con Power BI. Incluye modelo de datos, tabla de fechas en DAX, KPIs y páginas: **Portada**, **Hipótesis**, **Informe**, **Mensuales**, **Conclusiones** y **Tooltip**. Basado en la documentación del proyecto final (PDF adjunto). :contentReference[oaicite:2]{index=2}

## 🧭 Contenido
- `ProyectoFinal-Alvaro.pbix` – archivo principal de Power BI
- `docs/Proyecto-Final-Alvaro-Vargas.pdf` – documentación del proyecto (memoria)
- `assets/` – capturas de las páginas del informe
- `dax/` – snippets DAX (tabla de fechas y medidas)
- `CHANGELOG.md` – cambios por versión

## 🗺️ Modelo y Alcance
- Modelo tipo estrella con tablas de dimensiones (Categorías, Ciudades, Colores, Estados, Familias, Géneros, Regiones, TipoProducto, TipoVenta, Vendedor) y **hechos de Ventas**; relación con **Calendario** por fecha. :contentReference[oaicite:3]{index=3}
- Páginas: **Portada**, **Hipótesis**, **Informe**, **Mensuales**, **Conclusiones**, **Tooltip**. :contentReference[oaicite:4]{index=4}

## 🧮 DAX destacado
- **Tabla de Fechas** con columnas de Año, Mes, Nº de Mes, Trimestre, Semestre, Bimestre, Estación; marcada como tabla de fechas. :contentReference[oaicite:5]{index=5}
- **Medidas clave**:
  - `Total Facturado = SUM(VENTAS[TOTAL])`
  - `Total Rentabilidad = SUM(VENTAS[RENTABILIDAD])`
  - `Ventas = COUNTROWS(VENTAS)`
  - `Facturación Promedio = AVERAGE(VENTAS[TOTAL])`
  - `Rentabilidad Promedio = AVERAGE(VENTAS[RENTABILIDAD])`
  - `Tasa` y `Diferencia` para crecimiento vs periodo anterior
  - KPIs de **Evaluación** (estrellas) y percentiles/mediana de rentabilidad
  - Identificación de **estado más/menos rentable** y **estado con más ventas**  
  (Ver detalles en `/dax` y en el PDF). :contentReference[oaicite:6]{index=6}

## 📊 Visuales y segmentaciones
- Mapa de rentabilidad por estados, Top 5 productos más rentables, rentabilidad por tipo de venta (Online/Outlet/Tienda), segmentadores por Zona/TipoProducto/Semestre/Año/Mes. :contentReference[oaicite:7]{index=7}
- Custom visual: **TACHOMETER by E&A** para rentabilidad anual/mensual (con límite dinámico). :contentReference[oaicite:8]{index=8}

## 🚀 Cómo abrir
1. Cloná el repo y abrí `ProyectoFinal-Alvaro.pbix` con **Power BI Desktop** (versión reciente).
2. Asegurate de tener el custom visual **Tachometer by E&A** (importar desde marketplace si el archivo lo requiere). :contentReference[oaicite:9]{index=9}
3. Actualizá datos si corresponde y navegá por las páginas (botonera en Portada). :contentReference[oaicite:10]{index=10}

## 📁 Estructura
