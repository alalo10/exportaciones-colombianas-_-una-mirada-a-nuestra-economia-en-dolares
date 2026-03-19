# Exportaciones Colombianas — Una mirada a nuestra economía en dólares

**Proyecto Final — Estadística II**  
📚 Universidad Industrial de Santander  

**Autora:**
- Angela Lozano Pulido

---

## 📌 Descripción

Este proyecto analiza estadísticamente las exportaciones colombianas entre **2011 y 2024**, usando datos oficiales del **ANDA (Archivo Nacional de Datos del DANE)**. A través de cuatro fases de estudio, se aplican técnicas de inferencia estadística para responder preguntas reales sobre el comportamiento del comercio exterior colombiano, medido en dólares FOB.

---

## 🗂️ Fases del Proyecto

### 🔹 Fase 1 — Pruebas de Hipótesis
- **Una muestra, varianza desconocida:** Se contrasta si el valor reportado por el MINCIT para las exportaciones a EE.UU. en enero 2024 (960 millones de dólares) es consistente con la base de datos del DANE.
- **Dos muestras independientes:** Se compara si las exportaciones colombianas hacia EE.UU. en enero de 2023 y enero de 2024 fueron estadísticamente iguales.

### 🔹 Fase 2 — Pruebas de Bondad de Ajuste (Chi-cuadrado)
- **Prueba 1:** Se evalúa si el valor FOB exportado hacia EE.UU. en el periodo 2011–2024 sigue una distribución uniforme en el tiempo, contrastando con hallazgos históricos del Banco de la República.
- **Prueba 2:** Se analiza si el valor FOB exportado hacia países latinoamericanos en 2014–2023 se distribuye de forma uniforme entre los países de destino.

### 🔹 Fase 3 — Regresión Lineal Simple
- Se modela la relación entre el **peso neto de la carga (PNK)** y el **valor FOB en dólares** para exportaciones a EE.UU. en enero de 2024.
- Se aplica limpieza de datos y tratamiento de outliers para mejorar el ajuste del modelo.

### 🔹 Fase 4 — Regresión Lineal con Transformación de Potencia
- Se aplica una **transformación logarítmica** a los datos para capturar mejor la relación no lineal entre peso y valor FOB.
- El modelo de potencia resultante revela efectos de **economías de escala** en las exportaciones.

### 🔹 Series de Tiempo
- **Serie 1:** Evolución mensual del valor FOB promedio de todas las exportaciones colombianas (2011–2024).
- **Serie 2:** Frecuencia mensual de exportaciones desde Colombia hacia EE.UU. (2011–2024), identificando tendencias y cambios estructurales.

---

## 🗄️ Dataset

Los datos utilizados en este proyecto **no están incluidos en el repositorio** por su tamaño (432 MB).

Puedes acceder al archivo CSV ya limpio y listo para usar aquí:

📥 **[Descargar datos limpios — Google Drive](https://drive.google.com/file/d/1-ZJoichICsJBzFYdZz4ra5cUML-d0vPU/view?usp=sharing)**

### Origen de los datos
- **Fuente oficial:** ANDA — Archivo Nacional de Datos del DANE  
- **Portal:** [microdatos.dane.gov.co](https://microdatos.dane.gov.co/)  
- **Cobertura:** Exportaciones colombianas enero 2011 — diciembre 2024  

### Variables principales

| Variable | Descripción |
|---|---|
| `ANHO` | Año de la exportación |
| `MES` | Mes de la exportación |
| `COD_PAI4` | Código del país de destino (ej: `USA`, `MEX`) |
| `FOBDOL` | Valor FOB de la exportación en dólares |
| `PNK` | Peso neto de la carga en kilogramos |

> ⚠️ Para ejecutar el notebook, descarga el archivo y ubícalo en tu Google Drive en la ruta `MyDrive/ESTADISTICA II/`

---

## 🚀 ¿Cómo ejecutar el proyecto?

1. Clona este repositorio o descarga el archivo `.ipynb`.
2. Sube el notebook a **Google Colab**.
3. Conecta tu **Google Drive** y ubica los archivos `.csv` del DANE en la ruta:  
   `MyDrive/ESTADISTICA II/`
4. Ejecuta las celdas en orden.

> ⚠️ Los archivos de datos **no están incluidos** en este repositorio por su tamaño. Puedes descargarlos directamente desde el [portal ANDA del DANE](https://microdatos.dane.gov.co/).

---

## 📈 Principales Hallazgos

- Las exportaciones a EE.UU. en enero 2024 (~959M USD) son estadísticamente **diferentes** al valor oficial reportado por el MINCIT (960M), debido al gran tamaño muestral (n=4.627).
- Existe evidencia estadística de que las exportaciones a EE.UU. **aumentaron** entre enero 2023 (884M) y enero 2024 (959M).
- El valor FOB exportado **no se distribuye de forma uniforme** ni en el tiempo ni entre países latinoamericanos.
- La relación PNK–FOBDOL es positiva pero **sublineal** (β ≈ 0.54), lo que sugiere economías de escala.
- La frecuencia de exportaciones hacia EE.UU. mostró una **tendencia creciente sostenida** de 2011 a 2022, con una caída notable hacia finales de ese año.

---

<p align="center">
  Hecho con ❤️ en la Universidad Industrial de Santander · 2025
</p>
