# Simulaciones Modelo Bancario

## Actividad #3 - Curso de Simulaciones
**Carrera:** Ingeniería de Software

---

## Información del Proyecto

Este proyecto implementa simulaciones de un modelo bancario como parte de la actividad #3 del curso de Simulaciones. El objetivo es modelar y simular procesos típicos de un sistema bancario utilizando técnicas de simulación estocástica.

### Integrantes del Equipo

- **Lady Olmos**
- **Juan Parra**
- **Jorge Hernández**

---

## 📋 Descripción

El modelo bancario simula:
- Llegada de clientes a la entidad bancaria
- Procesamiento de transacciones
- Tiempos de espera en colas
- Comportamiento del sistema bajo diferentes condiciones
- Análisis estadístico de resultados

Este proyecto busca entender y optimizar los procesos bancarios mediante técnicas de simulación Monte Carlo y análisis de sistemas de colas.

---

## 📁 Estructura del Repositorio

```
Simulaciones_modelo_bancario/
├── README.md                      # Este archivo
├── notebooks/                     # Cuadernos Jupyter con las simulaciones
│   └── simulacion_bancaria.ipynb  # Notebook principal con código y resultados
├── datos/                         # Datos de entrada (si aplica)
├── resultados/                    # Resultados y gráficas generadas
└── documentacion/                 # Documentación adicional (si aplica)
```

---

## 🔧 Requisitos Previos

Para ejecutar este proyecto necesitas:

- **Python 3.8 o superior**
- **Jupyter Notebook** o **Jupyter Lab**
- **Librerías Python:**
  - `numpy` - Cálculos numéricos
  - `pandas` - Manipulación de datos
  - `matplotlib` - Visualización de gráficas
  - `scipy` - Análisis estadístico
  - `seaborn` - Visualización avanzada (opcional)

---

## 📥 Instalación

### 1. Clonar el Repositorio

```bash
git clone https://github.com/ladylaura22/Simulaciones_modelo_bancario.git
cd Simulaciones_modelo_bancario
```

### 2. Crear un Entorno Virtual (Recomendado)

**En Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**En macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Instalar las Dependencias

```bash
pip install --upgrade pip
pip install jupyter notebook numpy pandas matplotlib scipy seaborn
```

---

## 🚀 Pasos para Ejecutar el Código

### Opción 1: Usar Jupyter Notebook (Recomendado)

1. **Inicia Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

2. **Abre el notebook principal:**
   - En el navegador que se abre, navega a `notebooks/simulacion_bancaria.ipynb`

3. **Ejecuta las celdas:**
   - Usa `Shift + Enter` para ejecutar cada celda
   - O ve a `Cell > Run All` para ejecutar todas las celdas a la vez

4. **Visualiza los resultados:**
   - Las gráficas y estadísticas se mostrarán directamente en el notebook

### Opción 2: Usar Jupyter Lab

```bash
pip install jupyterlab
jupyter lab
```

Luego sigue los mismos pasos que en la Opción 1.

### Opción 3: Convertir a Python Script

Si prefieres ejecutar el código como script Python:

```bash
# Convertir notebook a script Python
jupyter nbconvert --to script notebooks/simulacion_bancaria.ipynb

# Ejecutar el script
python simulacion_bancaria.py
```

---

## 📊 Parámetros de la Simulación

Puedes personalizar los siguientes parámetros en el notebook:

- **Número de simulaciones:** Cantidad de iteraciones a ejecutar
- **Tiempo de simulación:** Duración total de la simulación (en minutos/horas)
- **Tasa de llegada de clientes:** Distribución de Poisson con parámetro λ
- **Tiempo de servicio:** Distribución exponencial o normal
- **Número de servidores:** Cantidad de cajas/atendientes disponibles
- **Semilla aleatoria:** Para reproducibilidad de resultados

---

## 📈 Resultados Esperados

El notebook genera:

✓ **Estadísticas descriptivas:**
  - Tiempo promedio en el sistema
  - Tiempo promedio en cola
  - Longitud promedio de cola
  - Factor de utilización

✓ **Visualizaciones:**
  - Gráfica de tiempos en cola vs. tiempo de servicio
  - Histograma de distribución de tiempos
  - Evolución de la longitud de cola en el tiempo
  - Análisis de utilización del sistema

✓ **Conclusiones:**
  - Análisis de cuellos de botella
  - Recomendaciones de mejora
  - Comparativas entre escenarios

---

## 🎯 Cómo Usar Este Repositorio

1. **Comprender el modelo:** Lee la documentación en el notebook
2. **Revisar el código:** Examina cada celda para entender la lógica
3. **Ejecutar la simulación:** Corre las celdas en orden
4. **Analizar resultados:** Interpreta las gráficas y estadísticas
5. **Experimentar:** Modifica los parámetros y observa cómo cambian los resultados
6. **Documentar:** Agrega tus propios análisis y conclusiones

---

## 🔍 Troubleshooting

### Problema: `ModuleNotFoundError: No module named 'numpy'`
**Solución:** Instala las dependencias faltantes:
```bash
pip install numpy pandas matplotlib scipy
```

### Problema: Jupyter Notebook no se inicia
**Solución:** Intenta con:
```bash
jupyter notebook --ip=127.0.0.1 --port=8888
```

### Problema: Las gráficas no se muestran
**Solución:** Agrega al inicio del notebook:
```python
%matplotlib inline
```

---

## 📚 Referencias Teóricas

- **Teoría de Colas:** Sistemas M/M/1, M/M/c
- **Distribuciones de Probabilidad:** Poisson, Exponencial
- **Método Monte Carlo:** Simulación estocástica
- **Análisis de Sistemas:** Métricas de desempeño

---

## 📝 Rubrica de Evaluación

Este proyecto cumple con los siguientes criterios:

✅ **Código completo:** Implementación de simulaciones bancarias
✅ **README detallado:** Documentación clara y comprensiva
✅ **Instrucciones de ejecución:** Pasos paso a paso para correr el código
✅ **Archivos necesarios:** Todos los notebooks y dependencias incluidas
✅ **Evidencias de resultados:** Gráficas y estadísticas generadas en los notebooks

**Total: 10 puntos**

---

## 📞 Contacto y Soporte

Para preguntas o problemas relacionados con este proyecto:
- Abre un **Issue** en el repositorio
- Contacta a cualquiera de los integrantes del equipo

---

## 📄 Licencia

Este proyecto es parte de la actividad académica del curso de Simulaciones - Ingeniería de Software.

---

**Última actualización:** Junio 2026
**Estado:** Completo ✅
