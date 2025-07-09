# machine-learnig
# 🎯 CS:GO Round Prediction

Este proyecto aplica técnicas de **Machine Learning** para predecir el resultado de una ronda en el videojuego **Counter-Strike: Global Offensive (CS:GO)** a partir de métricas relacionadas al rendimiento de los jugadores y la economía del equipo.

---

## 🧠 Objetivo

Predecir si un equipo ganará o perderá una ronda basándose en variables clave como:
- Equipamiento inicial
- Kills y asistencias
- Tiempo de vida
- Headshots y flanqueos

Se desarrollaron modelos de **clasificación** y **regresión**, y se seleccionaron las características más influyentes del resultado de la ronda.

---

## 🗃️ Dataset

El dataset utilizado corresponde a registros de rondas de partidas de CS:GO, con información detallada sobre el desempeño de cada equipo.

📄 Archivo: `Anexo ET_demo_round_traces_2022 (2).csv`  
🔢 Registros: ~34.000 rondas  
📌 Variables relevantes:
- `RoundWinner`: Variable objetivo (1 = gana, 0 = pierde)
- `TeamStartingEquipmentValue`
- `RoundKills`, `RoundAssists`, `RoundHeadshots`, etc.

---

## ⚙️ Estructura del Proyecto

```bash
csgo-round-prediction/
├── notebooks/
│   └── entrega3.ipynb         # Notebook principal del proyecto
├── eda/
│   ├── histogram_roundkills.png
│   ├── boxplot_equipo_vs_resultado.png
│   ├── matriz_correlacion.png
│   └── comparacion_ganadores_perdedores_CORREGIDO.png
├── api/
│   ├── main.py                # API con FastAPI para predicción interactiva
│   ├── modelo_rf.pkl          # Modelo de clasificación entrenado
│   ├── imputador.pkl          # Imputador para datos faltantes
├── data/
│   └── Anexo ET_demo_round_traces_2022 (2).csv
├── requirements.txt
└── README.md
