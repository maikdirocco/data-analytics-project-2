# Segundo Proyecto - Data Analytics

# Proyecto de Base de Datos - Ventas de Autos Usados en Emiratos Árabes Unidos

Este repositorio contiene la implementación de un sistema de base de datos relacional diseñado para gestionar y analizar información sobre las ventas de autos usados en Emiratos Árabes Unidos. El proyecto está enfocado en ofrecer una solución escalable y eficiente para el almacenamiento y análisis de datos clave relacionados con vehículos.

## Contenido del Proyecto

### Link al documento Word editable que se pide en la consigna del proyecto
### https://1drv.ms/w/c/86865b5012ac551c/ETcnE2i-ciRMtIdpOopz5HcB7w2ja4jVZmTGMNrxLf5FmA?e=ygw6bb

### 1. Objetivo del Proyecto
El objetivo principal fue crear una base de datos que permita:
- **Gestión de datos**: Almacenar información detallada de los vehículos, como marca, modelo, precio, kilometraje y más.
- **Análisis de ventas**: Identificar tendencias del mercado, patrones de compra y generar predicciones de precios.

### 2. Alcance
El sistema ofrece funcionalidades para:
- Identificar tendencias en las ventas basadas en atributos clave (precio, año de fabricación, etc.).
- Analizar la demanda de vehículos en distintas ubicaciones.
- Evaluar la relación entre kilometraje y precio de venta.
- Generar informes personalizados sobre el rendimiento de ventas considerando múltiples variables, como tipo de combustible o condición del vehículo.

### 3. Diagrama de Entidad-Relación (ERD)
Se incluye un diagrama profesional que representa:
- Las relaciones entre las tablas.
- Llaves primarias y foráneas para asegurar integridad referencial.
- Una visión clara de la estructura general de la base de datos.

### 4. Tablas y Relaciones
El modelo relacional incluye las siguientes tablas:
- **Vehicle**: Información general del vehículo, con referencias a tablas como `Model`, `BodyType` y `FuelType`.
- **Model y Make**: Relación jerárquica entre modelos y marcas de autos.
- **Características del Vehículo**: Tablas como `Color`, `Cylinders`, `Transmission`, y `BodyType` que definen atributos clave.
- **Ubicación y Condición**: Información sobre la ubicación del vehículo (`Location`) y su estado (`VehicleCondition`).

**Relaciones principales**:
- Cada vehículo está asociado a un modelo específico (`Vehicle ↔ Model`).
- Las marcas (`Make`) agrupan varios modelos (`Model ↔ Make`).
- Las tablas independientes (como `Color` y `BodyType`) actúan como catálogos referenciados desde `Vehicle`.

### 5. Detalle de las Columnas
Cada tabla está definida con las siguientes columnas:
- **Vehicle**: Incluye `VehicleID` (PK), `ModelID` (FK), `Year`, `Price`, `Mileage`, entre otros.
- **Model**: `ModelID` (PK), `ModelName`, y `MakeID` (FK).
- **BodyType, Transmission, y demás atributos**: Cada una contiene una columna ID primaria y un campo descriptivo.

Se especificaron tipos de datos optimizados para cada atributo, asegurando consistencia y escalabilidad.

### 6. Consideraciones Técnicas
- **Normalización**: La base de datos está completamente normalizada para evitar redundancias.
- **Integridad referencial**: Todas las claves foráneas están definidas para garantizar la consistencia entre tablas.

### 7. Aplicación del Proyecto
Este sistema está pensado para:
- **Usuarios finales**: Analistas de datos y gerentes de ventas de autos usados.
- **Niveles de análisis**:
  - Operativo: Consultas rápidas y análisis de ventas individuales.
  - Táctico: Identificación de patrones regionales y de demanda.
  - Estratégico: Predicciones y decisiones basadas en tendencias del mercado.

---
