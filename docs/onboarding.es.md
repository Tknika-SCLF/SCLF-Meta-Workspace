# 🚀 SCLF Onboarding Guide

Tknika — Smart Collaborative Learning Factory

---

## 🌍 Selecciona idioma / Select language / Hautatu hizkuntza

- 🇪🇸 [Español](onboarding.es.md)  
- 🇪🇺 [Euskara](onboarding.eu.md)  
- 🇬🇧 [English](onboarding.en.md)  

---

## 🎯 Objetivo

Este documento explica cómo empezar a trabajar en el ecosistema SCLF. La arquitectura se basa en tres principios fundamentales:

- 👉 No hay monorepo
- 👉 No hay submódulos
- 👉 Todo es modular

## 🧩 Estructura del sistema

SCLF está compuesto por múltiples repositorios independientes. Cada uno funciona como un proyecto autónomo:

- `sclf-drone`
- `sclf-gripper`
- `sclf-computer-vision`
- `sclf-ikasmes`
- `sclf-xplanar`
- etc.

**Nota:** Solo clona los módulos que vayas a utilizar para mantener tu entorno ligero.

## 🖥️ Setup inicial

### 1. Crear carpeta de trabajo

```bash
mkdir SCLF
cd SCLF
```

### 2. Clonar repositorios necesarios

```bash
git clone git@github.com:Tknika-SCLF/sclf-drone.git
git clone git@github.com:Tknika-SCLF/sclf-gripper.git
git clone git@github.com:Tknika-SCLF/sclf-computer-vision.git
```

## 🔐 Autenticación (recomendado)

Para evitar pedir credenciales constantemente, se recomienda usar SSH.

Generar clave:

```bash
ssh-keygen -t ed25519 -C "tu_email"
```

Después, añade la clave pública a tu configuración de GitHub.

## 🧠 Metodología de trabajo

### Flujo estándar de Git

Para cualquier contribución, sigue estos pasos dentro del repositorio correspondiente:

1. **Entrar en el repo**
   ```bash
   cd sclf-drone
   ```
2. **Actualizar la rama principal y crear una rama nueva**
   ```bash
   git checkout main
   git pull
   git checkout -b feature/nombre-de-la-mejora
   ```
3. **Trabajar y commitear**
   ```bash
   git add .
   git commit -m "feat: descripción clara de los cambios"
   ```
4. **Subir cambios**
   ```bash
   git push origin feature/nombre-de-la-mejora
   ```
5. **Pull Request**
   Crear la PR directamente en la interfaz de GitHub.

## ⚠️ Reglas importantes

### ✅ Do's
- Usar ramas para cada cambio
- Revisar cambios antes de ejecutar scripts
- Mantener repositorios pequeños y claros

### ❌ Don'ts
- No trabajar en `main` directamente
- No usar submódulos
- No ejecutar código sin entenderlo

## 🧪 Seguridad (muy importante)

Si trabajas con asistencia de IA:

👉 **Nunca ejecutes scripts generados automáticamente sin supervisión.**

**Siempre:**
- Leer el código
- Entender su lógica
- Ejecutarlo manualmente

## 🧰 Entorno recomendado

- **WSL:** Linux dentro de Windows para mejor compatibilidad
- **VSCode / Antigravity:** como entorno principal de trabajo
- **Docker:** opcional, pero recomendado para aislamiento de procesos

## 📂 Meta-Workspace

Sobre este repositorio principal:

- ❌ No es un entorno de desarrollo
- ✅ Es un índice y punto de entrada al ecosistema

## 🧭 Resumen

- Clona solo lo necesario
- Trabaja de forma modular por repositorios
- Usa ramas siempre
- Revisa minuciosamente antes de ejecutar
