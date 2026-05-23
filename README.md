# Sistema Híbrido de Predicción de PM2.5 mediante FFT y Random Forest (Riobamba)

## 📝 Descripción del Proyecto
Este proyecto implementa un modelo predictivo híbrido de alta precisión para la concentración de partículas finas (PM2.5) en la ciudad de Riobamba. La metodología integra técnicas de procesamiento de señales mediante la Transformada Rápida de Fourier (FFT) para aislar ciclos temporales dominantes, combinándolas con algoritmos de Machine Learning (Random Forest Regressor) para optimizar la precisión predictiva en comparación con modelos meteorológicos tradicionales.

## 🚀 Arquitectura y Fases del Código
El script adjunto se desarrolla de manera secuencial cumpliendo las siguientes etapas de ingeniería:
1. **Fase 1 y 2 (Limpieza de Datos):** Simulación de 8,760 observaciones horarias y tratamiento de valores nulos mediante interpolación lineal.
2. **Fase 3 (Análisis Espectral - FFT):** Transformación de la señal al dominio de la frecuencia para extraer las 6 componentes dominantes (4380h, 168h, 84h, 24h, 12h, 8h).
3. **Fase 4 y 5 (Modelado y Entrenamiento):** Implementación comparativa del modelo convencional frente al modelo híbrido enriquecido con variables espectrales.
4. **Fase 6 (Validación Gráfica):** Despliegue de métricas de control (MSE) y evaluación visual de residuos.

## 📊 Requerimientos Técnicos e Instalación
Para ejecutar este pipeline analítico, es necesario contar con Python 3.11 y las siguientes librerías científicas:
```bash
pip install numpy pandas scipy scikit-learn matplotlib seaborn
