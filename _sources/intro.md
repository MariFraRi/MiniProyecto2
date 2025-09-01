# **Mini Proyecto 2: Predicción y Clasificación de Autos Usados**

## **Integrantes**
- Mariana Franco
- Jerónimo Domínguez
- Juan Andrés Ramos

## **Contextualización del Proyecto**
El propósito de este proyecto es **analizar y modelar precios de autos usados** publicados en la plataforma **Craigslist**.  
Además de predecir el **precio estimado de un vehículo**, se busca clasificar la **demanda** de un auto (alta o baja), con base en sus características principales.

---
## **Contexto**
**Craigslist** es la colección más grande del mundo de vehículos usados en venta.  
Sin embargo, es muy difícil recopilar todos estos anuncios en un mismo lugar.  
Para un proyecto escolar se construyó un **scraper** que luego se amplió, creando este dataset que incluye cada publicación de vehículos usados dentro de los Estados Unidos en Craigslist.

---

## **Descripción del Dataset**

El dataset proviene de **Craigslist Cars and Trucks Dataset (Kaggle)** y contiene información de más de **426,000 vehículos** listados en diferentes regiones de Estados Unidos.  
Cuenta con **26 variables**, tanto numéricas como categóricas, relacionadas con el vehículo, el anuncio y su localización.  

- **Tamaño:** 426,880 registros × 26 columnas  
- **Fuente:** Publicaciones en línea de Craigslist  
- **Periodo de recolección:** Principalmente hasta mayo de 2021  

---

## **Variables del Dataset**

| Variable        | Tipo       | Descripción |
|-----------------|-----------|-------------|
| `id`            | Entero    | Identificador único del anuncio |
| `url`           | Texto     | Enlace al anuncio original (irrelevante para análisis) |
| `region`        | Categórica| Región donde se publica el anuncio |
| `region_url`    | Texto     | URL de la región (irrelevante) |
| `price`         | Numérica  | Precio listado del vehículo (variable objetivo principal) |
| `year`          | Numérica  | Año de fabricación |
| `manufacturer`  | Categórica| Marca del vehículo |
| `model`         | Categórica| Modelo del vehículo |
| `condition`     | Categórica| Estado físico del auto (ej. "excellent", "good") |
| `cylinders`     | Categórica| Número de cilindros del motor |
| `fuel`          | Categórica| Tipo de combustible (gasolina, diésel, eléctrico, etc.) |
| `odometer`      | Numérica  | Kilometraje recorrido (en millas) |
| `title_status`  | Categórica| Estado legal del título (ej. "clean", "salvage") |
| `transmission`  | Categórica| Tipo de transmisión (manual, automática) |
| `VIN`           | Texto     | Número de identificación del vehículo (puede faltar) |
| `drive`         | Categórica| Tracción (4WD, FWD, RWD) |
| `size`          | Categórica| Tamaño del vehículo (compacto, mediano, grande) |
| `type`          | Categórica| Tipo de vehículo (sedán, SUV, camioneta, etc.) |
| `paint_color`   | Categórica| Color del auto |
| `image_url`     | Texto     | Imagen del vehículo (irrelevante) |
| `description`   | Texto     | Descripción del anuncio (texto libre, difícil de usar directamente) |
| `county`        | Texto     | Condado (poco útil) |
| `state`         | Categórica| Estado en EE.UU. |
| `lat`, `long`   | Numérica  | Coordenadas geográficas |
| `posting_date`  | Temporal  | Fecha de publicación del anuncio |

---

## **Observaciones importantes**

- El dataset tiene **valores faltantes** en variables claves.
- Existen **outliers** en `price`. 
- Varias columnas (`url`, `image_url`, `description`, `region_url`) no son útiles para modelar y probablemente se descarten.  
- Se trabaja en dos objetivos principales:  

  1. **Regresión:** Estimar el precio de un vehículo (`price`).  
  2. **Clasificación:** Determinar si un auto tiene **alta o baja demanda**, usando reglas de negocio (ej. número de publicaciones, precio competitivo). 

```{tableofcontents}
```
