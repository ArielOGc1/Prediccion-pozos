# 🛢️ Selección de Pozos Petroleros

## 📌 Descripción
Este proyecto consiste en desarrollar un modelo para **identificar las mejores ubicaciones donde abrir 200 pozos petroleros** en tres regiones.  
Utilicé **regresión lineal** para predecir el volumen de reservas y la técnica de **bootstrapping** para analizar riesgos y beneficios.

---

## ✅ Objetivos
- Predecir el **volumen de reservas** en pozos nuevos.
- Seleccionar los **200 pozos con mayores reservas estimadas** por región.
- Evaluar beneficios y riesgos para determinar la **región más rentable**.

---

## ⚙️ Metodología
- Procesé datos de **500 pozos por región**.
- Entrené un modelo de **regresión lineal** para estimar reservas.
- Calcule el **beneficio esperado** considerando:
  - Presupuesto: **$100M** para 200 pozos.
  - Ingreso por barril: **4.5 USD** (4500 USD por 1000 barriles).
- Apliqué **bootstrapping (1000 iteraciones)** para:
  - Beneficio promedio.
  - Intervalo de confianza (95%).
  - Riesgo de pérdidas (< 2.5%).

---

## 🛠 Tecnologías
- **Lenguaje:** Python  
- **Librerías:** pandas, numpy, scikit-learn, matplotlib  
- **Técnicas:** Regresión Lineal, Bootstrapping, Análisis Estadístico  

---

## 📊 Resultado Esperado
Seleccionar la región que cumpla:
- **Mayor beneficio promedio**.
- **Riesgo de pérdidas < 2.5%**.
