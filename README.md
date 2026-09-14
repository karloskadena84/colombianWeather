# Colombian Weather

Dashboard de clima para ciudades de Colombia — UI liquid-glass, datos en tiempo real y calidad del aire.

**Autor:** Carlos Cadena

## Estado del repo

El dashboard completo está en tu PC (carpeta `weather-dashboard-colombia` / el ZIP).  
Sube el `index.html` bueno con los pasos de abajo para dejar la app publicada aquí.

## Cómo subir el dashboard completo (Windows)

1. Abre **CMD** o **PowerShell** en la carpeta del proyecto (donde está el `index.html` que funciona):

```bat
cd %USERPROFILE%\Documents\weather-dashboard-colombia
```

2. Conecta con GitHub:

```bat
git init
git remote remove origin
git remote add origin https://github.com/karloskadena84/colombianWeather.git
```

3. Sube los archivos:

```bat
git add index.html README.md
git add assets 2>nul
git commit -m "Dashboard Colombian Weather completo"
git branch -M main
git pull origin main --allow-unrelated-histories --no-edit
git push -u origin main
```

GitHub te pedirá iniciar sesión (navegador o token personal).

### Alternativa sin git (web)

1. Entra a https://github.com/karloskadena84/colombianWeather
2. **Add file → Upload files**
3. Arrastra tu `index.html` (el del ZIP que funciona en local)
4. Commit en la rama `main`

## Cómo verlo en local

```bat
py -m http.server 8080
```

Abre: http://localhost:8080

## Características

- Open-Meteo (clima + calidad del aire), sin API key
- Medellín por defecto; agregar / quitar ciudades (mínimo 1)
- Video de fondo según clima, modo oscuro, glass UI

## APIs

| Servicio | Uso |
|----------|-----|
| `api.open-meteo.com` | Clima |
| `air-quality-api.open-meteo.com` | AQI |
| Mixkit CDN | Videos de fondo |

## Licencia

Uso del autor del repositorio. Datos © Open-Meteo.
