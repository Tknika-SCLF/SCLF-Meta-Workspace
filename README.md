# 🌌 SCLF Meta-Workspace

![SCLF Platform Banner](assets/img/banner.webp)

### Tknika's Smart Collaborative Learning Factory Hub

[![Erakundea](https://img.shields.io/badge/Erakundea-Tknika--SCLF-1c1c1a?style=flat-square&logo=github)](https://github.com/Tknika-SCLF)
[![Egoera](https://img.shields.io/badge/Egoera-Aktibo-c1d10c?style=flat-square&labelColor=1c1c1a)](https://github.com/Tknika-SCLF/SCLF-Meta-Workspace)
[![Webgunea](https://img.shields.io/badge/Webgunea-Ikusi-c1d10c?style=flat-square&labelColor=1c1c1a)](https://tknika-sclf.github.io/SCLF-Meta-Workspace/)

---

## 🏗️ Filosofía de "Ecosistema Híbrido" (v2)

Este repositorio centraliza los recursos del proyecto **SCLF (Smart Collaborative Learning Factory)**. Siguiendo una estrategia híbrida para optimizar el rendimiento y la escalabilidad:

1.  **Hub de GitHub**: Mantenemos el repositorio ligero (<200MB) para alojar código, esquemas electrónicos y este portal web.
2.  **Visualización 3D**: Integración nativa con Google `<model-viewer>` para inspeccionar prototipos directamente en la web.
3.  **Almacenamiento Externo**: Los archivos pesados de ingeniería (planos STEP, modelos CAD completos, vídeos 4K) se sirven mediante enlaces a almacenamiento externo (Google Drive/Sharepoint).
4.  **Formación Centralizada**: El seguimiento académico y la certificación se realizan a través de la plataforma **Moodle** de Tknika.

---

## 🚀 Organización del Proyecto

El ecosistema se divide en cuatro áreas principales:

*   **🤖 Productos**: SCLF Gripper, Drone, Robot Cuadrúpedo.
*   **🏭 Procesos**: BOM Registry, IkasMES, Robótica Móvil, XPlanar.
*   **🎓 Formación**: Moodle, Contenido Educativo, Project Hub.
*   **📄 Documentos**: Gestión de Calidad, Plantillas de documentación.

---

## 🛠️ Estructura del Repositorio

*   `index.html`: Portal web principal de acceso público.
*   `assets/`:
    *   `img/`: Imágenes y banners optimizados.
    *   `models/`: Modelos `.glb` optimizados para visualización web.
*   `sclf-*`: Submódulos Git que apuntan a los repositorios de código de cada componente.

---

## 📥 Clonación del Entorno

Para obtener el espacio de trabajo meta con todos sus módulos vinculados:

```powershell
git clone --recursive https://github.com/Tknika-SCLF/SCLF-Meta-Workspace.git
```

---

<div align="center">
  <sub>Desarrollado por el equipo <b>AiotR</b> de Tknika para el ecosistema <b>SCLF</b></sub>
</div>
