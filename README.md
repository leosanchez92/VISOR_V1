# Visor Territorial Nueva Imperial

Conjunto de visores geográficos interactivos construidos con [Leaflet](https://leafletjs.com/) para la comuna de Nueva Imperial. Cada visor permite explorar distintas capas de información territorial sobre un mapa base, con búsqueda, leyendas y paneles de información. Se accede a las distintas categorías mediante un main site.

## Visores disponibles

| Visor | Ruta | Contenido |
|---|---|---|
| Principal | `index.html` | Localidades, sedes rurales y límite comunal. |
| Juntas de Vecinos (JJVV) | `2_JJVV/index3.html` | Organizaciones territoriales por localidad. |
| Plan Regulador Comunal (PRC) | `3_PRC/index2.html` | Zonificación e instrumentos de planificación. |
| Áreas Verdes | `4_AREAS_VERDES/index4.html` | Espacios públicos y áreas verdes. |
| Salud | `5_SALUD/index5.html` | Establecimientos y cobertura de salud. |

## Estructura del proyecto

```
├── index.html                # Visor principal
├── assets/                    # Librerías y estilos comunes (Leaflet y plugins)
├── data/                       # Datos geográficos (GeoJSON) del visor principal
├── img/                         # Imágenes, logos e íconos
├── legend/                       # Íconos de leyenda
├── 2_JJVV/                        # Visor de Juntas de Vecinos (assets/data/img propios)
├── 3_PRC/                          # Visor del Plan Regulador Comunal
├── 4_AREAS_VERDES/                  # Visor de Áreas Verdes
└── 5_SALUD/                          # Visor de Salud
```

## Uso local

Al ser un sitio estático, basta con servir la carpeta del proyecto con cualquier servidor HTTP simple, por ejemplo:

```bash
python3 -m http.server 8000
```

Luego abre `http://localhost:8000` en tu navegador para el visor principal, o navega a la ruta del visor temático que quieras revisar (por ejemplo `http://localhost:8000/2_JJVV/index3.html`).
