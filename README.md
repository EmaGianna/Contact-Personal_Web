# Emanuel Giannattasio - Portfolio

Landing page personal profesional enfocada en Data Engineering y desarrollo ETL.

## Vista previa

**URL**: https://emagianna.github.io/Contact-Personal_Web/

## Estructura del proyecto

```
/
├── index.html          # Página principal
├── css/
│   └── styles.css      # Estilos
├── js/
│   └── script.js       # JavaScript (animaciones, navegación)
├── cv/
│   └── CV_egsr.pdf     # CV descargable
└── README.md
```

## Tecnologías

- HTML5
- CSS3 (Variables, Flexbox, Grid)
- JavaScript Vanilla
- Google Fonts (Inter, JetBrains Mono)

## Desarrollo local

Abrir `index.html` en el navegador o usar un servidor local:

```bash
# Python
python -m http.server 8000

# Node.js
npx serve
```

## Flujo de trabajo (Git Flow)

El repositorio sigue la metodología **Git Flow**:

| Rama | Propósito |
|------|-----------|
| `main` | Producción. Lo que está aquí se publica en GitHub Pages. Solo recibe merges desde `release/*` o `hotfix/*`. |
| `dev` | Integración. Base para el desarrollo de nuevas funcionalidades. |
| `feature/<nombre>` | Nuevas funcionalidades o cambios. Se crean desde `dev` y se integran de vuelta en `dev`. |
| `release/<versión>` | Preparación de una versión. Se crea desde `dev` y se integra en `main` y `dev`. |
| `hotfix/<nombre>` | Correcciones urgentes en producción. Se crean desde `main` y se integran en `main` y `dev`. |

### Ejemplo: nueva funcionalidad

```bash
git checkout dev
git pull origin dev
git checkout -b feature/nueva-seccion
# ... cambios y commits ...
git push -u origin feature/nueva-seccion
# Abrir Pull Request hacia dev
```

### Ejemplo: publicar a producción

```bash
git checkout dev
git checkout -b release/1.1.0
# ... ajustes finales ...
# Pull Request de release/1.1.0 hacia main, luego merge de vuelta a dev
git tag -a v1.1.0 -m "Release 1.1.0"
```

### Convenciones

- No hacer commits directos sobre `main` ni `dev`; usar Pull Requests.
- Mensajes de commit siguiendo [Conventional Commits](https://www.conventionalcommits.org/) (`feat:`, `fix:`, `docs:`, `style:`, `refactor:`, `chore:`).
- Eliminar las ramas `feature/*`, `release/*` y `hotfix/*` una vez integradas.

## Despliegue

Configurado para GitHub Pages desde la rama `main`.
