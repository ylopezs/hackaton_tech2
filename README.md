# Resumen del Proyecto: Modelo de predicción de fallas en la maquinaria

## **Equipo**  
**Nombre del equipo:** Starlight  
## **Integrantes**
Luisa Granada Usme
Luz Marina Getial
Yonatan Alberto López Sierra

## **Descripción del Proyecto**  
**Problema abordado:** Ineficiencia en la producción debido a fallas no planificadas en maquinaria industrial.  
**Variable objetivo:** `fallo_detectado` (binaria: 1 = fallo, 0 = sin fallo).  
**Sector objetivo:** Manufactura e industria, donde las paradas no planificadas impactan la producción y calidad.  

## **Dataset**  
- **Origen:** Registros operativos de sensores industriales (proporcionados por la universidad).  
- **Variables:**  
  - Operativas: temperatura, vibración, humedad, consumo energético, eficiencia, tiempo de ciclo.  
  - Identificación: operador, máquina, producto, turno.  
  - Fallas: `fallo_detectado`, `tipo_fallo`.  
- **Tamaño:** 6,000 registros y 18 columnas.  
- **Preprocesamiento:** Limpieza de duplicados, imputación de nulos, tratamiento de outliers, escalado y codificación.  

## **Modelo Predictivo**  
- **Algoritmo seleccionado:** Random Forest (tras evaluar regresión logística y árbol de decisión).  
- **Rendimiento:** 90% de precisión (9 de cada 10 predicciones correctas).  
- **Supuestos:**  
  - Datos registrados correctamente y sincronizados.  
  - Distribución histórica de fallos representativa del futuro.  

## **Visualizaciones**  
1. **Matriz de confusión:** Comparación entre predicciones y valores reales.  
2. **Curva ROC:** Evalúa sensibilidad y especificidad del modelo.  
3. **Importancia de variables:** Ranking de variables más influyentes (ej. consumo de energía, vibración).  
4. **Gráfico real vs. predicho:** Dispersión de predicciones frente a datos reales.  
- **Herramientas:** Matplotlib, Seaborn, scikit-learn.  

## **Recomendaciones Estratégicas**  
1. **Alertas automáticas:** Activar mantenimiento preventivo al detectar patrones de fallo (ej. picos de vibración/temperatura).  
2. **Enfoque en variables clave:** Monitorear consumo de energía, eficiencia y vibración para predecir fallos con mayor precisión.  

## **Valor Diferencial**  
- Combinación de Random Forest con análisis visual (heatmap, importancia de variables) para decisiones predictivas claras.  
- **Escalabilidad:** Incorporar sensores en tiempo real y gemelos digitales para simulaciones avanzadas.  

## **Entregables**  
- Dataset limpio y documentado.  
- Notebook de análisis.  
- Visualizaciones clave (matriz de confusión, curva ROC).  
- Reporte con recomendaciones.  
- Repositorio en GitHub.  
