# 🧮 Predictor de Gastos

Link to coolab: https://colab.research.google.com/drive/1BHZmJs_92C-paKWqq6809uxRFOyEcts1?usp=sharing
Este repositorio contiene un modelo de predicción de gastos desarrollado en Google Colab. El modelo utiliza un archivo `.xlsx` con registros de actividades y sus gastos para hacer predicciones sobre gastos futuros.

---

## 📝 Formato del archivo de registros

Para obtener predicciones precisas, es importante que tu archivo de registros siga este formato en Excel:

| Número | Fecha (dd/mm/aa) | Nombre actividad | Costo | Presupuesto | Tiempo invertido | Tipo | Momento | No. de personas |
| ------ | ---------------- | ---------------- | ----- | ------------ | ---------------- | ---- | ------- | --------------- |
| 1      | dd/mm/aa         | Nombre           | 0     | 0            | 0                | 1-6  | 1-3     | 1+              |

---

### 📊 Descripción de las variables

- **Costo:** Costo real de la actividad, en pesos.
- **Presupuesto:** Presupuesto disponible para la actividad, en pesos.
- **Tiempo invertido:** Minutos dedicados a realizar la actividad.
- **Tipo:** Número correspondiente al tipo de actividad:
  1. Alimentos/Salud
  2. Ahorro/Inversión
  3. Ejercicio/Deporte
  4. Entretenimiento/Ocio
  5. Académico
  6. Transporte
- **Momento:** Momento en que se realizó la actividad:
  - 1: Mañana
  - 2: Tarde
  - 3: Noche
- **No. de personas:** Cantidad de personas involucradas en la actividad.

---

## 🚀 Cómo usar el predictor

1. Sube tu archivo de registros `.xlsx` usando el botón de **Upload File** en Google Colab.
2. Asegúrate de tener al menos 100 registros para obtener mejores resultados.
3. Corre las celdas del notebook de Google Colab siguiendo el flujo del programa.
4. El modelo procesará los datos y mostrará los resultados de predicción de gastos.

---

## ⚙️ Requisitos

- Python 3.x
- Paquetes:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - openpyxl

Si quieres instalarlos manualmente:
```bash
pip install pandas numpy scikit-learn matplotlib openpyxl
