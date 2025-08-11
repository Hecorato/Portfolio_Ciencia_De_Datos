# Agrupación de Coordenadas y Detección de Grupos Repetidos

Este proyecto procesa un conjunto de coordenadas geográficas (latitud/longitud) para:
1. **Agrupar puntos cercanos** en un radio de 4 metros usando `BallTree` con métrica *Haversine*.
2. **Detectar grupos repetidos** que aparecen en **más de un mes distinto**.
3. **Exportar un archivo Excel** (`resultado.xlsx`) con el detalle de esos grupos repetidos.

---

## 📂 Archivo generado
- **`resultado.xlsx`** → Contiene únicamente las filas que pertenecen a grupos detectados como repetidos (más de un mes).

---

## 🛠 Requisitos
Instala las librerías necesarias:
```bash
pip install pandas numpy scikit-learn openpyxl
