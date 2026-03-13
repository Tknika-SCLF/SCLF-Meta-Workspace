<div align="center">
  <img src="assets/banner.png" width="100%" alt="SCLF Platform Banner" />

  # 🌌 SCLF Meta-Workspace
  ### El Ecosistema Integral de Robótica y Procesos de AiotR
  
  [![Organization](https://img.shields.io/badge/Organization-AiotR-blue?style=for-the-badge&logo=github)](https://github.com/AiotR)
  [![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)](https://github.com/AiotR/SCLF-Meta-Workspace)
  [![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

  ---
</div>

## 🚀 Vista General

Este repositorio centraliza todos los componentes de la plataforma **SCLF** (Smart & Connected Logistics Factory). Utiliza **Git Submodules** para gestionar cada módulo de forma independiente pero manteniendo una visión global del sistema.

---

## 🛠️ Módulos del Sistema

<table width="100%">
  <tr>
    <td width="50%" valign="top">
      <h3>🤖 Robótica & Hardware</h3>
      <ul>
        <li><b><a href="sclf-gripper">🦾 SCLF Gripper</a></b><br/><i>Control de actuadores y pinzas robóticas.</i></li>
        <li><b><a href="sclf-drone">🛸 SCLF Drone</a></b><br/><i>Sistemas aéreos no tripulados.</i></li>
        <li><b><a href="sclf-quadruped-robot">🐕 SCLF Quadruped</a></b><br/><i>Plataforma robótica de cuatro patas.</i></li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>📊 Gestión & Datos</h3>
      <ul>
        <li><b><a href="sclf-bom-registry">📋 BOM Registry</a></b><br/><i>Gestión de materiales y componentes.</i></li>
        <li><b><a href="sclf-ikasmes">🏭 IkasMES</a></b><br/><i>Manufacturing Execution System.</i></li>
        <li><b><a href="sclf-manufacturing-processes">⚙️ Manufacturing</a></b><br/><i>Definición de procesos industriales.</i></li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>📚 Contenido & Educación</h3>
      <ul>
        <li><b><a href="sclf-educational-content">📖 Educational Content</a></b><br/><i>Material didáctico y tutoriales.</i></li>
        <li><b><a href="sclf-tknika-project-hub">🏠 Project Hub</a></b><br/><i>Centro de coordinación de Tknika.</i></li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>✅ Estándares & Calidad</h3>
      <ul>
        <li><b><a href="sclf-quality">🛡️ Quality</a></b><br/><i>Control de calidad y normativas.</i></li>
        <li><b><a href="sclf-templates">📄 Templates</a></b><br/><i>Plantillas de diseño y documentación.</i></li>
      </ul>
    </td>
  </tr>
</table>

---

## 📥 Configuración del Entorno

Para empezar a trabajar con todo el ecosistema, clona este repositorio utilizando el flag `--recursive`:

```powershell
git clone --recursive https://github.com/AiotR/SCLF-Meta-Workspace.git
```

### Comandos Útiles

*   **Actualizar todo:** `git submodule update --remote --merge`
*   **Añadir módulo:** `git submodule add [URL] [nombre]`

---

<div align="center">
  <sub>Desarrollado con ❤️ por <b>Antigravity AI</b> para el equipo de <b>AiotR</b></sub>
</div>
