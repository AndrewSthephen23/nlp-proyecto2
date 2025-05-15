# Proyecto 2 – Backpropagation Through Time y Modelos Seq2Seq

Este proyecto explora el entrenamiento de redes neuronales recurrentes (RNN) mediante el algoritmo **Backpropagation Through Time (BPTT)**, aplicadas a tareas de secuencia a secuencia (seq2seq). Se implementan modelos con y sin atención, abordando problemas como la explosión/desvanecimiento de gradientes y el *exposure bias* en la generación de secuencias.

## Objetivos

- Comprender el funcionamiento del algoritmo BPTT y técnicas como truncamiento y grad-clipping.
- Implementar modelos seq2seq básicos usando LSTM/GRU en PyTorch.
- Analizar el efecto del *teacher forcing* y el *exposure bias* en el rendimiento del modelo.
- Evaluar modelos con y sin regularización mediante técnicas como *dropout* recurrente.

## Técnicas utilizadas

- **Backpropagation Through Time (BPTT)**: Entrenamiento expandido en el tiempo para redes recurrentes.
- **Truncamiento y Clipping de gradientes**: Para mejorar estabilidad y evitar explosiones numéricas.
- **Modelos Seq2Seq**: Encoder-decoder con o sin atención.
- **Teacher Forcing**: Técnica de entrenamiento guiado.
- **Dropout Recurrente**: Regularización adaptada a secuencias.
- **BLEU & Edit Distance**: Para evaluar generación de secuencias.

## Métricas

- **Pérdida (Loss)**
- **Perplejidad**
- **BLEU Score**
- **Edit Distance**

## Actividades principales

1. Implementación básica de un modelo seq2seq sin atención.
2. Evaluación con y sin *teacher forcing* (p=1 y p=0).
3. Entrenamiento con truncamiento de BPTT para secuencias largas.
4. Aplicación de técnicas de regularización (dropout recurrente).
5. Generación de secuencias y análisis del *exposure bias*.

## Estructura del repositorio

- `src/`: Código fuente (modelos, entrenamiento, utilidades).
- `notebooks/`: Cuadernos Jupyter con visualizaciones y pruebas.
- `data/`: Conjuntos de datos sintéticos o reales usados para entrenar.
- `informes/`: Documentación y análisis por etapas.
- `docker/`: Archivos para levantar el entorno con Docker.

## Requisitos

Instalar las dependencias con:

```bash
pip install -r requirements.txt

