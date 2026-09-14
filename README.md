# Colombian Weather

Dashboard de clima para ciudades de Colombia — UI liquid-glass, datos en tiempo real y calidad del aire.

**Autor:** Carlos Cadena

## Características

- Pronóstico en vivo con [Open-Meteo](https://open-meteo.com/) (sin API key)
- Calidad del aire (AQI europeo + PM2.5)
- Ciudades principales: Medellín, Bogotá, Cali, Barranquilla (+ búsqueda y lista personalizable)
- Fondo de video según el clima
- Interfaz en español, glassmorphism, modo oscuro
- Agregar / quitar ciudades (mínimo 1)

## Cómo verlo

### Opción A — GitHub Pages
Si activas Pages en este repo (Settings → Pages → Deploy from branch `main`), abre la URL pública del sitio.

### Opción B — Local

```bash
# Clonar
git clone https://github.com/karloskadena84/colombianWeather.git
cd colombianWeather

# Servidor local (necesario para la API; no abras solo el file://)
python -m http.server 8080
# o: py -m http.server 8080
```

Luego abre: http://localhost:8080

## Estructura

```
index.html          # App completa (HTML + CSS + JS)
assets/             # Video/poster de respaldo (opcional)
README.md
```

## APIs

| Servicio | Uso |
|----------|-----|
| `api.open-meteo.com` | Clima actual, por horas y diario |
| `air-quality-api.open-meteo.com` | Calidad del aire |
| Mixkit (CDN) | Videos de fondo por condición |

## Licencia

Uso libre para el autor del repositorio. Datos © Open-Meteo. Videos de fondo según licencia Mixkit.
