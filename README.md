# 🧠 Proyecto Final – EDA + Dashboard Comercial  

## 📌 Descripción General  
Este proyecto presenta un **análisis exploratorio de datos (EDA)** y la construcción de un **Dashboard interactivo en Excel**, con el objetivo de obtener información clave sobre el rendimiento comercial, comportamiento de clientes y eficiencia en los métodos de envío.  

El flujo de trabajo abarca desde la **limpieza y transformación de datos crudos** hasta la **generación de indicadores de negocio**, siguiendo buenas prácticas de programación y análisis de datos.  

---

## 🗂️ Estructura del Proyecto  

```
PROYECTO_FINAL/
│
├── data/
│   ├── archivos_final/
│   │   ├── dashboard_final.xlsx      → Dashboard interactivo final
│   │   └── dataset_final.xlsx        → Dataset limpio y consolidado
│   ├── archivos_origen/
│   │   ├── customers_origen.xlsx     → Datos originales de clientes
│   │   └── orders_origen.xlsx        → Datos originales de pedidos
│
├── doc_proyecto/
│   └── Descripción del proyecto.docx → Documentación descriptiva
│
├── notebooks/
│   ├── 01_analisis_pre_customers.ipynb → Análisis exploratorio inicial de clientes
│   ├── 02_analisis_pre_orders.ipynb    → Análisis exploratorio inicial de pedidos
│   ├── 03_limpieza_datasets.ipynb      → Limpieza, depuración y unión de datasets
│   └── 04_EDA_final.ipynb              → Análisis EDA completo y preparación final
│
├── .gitattributes
└── .gitignore
```

---

## 🧩 Flujo de Trabajo  

### 1️⃣ Análisis Preliminar  
- Exploración inicial de los datasets de **clientes** y **pedidos**.  
- Identificación de inconsistencias, valores nulos y duplicados.  
- Revisión de las relaciones clave entre las tablas.  

📘 *Notebooks:*  
`01_analisis_pre_customers.ipynb` y `02_analisis_pre_orders.ipynb`

---

### 2️⃣ Limpieza y Preparación de Datos  
- Eliminación de columnas innecesarias y corrección de errores.  
- Estandarización de nombres de columnas y formatos.  
- Unión de los datasets mediante el identificador común (`customer_id`).  
- Generación del **dataset final** (`dataset_final.xlsx`).

🧹 *Notebook:* `03_limpieza_datasets.ipynb`  

> 💡 **Buena práctica:**  
> Se respetó la trazabilidad de los datos, conservando una copia original (`archivos_origen/`) y generando un conjunto limpio final (`archivos_final/`).

---

### 3️⃣ Análisis Exploratorio (EDA)  
- Análisis descriptivo y visual de las principales variables:  
  - Comportamiento de ventas y pedidos.  
  - Distribución de clientes por región y categoría.  
  - Identificación de patrones de devolución.  
- Generación de insights relevantes para el área comercial.  

📊 *Notebook:* `04_EDA_final.ipynb`

#### 🧮 Dataframes de Apoyo (EDA)

Durante el análisis se generaron varios **dataframes de trabajo** para profundizar en la exploración de los datos.  
Estos incluían métricas agregadas, análisis de devoluciones, comportamiento por categorías y segmentación por método de envío.  

> 🔍 **Importante:**  
> Aunque aportaron valor al análisis descriptivo y permitieron validar insights, **no fueron utilizados directamente en el Dashboard final**, ya que su propósito fue exclusivamente analítico dentro del notebook `04_EDA_final.ipynb`.


> 📘 **Librerías utilizadas:**  
> `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `warnings`, `os`, `pathlib`.

---

### 4️⃣ Dashboard Final  
Se desarrolló un **Dashboard en Excel** (`dashboard_final.xlsx`) que resume las métricas clave del negocio.  

#### 🔹 Indicadores Principales  
| Métrica | Valor |
|:--------|-------:|
| 💰 **Ventas Totales** | 38.636.959,59 € |
| 📦 **Pedidos Totales** | 55.000 |
| 👥 **Clientes Únicos** | 5.000 |
| 💳 **Ticket Medio (€)** | 702,49 |
| 🔁 **Tasa de Devolución** | 5,02 % |

#### 📈 Visualizaciones Incluidas  
- **Ventas por categoría** → rendimiento por línea de producto.  
- **Pedidos por región** → concentración geográfica.  
- **Método de envío** → preferencia logística.  
- **Histórico de devoluciones** → evolución temporal.  
- **Tasa de devolución por método de envío** → análisis cruzado entre servicio y devoluciones.  

📸 **Vista del Dashboard:**  

[![dash.png](https://i.postimg.cc/0yNKm9bQ/dash.png)](https://postimg.cc/rKvp2XGX)


---

## 🧠 Principales Hallazgos  
- Las **ventas más altas** se concentran en categorías como *Home* y *Office Supplies*.  
- El **método de envío “Standard”** domina la operativa (≈70% de los pedidos).  
- Las **regiones centrales** presentan un volumen de pedidos mayor, aunque también una **tasa de devolución más alta**.  
- El **ticket medio de 702,49 €** y la **tasa de devolución del 5 %** sugieren una cartera de clientes sólida, pero con margen de mejora en satisfacción posventa.

---

## ⚙️ Buenas Prácticas Implementadas  
- Uso de **nombres de variables claros y consistentes**.  
- Separación por **etapas y notebooks** según propósito.  
- Documentación de cada bloque de código con comentarios.  
- **Control de versiones** con Git y archivo `.gitignore`.  
- Conservación de datasets originales y finales para garantizar **reproducibilidad**.  

---

## 🧰 Librerías Principales  

| Tipo | Librerías |
|------|------------|
| Análisis de datos | `pandas`, `numpy` |
| Visualización | `matplotlib`, `seaborn`, `plotly` |
| Soporte / Sistema | `os`, `pathlib`, `warnings` |

---

## 📦 Resultados Entregables  
- 🗃️ **Dataset final:** `dataset_final.xlsx`  
- 📊 **Dashboard:** `dashboard_final.xlsx`  
- 📓 **Notebooks EDA:** todo el flujo de análisis reproducible  
- 📄 **Documentación:** `Descripción del proyecto.docx`

---

## 🚀 Conclusión  
Este proyecto demuestra un flujo completo de **Data Cleaning → EDA → Visualización Ejecutiva**, transformando datos dispersos en **información útil para la toma de decisiones**.  

El **dashboard final** permite monitorizar los principales KPIs comerciales, detectar oportunidades de mejora en los métodos de envío y analizar el comportamiento del cliente con una perspectiva global.  

> 💬 *“El poder del dato no está en recolectarlo, sino en transformarlo en decisiones.”*

---

## 🧑‍💻 Autor  
**Hugo Pérez Romero**  
Data Analyst | SQL | Python | Dashboard Design  
