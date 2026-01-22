# ⚡ Guía Rápida - Sprint Planning en 5 Minutos

> Instrucciones paso a paso para configurar tu Sprint Planning automáticamente

---

## 🚀 Configuración Rápida

### **Opción 1: Automática con Script (Recomendada)**

```bash
# 1. Clonar el repositorio
git clone https://github.com/SistemasTecTlaxiaco/desarrollo-aplicaciones-descentralizadas.git
cd desarrollo-aplicaciones-descentralizadas

# 2. Autenticarse (solo primera vez)
gh auth login

# 3. Ejecutar script
chmod +x setup-sprint.sh
./setup-sprint.sh
```

**✅ ¡Listo!** En menos de 1 minuto tendrás 11 issues creados.

---

### **Opción 2: Manual (Si no tienes GitHub CLI)**

#### **Paso 1: Crear Labels**
Ve a: `https://github.com/SistemasTecTlaxiaco/desarrollo-aplicaciones-descentralizadas/labels`

Crea estos labels:
- `Sprint-1` (verde)
- `Inicio` (azul)
- `Desarrollo` (amarillo)
- `Cierre` (rojo)
- `Evaluación` (celeste)
- `Práctica` (morado)
- `Investigación` (turquesa)
- `Ceremonia-Scrum` (rosa)

#### **Paso 2: Crear Issues Manualmente**
Ve a: `Issues → New Issue`

Copia las descripciones del archivo `setup-sprint.sh` para cada issue.

---

## 📋 Crear GitHub Project

### **Método Rápido:**

1. Ve a: https://github.com/users/josealfredo79/projects
2. Clic en **"New project"**
3. Selecciona: **"Team backlog"** template
4. Nombre: `Desarrollo Aplicaciones Descentralizadas`
5. Clic en **"Create project"**

### **Configurar Columnas:**

```
📝 Backlog → 🔄 Sprint Backlog → 👷 In Progress → 👀 Review → ✅ Done
```

### **Agregar Issues:**

1. En el proyecto, clic en **"Add items"**
2. Busca tu repositorio
3. Selecciona todos los issues (Ctrl+A / Cmd+A)
4. Clic en **"Add selected items"**

---

## 👥 Conformar Equipos

### **Template de Equipo:**

```markdown
## 📌 Equipo [Número]

**Nombre del Equipo:** _________________

### Integrantes:
1. **Product Owner:** _________________
2. **Scrum Master:** _________________
3. **Developer:** _________________
4. **Developer:** _________________
5. **Developer:** _________________

### Normas del Equipo:
- [ ] Reuniones diarias: __________ (hora)
- [ ] Canal de comunicación: __________
- [ ] Repositorio del equipo: __________
- [ ] Definition of Done acordada

### Sprint Goal:
_________________________________________________
```

Copia esto en un nuevo issue o documento compartido.

---

## 📊 Estimar Story Points

### **Guía de Estimación:**

| Story Points | Esfuerzo | Tiempo Estimado |
|--------------|----------|-----------------|
| 1 SP | Muy Bajo | 1-2 horas |
| 2 SP | Bajo | 2-4 horas |
| 3 SP | Medio | 4-6 horas |
| 5 SP | Alto | 1-2 días |
| 8 SP | Muy Alto | 2-3 días |

### **Técnica Planning Poker:**

1. Cada miembro estima individualmente
2. Revelan estimaciones simultáneamente
3. Discuten diferencias grandes
4. Re-estiman hasta consenso

---

## 🎯 Priorizar Backlog

### **Método MoSCoW:**

- **M**ust have (Debe tener) → Alta prioridad
- **S**hould have (Debería tener) → Media prioridad
- **C**ould have (Podría tener) → Baja prioridad
- **W**on't have (No tendrá) → Fuera del sprint

### **En GitHub:**

1. Edita cada issue
2. Agrega label de prioridad:
   - 🔴 `priority: high`
   - 🟡 `priority: medium`
   - 🟢 `priority: low`

---

## 🔄 Ceremonias Scrum

### **1️⃣ Sprint Planning (Día 1)**
- ⏱️ **Duración:** 2 horas
- 🎯 **Objetivo:** Planificar el sprint
- 📝 **Entregable:** Sprint Backlog completo

### **2️⃣ Daily Standup (Diario)**
- ⏱️ **Duración:** 15 minutos
- 🎯 **3 Preguntas:**
  - ¿Qué hice ayer?
  - ¿Qué haré hoy?
  - ¿Qué impedimentos tengo?

### **3️⃣ Sprint Review (Último día)**
- ⏱️ **Duración:** 1 hora
- 🎯 **Objetivo:** Presentar entregables
- 📝 **Entregable:** Demo + Presentación

### **4️⃣ Sprint Retrospective (Último día)**
- ⏱️ **Duración:** 45 minutos
- 🎯 **Objetivo:** Mejorar proceso
- 📝 **Formato:**
  - ✅ ¿Qué salió bien?
  - ❌ ¿Qué salió mal?
  - 💡 ¿Qué podemos mejorar?

---

## 📝 Trabajar en Issues

### **Flujo de Trabajo:**

```bash
# 1. Asignar issue a ti mismo
gh issue edit [NÚMERO] --add-assignee @me

# 2. Mover a "In Progress" en el Project

# 3. Crear branch para la tarea
git checkout -b issue-[NÚMERO]-descripcion

# 4. Trabajar en la tarea

# 5. Commit con referencia al issue
git commit -m "Add: mapa mental Web 3.0 #5"

# 6. Push
git push origin issue-[NÚMERO]-descripcion

# 7. Mover a "Review" en el Project

# 8. Cerrar issue cuando se complete
gh issue close [NÚMERO]
```

---

## 🎨 Plantillas Útiles

### **Plantilla de Retrospectiva:**

```markdown
## 🔄 Sprint Retrospective

**Fecha:** __________
**Equipo:** __________

### ✅ ¿Qué salió bien?
1. _________________________
2. _________________________
3. _________________________

### ❌ ¿Qué salió mal?
1. _________________________
2. _________________________
3. _________________________

### 💡 ¿Qué mejoraremos?
1. _________________________
2. _________________________
3. _________________________

### 🎯 Action Items:
- [ ] Acción 1 - Responsable: _____
- [ ] Acción 2 - Responsable: _____
```

### **Plantilla de Sprint Review:**

```markdown
## 📊 Sprint Review

**Sprint:** Sprint 1
**Fecha:** __________
**Equipo:** __________

### 🎯 Sprint Goal
_____________________________________

### 📈 Métricas
- **Story Points planificados:** 34 SP
- **Story Points completados:** ___ SP
- **Velocity:** ___ SP
- **Tasa de completitud:** ____%

### ✅ Issues Completados
- [ ] #1 - Sprint Planning
- [ ] #2 - Backlog
- [ ] ...

### 🚧 Issues No Completados
- [ ] #X - Razón: ____________

### 🎓 Lecciones Aprendidas
1. _________________________
2. _________________________

### 📸 Capturas de Demos
(Incluir imágenes de prácticas)
```

---

## 🔧 Comandos GitHub CLI Útiles

```bash
# Ver issues del sprint
gh issue list --label "Sprint-1"

# Ver solo issues abiertos
gh issue list --state open

# Ver issues asignados a ti
gh issue list --assignee @me

# Crear nuevo issue
gh issue create --title "Título" --body "Descripción"

# Comentar en un issue
gh issue comment [NÚMERO] --body "Mi comentario"

# Ver detalles de un issue
gh issue view [NÚMERO]

# Listar labels
gh label list

# Ver PRs abiertos
gh pr list
```

---

## 🚨 Solución de Problemas

### **Error: "gh: command not found"**
**Solución:** Instala GitHub CLI
```bash
# Windows
winget install --id GitHub.cli

# macOS
brew install gh

# Linux
sudo apt install gh
```

### **Error: "Not authenticated"**
**Solución:** Autentícate
```bash
gh auth login
```

### **Error: "Permission denied"**
**Solución:** Verifica que tienes acceso al repositorio
```bash
gh repo view SistemasTecTlaxiaco/desarrollo-aplicaciones-descentralizadas
```

### **Script no ejecuta en Windows**
**Solución:** Usa Git Bash o WSL
```bash
# Git Bash
bash setup-sprint.sh

# O instala WSL
wsl --install
```

---

## 📱 Apps Recomendadas

### **Para Estudiantes:**
- **GitHub Mobile** - Gestionar issues desde el móvil
- **Discord/Slack** - Comunicación del equipo
- **Trello/Notion** - Notas y documentación
- **Miro** - Mapas mentales colaborativos

### **Para Docente:**
- **GitHub Classroom** - Gestionar asignaciones
- **ZenHub** - Analíticas avanzadas de proyectos
- **Kahoot** - Quiz interactivos

---

## 🎯 Checklist de Inicio

```markdown
### Para el Estudiante:
- [ ] Cuenta de GitHub creada
- [ ] Agregado al repositorio
- [ ] GitHub CLI instalado
- [ ] Equipo conformado
- [ ] Rol Scrum asignado
- [ ] Acceso al GitHub Project
- [ ] Normas del equipo acordadas

### Para el Docente:
- [ ] Repositorio creado
- [ ] Issues generados
- [ ] GitHub Project configurado
- [ ] Estudiantes agregados como colaboradores
- [ ] Criterios de evaluación comunicados
- [ ] Fechas de entrega establecidas
```

---

## 📞 Ayuda Adicional

**Documentación completa:** [README.md](./README.md)

**Recursos:**
- [GitHub Docs](https://docs.github.com/)
- [GitHub CLI Manual](https://cli.github.com/manual/)
- [EduScrum Guide](https://www.eduscrum.nl/en/)

**Contacto:**
- Docente: @josealfredo79
- Issues del proyecto: https://github.com/SistemasTecTlaxiaco/desarrollo-aplicaciones-descentralizadas/issues

---

**🎉 ¡Ahora estás listo para comenzar tu Sprint!**
