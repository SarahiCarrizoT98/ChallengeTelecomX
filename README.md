# TelecomX_LATAM-1
# 📊 Análisis de Evasión de Clientes (Churn) - Telecomunicaciones

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Seaborn](https://img.shields.io/badge/Seaborn-blue?style=for-the-badge&logo=python&logoColor=white)

## 📋 Descripción del Proyecto
Este proyecto aborda el problema de la **evasión de clientes (Churn)** en una compañía de telecomunicaciones. A través de un análisis exploratorio de datos (EDA) y técnicas de transformación de variables, se identifican los factores críticos que influyen en la salida de los usuarios para proponer estrategias de retención basadas en datos.

---

## 🚀 Estructura del Análisis

### 1. Limpieza y Transformación
* **Saneamiento:** Eliminación de valores nulos en cargos totales.
* **Feature Engineering:** Creación de la métrica `Cuentas_Diarias` (Cargo Mensual / 30).
* **Localización:** Traducción integral de variables al español y renombrado de columnas.
* **Codificación:** Conversión de variables categóricas a binarias ($1$ y $0$) para análisis estadístico.

### 2. Análisis Exploratorio (EDA)
Se utilizaron visualizaciones avanzadas para identificar patrones de comportamiento:
* **Distribución de Evasión:** El **26.6%** de la base de clientes presenta estado de evasión.
<ul>
<img src="./Images/1 Distribucion-Clientes-Evasion.png" style="width: 60%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1); margin: 15px 0;">
</ul>

* **Análisis por Categoría:** Identificación de mayor riesgo en contratos **Mensuales** y métodos de pago por **Cheque Electrónico**.
<ul>
<img src="./Images/2 Distribucion-Clientes-Evasion-Cualitativa.png" style="width: 100%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1); margin: 15px 0;">
</ul>

* **Variables Numéricas:** Uso de **Boxplots** para comparar Antigüedad vs. Cargos Mensuales.
<ul>
<img src="./Images/3 Distribucion-Clientes-Evasion-Cuantitativa.png" style="width: 100%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1); margin: 15px 0;">
</ul>



---

## 📉 Principales Hallazgos (Insights)

<div align="center">
  <table style="width: 100%; text-align: center;">
    <tr>
      <th style="background-color: #45B39D; color: white;">Factor de Retención</th>
      <th style="background-color: #EC7063; color: white;">Factor de Riesgo (Churn)</th>
    </tr>
    <tr>
      <td>Antigüedad alta (> 24 meses)</td>
      <td>Contratos Mes a Mes</td>
    </tr>
    <tr>
      <td>Contratos Bianuales</td>
      <td>Cargos Mensuales > $80</td>
    </tr>
    <tr>
      <td>Pagos Automáticos</td>
      <td>Uso de Fibra Óptica (Insatisfacción/Precio)</td>
    </tr>
  </table>
</div>

---

## 🛠️ Visualizaciones Destacadas

### Matriz de Correlación
Se implementó una paleta de colores coherente con la identidad visual del proyecto (`#45B39D` para retención y `#EC7063` para evasión).
* **Correlación Crítica:** La antigüedad (`-0.35`) es el factor preventivo más fuerte.
<ul>
<img src="./Images/4 matriz-correlacion.png" style="width: 100%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1); margin: 15px 0;">
</ul>

---

## 💡 Recomendaciones Estratégicas

1. **Fidelización Temprana:** Implementar programas de beneficios específicos para clientes en sus primeros 12 meses de vida.
2. **Migración de Contratos:** Crear campañas para convertir clientes de planes mensuales a contratos anuales mediante descuentos progresivos.
3. **Auditoría de Fibra Óptica:** Investigar la causa de alta evasión en usuarios de fibra (¿Calidad de servicio o precio?).
4. **Optimización de Cobros:** Incentivar el uso de métodos de pago automáticos para reducir la fricción del pago manual.

---

## 🛠️ Requisitos
```bash
pandas
numpy
matplotlib
seaborn
```
---
**Proyecto Sarahi Carrizo Trejo**
