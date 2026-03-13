# SCLF Meta-Workspace

Este repositorio agrupa todos los componentes del ecosistema SCLF de AiotR en un único lugar utilizando **Git Submodules**.

## Componentes incluidos:

- [0. Project Hub](sclf-tknika-project-hub)
- [1. Gripper](sclf-gripper)
- [1. Drone](sclf-drone)
- [1. Quadruped](sclf-quadruped-robot)
- [2. Processes](sclf-manufacturing-processes)
- [2. BOM Registry](sclf-bom-registry)
- [3. Ikasmes](sclf-ikasmes)
- [4. Educational](sclf-educational-content)
- [5. Templates](sclf-templates)
- [6. Quality](sclf-quality)

## Cómo usar este Workspace

### Para clonar todo el entorno de una vez:
```bash
git clone --recursive [URL_DE_ESTE_REPO]
```

### Para actualizar todos los subrepositorios:
```bash
git submodule update --remote --merge
```

### Estructura
Este repositorio funciona como un contenedor. En GitHub, verás cada carpeta con un icono de enlace que lleva directamente al repositorio correspondiente.
