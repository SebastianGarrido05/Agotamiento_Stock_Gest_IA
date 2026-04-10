# Agotamiento_Stock_Gest_IA
Este proyecto tiene como finalidad desarrollar un sistema de predicción de agotamiento de stock
---

## Componentes del sistema
- **Scripts de procesamiento**: ingesta, limpieza, transformación y validación de datos.
- **Base de datos PostgreSQL**: para la carga y consulta estructurada de los datasets.
- **Metabase (opcional)**: dashboard de visualización de resultados.
- **Machine learning**:Modelado, entrenamiento y evaluación
- **Documentación**: diseño técnico completo + planificación.
---

## Tecnologías utilizadas

- VS code
- PostgreSQL
- Docker
- Google Android  
- Git / GitHub  
- Trello / Jira

---

## Pipeline implementado

| Etapa | Descripción |
|-------|-------------|
| 1. Diseño e instalación | Estructura de carpetas, setup del entorno, definición de herramientas |
| 2. Ingesta | Lectura desde CSV (hoja de cálculo google ), carga a memoria |
| 3. Limpieza | Eliminación de duplicados, tratamiento de nulos, revisión de tipos |
| 4. Transformación | Creación de variables como días sin reposición, tasa de ventas, etc. |
| 5. Validación | Revisión de rangos, tipos, coherencia; validación básica |
| 6. Carga en PostgreSQL | Subida del dataset limpio y validado a la base de datos local |
| 7. Entrenamiento IA | Clasificación binaria con scikit-learn para variable `SeAgotara` |
| 8. Evaluación | Métricas como accuracy, recall; revisión de logs de ejecución |
| 9. Visualización | Panel con predicciones, stock proyectado y alertas según la predicción de la IA |




---

## 📂 Estructura del repositorio

```
agotamiento-stock/
├── README.md
├── docs/
│   └── diseño_tecnico.pdf
├── scripts/
│   ├── ingesta.py
│   ├── limpieza.py
│   ├── transformacion.py
│   └── entrenamiento.py
├── data/
│   ├── stock.csv
│   └── productos_ventas.csv
├── dashboards/
│   └── foto_inventada.png
```

---


## Cómo ejecutar el sistema (entorno ya instalado)

1. Clonar el repositorio  
   `git clone https://github.com/SebastianGarrido05/Agotamiento_Stock_Gest_IA.git`

2. Entrar a la carpeta del proyecto  
   `cd agotamiento-stock`

3. Ejecutar el pipeline manualmente por etapas  
   Ejemplo:  
   `python scripts/ingesta.py`  
   `python scripts/limpieza.py`  
   `python scripts/entrenamiento.py`

4. Visualizar los resultados y métricas desde consola o dashboard

---

## Documentación técnica

El documento de diseño técnico está disponible en:  
[`docs/Diseno_Tecnico.pdf`](docs/Diseno_Tecnico.pdf)

---

## Equipo

- Martin Calderon  – Procesamiento y limpieza  
- Dylan Cruz – Modelado y entrenamiento  
- Sebastian Garrido – Visualización y documentación

