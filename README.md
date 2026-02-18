# FuegoLab: Motor de Inteligencia Satelital de Incendios Forestales (México 2022-2024)

### 🛰️ Automatización de Búsqueda Espectral en Copernicus & Sentinel-2

**Arquitecto:** Eduardo Lemus Mendoza
**Cobertura:** +20,000 Eventos de Fuego
**Stack:** Leaflet JS, Copernicus Browser API Linkage, CONAFOR Data

## 📋 Resumen Ejecutivo
La investigación de incendios forestales requiere validar "lo que se reporta" contra "lo que se ve". **FuegoLab** es un sistema de inteligencia geoespacial que indexa más de **20,000 reportes de incendios** (Datos CONAFOR) y genera automáticamente enlaces profundos (Deep Links) a la plataforma **Copernicus Browser**.

El sistema elimina la fricción de buscar manualmente coordenadas y fechas. Al hacer clic en un evento, el sistema inyecta la ubicación y la ventana temporal precisa en el servicio de la Agencia Espacial Europea (ESA), permitiendo visualizar imágenes **Sentinel-2** inmediatas para análisis de severidad (NBR), cicatrices de quema y emisiones.

## 🛠️ Arquitectura de la Solución
El valor técnico reside en la **Integración de Servicios** y la experiencia de usuario (UX) para analistas:

1.  **Ingesta de Datos:** Base de datos vectorizada de incidencias 2022-2024.
2.  **Motor de Enlace Dinámico:** Algoritmo que toma las coordenadas $(x, y)$ y la fecha $(t)$ del incendio, y construye una URL parametrizada para Copernicus Browser.
3.  **Visualización Interactiva:** Mapa web ligero basado en Leaflet con filtrado por superficie afectada (Hectáreas).

## 💡 Casos de Uso
* **Validación de Daños:** Auditoría visual de reportes oficiales vs. realidad satelital.
* **Entrenamiento de IA:** Generación rápida de datasets de imágenes para entrenar modelos de detección de fuego (Computer Vision).
* **Periodismo de Datos:** Verificación de incendios masivos y su impacto ambiental real.

## 🚀 Guía Rápida
1.  **Filtra:** Selecciona el año y la superficie mínima (ej. > 500 hectáreas).
2.  **Selecciona:** Haz clic en el marcador del incendio.
3.  **Audita:** Presiona *"Ver en Satélite"*. FuegoLab te llevará a la imagen exacta del día del evento en Sentinel-2.

## 🔗 Contacto y Desarrollo
Este proyecto demuestra cómo la web geoespacial ligera puede acelerar flujos de trabajo de teledetección complejos.

* **Perfil Profesional:** [Eduardo Lemus Mendoza en LinkedIn](https://www.linkedin.com/in/eduardo-lemus-mendoza/)
* **Portafolio Académico:** [Instructor en Udemy](https://www.udemy.com/user/eduardo-lemus-mendoza/)
