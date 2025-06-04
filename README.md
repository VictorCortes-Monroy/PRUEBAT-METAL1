# PRUEBAT-METAL1
# 🛰️ GPS Vehicle Monitoring App

Esta aplicación permite monitorear y analizar los movimientos de una flota de vehículos utilizando datos GPS, visualizando rutas, estadías, recorridos, vueltas y generando reportes inteligentes de forma automática.

---

## 🚀 Funcionalidades

- 📤 Carga de archivo CSV con eventos GPS
- 🕒 Filtro por rango de fechas
- 🚚 Selección de un vehículo específico o todos
- 📍 Cálculo automático de estadías por zona (geocercas)
- 🔁 Conteo de vueltas entre zonas
- 🧠 Generación de resúmenes narrativos con IA
- 🗺️ Visualización en mapa interactivo con clustering
- 🌡️ Mapa de calor de puntos GPS (opcional)
- 📥 Exportación de reportes en Excel con hojas por vehículo
- 📊 Análisis horario y de permanencia
- ✅ Compatible con múltiples vehículos simultáneos (hasta 37+)

---

## 📂 Estructura del archivo CSV esperado

| Nombre del Vehículo | Tiempo de evento     | Latitud  | Longitud  | Geocercas     |
|---------------------|----------------------|----------|-----------|---------------|
| TYZH41              | 2025-06-04 10:32:12  | -29.9043 | -71.2519  | Botadero      |

- `Tiempo de evento` debe ser un timestamp válido
- `Geocercas` puede estar vacío (se considerará "En tránsito")

---

## ⚙️ Instalación local

```bash
git clone https://github.com/tu_usuario/gps-monitor-app.git
cd gps-monitor-app
pip install -r requirements.txt
streamlit run app.py
