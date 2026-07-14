
---

#  Proyecto: Cs50 Shopping (Predicción de Revenue con KNN) 
Modelo de Machine Learning — CS50’s Introduction to Artificial Intelligence with Python

##  Descripción  
Este proyecto implementa un modelo de **k-nearest neighbors (KNN)** para predecir si un usuario generará **Revenue** en una tienda online, basándose en datos de navegación web.

El programa:

1. Carga datos desde un archivo CSV.  
2. Convierte cada fila en evidencia numérica y etiquetas.  
3. Divide los datos en entrenamiento y prueba.  
4. Entrena un modelo KNN con **k = 1**.  
5. Evalúa el modelo calculando:  
   - **Sensibilidad (True Positive Rate)**  
   - **Especificidad (True Negative Rate)**  
6. Muestra los resultados por consola.

---

##  Estructura del proyecto

```
shopping/
│── shopping.py
│── shopping.csv
│── README.md
```

---

##  Requisitos

- Python 3.10+
- scikit-learn
- pip

Instalación de dependencias:

```bash
pip install scikit-learn
```

---

##  Uso

Ejecuta el programa desde la terminal:

```bash
python3 shopping.py shopping.csv
```

Salida esperada:

```
Correct: XXXX
Incorrect: XXXX
True Positive Rate: XX.XX%
True Negative Rate: XX.XX%
```

---

##  Dataset

El archivo `shopping.csv` contiene información sobre sesiones de usuarios en un sitio web.  
Cada fila incluye:

- Actividad administrativa  
- Duración de páginas informativas  
- Páginas relacionadas con productos  
- Bounce rates  
- Exit rates  
- Page values  
- Día especial  
- Mes  
- Sistema operativo  
- Navegador  
- Región  
- Tipo de tráfico  
- Tipo de visitante  
- Si fue fin de semana  
- Revenue (TRUE/FALSE)

El programa transforma estos valores en tipos numéricos adecuados para el modelo.

---

##  Modelo

Se utiliza un **KNN con k = 1**, implementado con:

```python
KNeighborsClassifier(n_neighbors=1)
```

Este modelo clasifica cada usuario según el vecino más cercano en el espacio de características.

---

##  Métricas

El programa calcula:

### **Sensibilidad (True Positive Rate)**  
Proporción de compradores reales correctamente identificados.

### **Especificidad (True Negative Rate)**  
Proporción de no compradores correctamente identificados.

---

##  Pruebas

El proyecto pasa todas las pruebas de:

-  **check50 (11/11)**  
-  **style50 (0.99)**  

Cumpliendo completamente los requisitos del curso.

---

##  Autor

Proyecto realizado por **Zene**  
Curso: *CS50’s Introduction to Artificial Intelligence with Python*  
Año: 2026

---
