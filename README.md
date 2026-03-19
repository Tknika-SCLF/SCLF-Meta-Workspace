# 🌌 SCLF Meta-Workspace

![SCLF Platform Banner](assets/banner.webp)

### Tknika's Smart Collaborative Learning Factory Hub

[![Erakundea](https://img.shields.io/badge/Erakundea-Tknika--SCLF-1c1c1a?style=flat-square&logo=github)](https://github.com/Tknika-SCLF)
[![Egoera](https://img.shields.io/badge/Egoera-Aktibo-c1d10c?style=flat-square&labelColor=1c1c1a)](https://github.com/Tknika-SCLF/SCLF-Meta-Workspace)
[![Webgunea](https://img.shields.io/badge/Webgunea-Ikusi-c1d10c?style=flat-square&labelColor=1c1c1a)](https://tknika-sclf.github.io/SCLF-Meta-Workspace/)

---

## 🏗️ Filosofía de "Ecosistema Híbrido" (V2)

Este repositorio ha sido reestructurado para funcionar como un **Hub centralizado** de ingeniería. Siguiendo la estrategia de alto rendimiento para proyectos multidisciplinares:

1.  **GitHub (El Cerebro)**: Aloja el código fuente, esquemas ligeros, documentación en Markdown y este portal web (GitHub Pages). Se mantiene por debajo de **200MB**.
2.  **Visores Nativos**: Los modelos 3D se visualizan directamente en el navegador usando `.glb` optimizados y Google `<model-viewer>`.
3.  **Almacenamiento Externo (El Músculo)**: Los archivos pesados de ingeniería (planos STEP, modelos CAD completos, vídeos 4K, firmwares binarios) se gestionan mediante enlaces externos a **Google Drive / Sharepoint**.
4.  **Formación**: Toda la certificación y el seguimiento pedagógico se centraliza en la plataforma **Moodle** de Tknika.

---

## 🚀 Estructura del Repositorio

- `index.html`: Portal web principal (Landing Page).
- `assets/`:
  - `img/`: Imágenes optimizadas.
  - `models/`: Modelos 3D en formato `.glb` (optimización Draco recomendada).
- `sclf-*`: Submódulos Git con el código fuente de cada componente.

---

## 🛠️ Sistemaren Moduluak

### 🤖 Produktuak
*   **[🦾 SCLF Gripper](https://github.com/Tknika-SCLF/SCLF_Gripper_v1.0)**: Aktuatzaileen eta matxarda robotikoen kontrola.
*   **[🛸 SCLF Drone](https://github.com/Tknika-SCLF/sclf-drone)**: Tripulatu gabeko aire-sistemak.
*   **[🐕 SCLF Quadruped](https://github.com/Tknika-SCLF/sclf-quadruped-robot)**: Lau hanka dituen plataforma robotikoa.
*   **[📐 Diseinu Mekanikoa](https://github.com/Tknika-SCLF/sclf-mechanical-design)**: 3D ereduak eta planoen dokumentazioa.

... *(Ver más en la web)*

---

## 📥 Clonación del Entorno

Para trabajar con todo el ecosistema localmente:

```powershell
git clone --recursive https://github.com/Tknika-SCLF/SCLF-Meta-Workspace.git
```

---

<div align="center">
  <sub>Desarrollado por <b>Antigravity AI</b> para el equipo <b>AiotR</b> de Tknika</sub>
</div>
