#  Conventional Commit

**Conventional Commit** es una **convención o estándar** para escribir mensajes de *commit* en Git de forma **consistente, legible y automatizable**.  
Se basa en una estructura simple y predecible que describe qué tipo de cambio hiciste, dónde y por qué.

---

##  Estructura básica

El formato general es:

```
<tipo>(<área opcional>): <mensaje breve>
```

**Ejemplo:**
```
feat(login): agregar autenticación con Google
fix(api): corregir error en el endpoint de usuarios
docs(readme): actualizar guía de instalación
refactor(core): optimizar cálculo de rutas
```

---

##  Tipos más comunes

| Tipo | Significado |
|------|--------------|
| **feat** | Nueva funcionalidad |
| **fix** | Corrección de un bug |
| **docs** | Cambios en documentación |
| **style** | Cambios de formato o estilo (espacios, puntos, etc.) |
| **refactor** | Reestructuración del código sin cambiar funcionalidad |
| **test** | Agregar o modificar pruebas |
| **chore** | Tareas de mantenimiento o configuraciones (build, deps, etc.) |

---

##  Por qué es importante usarlo

1. **Estandariza la comunicación:**  
   Todos los miembros del equipo entienden fácilmente qué hace cada cambio sin leer el código.

2. **Automatiza versiones y changelogs:**  
   Herramientas como **semantic-release** pueden generar automáticamente versiones (`1.0.0`, `1.1.0`, etc.) y archivos `CHANGELOG.md` según los commits.

3. **Mejora la trazabilidad:**  
   Puedes filtrar fácilmente commits por tipo (`feat`, `fix`, etc.) para revisar solo lo que te interesa.

4. **Favorece las buenas prácticas:**  
   Obliga a escribir mensajes claros, breves y con contexto, lo que mejora la calidad del historial del proyecto.

5. **Facilita CI/CD:**  
   Integraciones automáticas (por ejemplo, publicar en npm o desplegar una app) pueden basarse en los tipos de commit.

---

##  Ejemplo práctico

Si haces varios commits como:

```
feat(user): agregar registro de nuevos usuarios
fix(auth): corregir token expirado
docs: actualizar instrucciones de instalación
```

Una herramienta podría generar automáticamente un **CHANGELOG.md** así:

```markdown
###  Features
- Agregar registro de nuevos usuarios

###  Fixes
- Corregir token expirado

###  Docs
- Actualizar instrucciones de instalación
```

---

##  Beneficio general

Usar **Conventional Commits** mejora la **organización, automatización y calidad** del flujo de desarrollo, especialmente cuando trabajas en equipo o integras pipelines de CI/CD.

---
# conventionalCommit
