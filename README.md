# Documentación del Notebook: Análisis Terpel

## Descripción General
Este notebook contiene análisis y visualizaciones relacionadas con la producción y rentabilidad de Terpel. Utiliza datos almacenados en formatos como Parquet y Excel, y genera gráficos interactivos con Plotly para explorar tendencias y métricas clave.

### Funciones Principales
1. **`grafica_rentabilidad_mensual`**: Genera un gráfico de líneas que muestra la evolución mensual del margen de ganancia promedio.
2. **`grafica_dashboard_mensual`**: Crea un dashboard con subgráficos que incluyen:
   - Volumen producido.
   - Costo de materias primas.
   - Rentabilidad promedio.
3. **Exportación de Dashboard**: Genera un archivo HTML (`index.html`) que consolida las gráficas en un formato visualmente accesible.

---

## Instalación de Dependencias con `uv`
Este proyecto utiliza `uv` para la gestión de dependencias. A continuación, se describen los pasos para instalar las dependencias necesarias:

### 1. Crear un Entorno Virtual
Primero, crea un entorno virtual para aislar las dependencias del proyecto:
```bash
python -m venv venv
```

### 2. Activar el Entorno Virtual
Activa el entorno virtual:
- **Windows**:
  ```bash
  .\venv\Scripts\activate
  ```
- **Linux/Mac**:
  ```bash
  source venv/bin/activate
  ```

### 3. Instalar Dependencias con `uv`
Instala las dependencias especificadas en el archivo `pyproject.toml` utilizando `uv`:
```bash
uv install
```

### 4. Instalar Dependencias Adicionales
Si necesitas soporte para archivos Parquet, asegúrate de instalar `pyarrow` o `fastparquet`:
```bash
uv pip install pyarrow
```
O:
```bash
uv pip install fastparquet
```

---

## Ejecución del Notebook
1. Asegúrate de que todas las dependencias estén instaladas.
2. Abre el notebook en Visual Studio Code o Jupyter Notebook.
3. Ejecuta las celdas en orden para generar las visualizaciones y exportar el dashboard.

---

## Exportación del Dashboard
El dashboard consolidado se exporta como un archivo HTML en la carpeta `exported_dashboards` con el nombre `index.html`. Este archivo puede abrirse en cualquier navegador web para visualizar las gráficas interactivas.

---

## Notas Adicionales
- Si encuentras errores relacionados con dependencias, verifica que el entorno virtual esté activado y que las bibliotecas necesarias estén instaladas.
- Para soporte adicional, consulta la documentación de `uv` y las bibliotecas utilizadas en este proyecto.