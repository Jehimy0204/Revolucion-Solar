# Git Workflow – Revolución Solar

---

## 📌 Enlace al repositorio

https://github.com/Jehimy0204/Revolucion-Solar

---

## 1. Flujo de trabajo con ramas

Este proyecto utiliza una estrategia basada en Git Flow simplificado, con las siguientes ramas principales:

- `main`: rama estable, lista para producción.
- `develop`: rama de desarrollo donde se integran nuevas funcionalidades.
- `feature/*`: ramas temporales para el desarrollo de funcionalidades específicas. Se crean desde `develop` y al finalizar se integran nuevamente allí.

Ejemplo del flujo de ramas:

main  
├── develop  
│   ├── feature/login-system  
│   ├── feature/form-contact  
│   └── feature/dashboard-ui  

---

## 2. Ramas de funcionalidad creadas

Desde la rama `develop` se crearon las siguientes ramas de funcionalidad:

- `feature/login-system`: desarrollo del sistema de autenticación.
- `feature/form-contact`: desarrollo del formulario de contacto.
- `feature/dashboard-ui`: implementación del panel de administración.

Estas ramas están disponibles en el repositorio GitHub.

---

## 3. Convención de commits

Para mantener un historial de cambios claro, los commits deben seguir esta estructura:

Ejemplos:  
- feat: agregar formulario de contacto  
- fix: corregir error en validación  
- refactor: mejorar estructura del código  

Tipos recomendados:  
- `feat`: nueva funcionalidad  
- `fix`: corrección de errores  
- `docs`: cambios en documentación  
- `style`: cambios de formato (espaciado, identación, etc.)  
- `refactor`: reestructuración del código sin cambiar su funcionalidad  
- `test`: pruebas  
- `chore`: tareas menores de mantenimiento  

---

## 4. Frecuencia recomendada de push/pull

- **Push**: al completar una funcionalidad o sección estable.
- **Pull**: antes de comenzar a trabajar y justo antes de hacer push para evitar conflictos.

Ejemplo:
```bash
git pull origin develop
git add .
git commit -m "feat: agregar login"
git push origin feature/login-system
```

---

## 5. Política de Pull Requests (PR)

- Las ramas `feature/*` deben integrarse a través de PR hacia `develop`.
- No se permite merge directo a `main`.
- Cada PR debe incluir:
  - Una descripción clara de los cambios realizados.
  - Revisión de al menos un integrante antes del merge.

---

## 6. Plantilla para Pull Requests (opcional)

```md
### 📋 Descripción
Explica brevemente qué funcionalidad o corrección se está integrando en esta solicitud de cambio.

### ✅ Cambios realizados
- [ ] Se agregó ...
- [ ] Se modificó ...
- [ ] Se eliminó ...
- [ ] Se corrigió ...

### 🔍 ¿Cómo probarlo?
Instrucciones claras para probar los cambios realizados, preferiblemente paso a paso.

### 📝 Notas adicionales
Anota cualquier decisión técnica, dudas, dependencias o aspectos relevantes para la revisión.
```

---

**Este documento forma parte del entregable del informe de análisis, diseño y alistamiento.**
