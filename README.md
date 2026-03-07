# 🤖 IngDash: Collaborative Dashboard

Bienvenido al taller de **Git & GitHub** febrero 2026. El objetivo de este proyecto es construir un panel de control colaborativo donde cada integrante registre su propio "módulo" de trabajo.

## Requisitos

- Tener instalado [Git](https://git-scm.com/).
- Una cuenta activa en [GitHub](https://github.com/).
- VS Code (recomendado).

## Instrucciones de la Práctica

### 1. Clonar el repositorio

Primero, obtén la base del proyecto y desconéctala de mi repositorio. Abre tu terminal y ejecuta:

```bash
git clone https://github.com/JosephAntonyDev/collab-dashboard-course.git
cd collab-dashboard-course
git remote remove origin
```

### 2. Crear tu propio repositorio en GitHub

- Ve a GitHub y crea un nuevo repositorio llamado `my-first-dashboard`.
- Vincula tu carpeta local con tu nuevo repo:

```bash
git remote add origin https://github.com/TU_USUARIO/my-first-dashboard.git
git branch -M main
git push -u origin main
```

### 3. Crear una rama (Feature Branch)

No trabajes en `main`. Crea una rama con tu nombre:

```bash
git checkout -b feature/nombre-apellido
```

### 4. Editar el código

- Abre `index.html`.
- Busca la sección `<main class="dashboard-container">`.
- Copia el bloque de la card de ejemplo y pega el tuyo debajo.
- Cambia el emoji, tu nombre y el porcentaje de la barra de progreso.

Ejemplo:

```html
<div class="card">
    <div class="icon">🚀</div>
    <h3>Diseño</h3>
    <p><strong>Responsable:</strong> Alejandro Ismael</p>
    <p><strong>Estatus:</strong> Durmiendo</p>
    <div class="bar">
        <div class="progress" style="width: 95%;"></div>
    </div>
</div>
```

### 5. Guardar y subir los cambios

```bash
git add .
git commit -m "feat: add my dashboard card"
git push origin feature/nombre-apellido
```
