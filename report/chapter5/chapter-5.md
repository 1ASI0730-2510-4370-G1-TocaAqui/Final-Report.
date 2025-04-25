# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration

#### Requirements Management

**Jira**: Herramienta de gestión ágil utilizada para organizar y monitorear las tareas del proyecto. Cada actividad fue registrada con una clave única y se asignó a miembros responsables, permitiendo controlar el avance por capítulo.  
Ruta de referencia: [https://www.atlassian.com/software/jira](https://www.atlassian.com/software/jira)

#### Product UX/UI Design

**Figma**: Plataforma online empleada para crear diseños visuales y prototipos navegables tanto para escritorio como dispositivos móvilxes. Fue esencial en la definición de la experiencia de usuario del landing.  
Ruta de referencia: [https://www.figma.com](https://www.figma.com)

#### Software Development

**Visual Studio Code**: Editor de texto utilizado por todos los miembros del equipo, elegido por su ligereza, compatibilidad con múltiples lenguajes y sus extensiones útiles para desarrollo web y control de versiones.  
Ruta de referencia: [https://code.visualstudio.com](https://code.visualstudio.com)

**HTML5 / CSS3 / JavaScript**: Tecnologías base para el desarrollo del sitio web estático. HTML estructura el contenido, CSS define el estilo visual y JavaScript brinda interactividad.

Referencias:
- HTML5: [https://www.w3schools.com/html/html5_syntax.asp](https://www.w3schools.com/html/html5_syntax.asp)
- CSS3: [https://google.github.io/styleguide/htmlcssguide.html](https://google.github.io/styleguide/htmlcssguide.html)
- JavaScript: [https://developer.mozilla.org/es/docs/Web/JavaScript](https://developer.mozilla.org/es/docs/Web/JavaScript)

**Git**: Sistema de control de versiones distribuido usado localmente para manejar el historial de cambios del proyecto.  
Ruta de referencia: [https://git-scm.com](https://git-scm.com)

#### Documentation & Project Hosting

**GitHub**: Plataforma en la nube donde se alojan los repositorios del equipo. Se utilizó para controlar versiones, gestionar ramas con GitFlow y mantener sincronizado el avance entre todos los integrantes.  
Repositorio de la Landing Page:  
[https://github.com/1ASI0730-2510-4370-G1-TocaAqui/Landing-Page](https://github.com/1ASI0730-2510-4370-G1-TocaAqui/Landing-Page)

#### Software Deployment

**GitHub Pages**: Servicio empleado para desplegar el sitio estático del proyecto directamente desde la rama `main`.  
Enlace en producción:  
[https://1asi0730-2510-4370-g1-tocaaqui.github.io/Landing-Page/](https://1asi0730-2510-4370-g1-tocaaqui.github.io/Landing-Page/)

**Vercel (previsto)**: Plataforma que será usada en los próximos sprints para desplegar la aplicación frontend en Vue.js, permitiendo despliegues automáticos desde GitHub.  
Ruta de referencia: [https://vercel.com](https://vercel.com)


### 5.1.2. Source Code Management

El equipo aplica la estrategia GitFlow, que organiza el desarrollo con ramas específicas para cada tipo de contribución. Las ramas implementadas en este Sprint fueron:

- `main`: contiene la versión estable desplegada
- `develop`: utilizada como base para integrar avances
- `feature/*`: se creó una rama por cada funcionalidad nueva del landing page

Durante este primer Sprint, se realizó trabajo activo en ramas `feature/*`, que luego fueron integradas mediante `merge` hacia la rama `main` para el despliegue en GitHub Pages. La estructura de ramas puede verse directamente en el historial del repositorio.

   ![Gitflow](/assets/gitflow.png)


Repositorio principal:  
[https://github.com/1ASI0730-2510-4370-G1-TocaAqui/Landing-Page](https://github.com/1ASI0730-2510-4370-G1-TocaAqui/Landing-Page)

**Commits estructurados (Conventional Commits)**  
Se siguió el estándar [Conventional Commits](https://www.conventionalcommits.org) para mantener claridad y coherencia en el historial del proyecto. Ejemplos reales incluidos:

- `feat(html): added material design`
- `style(icons): replace RemixIcon with Material Design Icons library`
- `feat(a11y): add ARIA attributes to main navigation and header sections`
- `docs(readme): update documentation for UPC university project`



### 5.1.3. Source Code Style Guide & Conventions

#### HTML

- Todas las etiquetas deben cerrarse correctamente
- Comentarios cortos en línea
- Uso obligatorio de atributos `alt`, `width`, `height` en imágenes
- Nombres de clases en inglés, en lower-case con guiones

Referencia: [https://www.w3schools.com/html/html5_syntax.asp](https://www.w3schools.com/html/html5_syntax.asp)

#### CSS

- Indentación de 2 espacios
- Código en minúscula y limpio
- Comentarios explicativos por bloque
- Nombres de clase descriptivos y semánticos

Referencia: [https://google.github.io/styleguide/htmlcssguide.html](https://google.github.io/styleguide/htmlcssguide.html)

#### JavaScript

- Variables con nombres representativos
- Uso coherente de comillas (simples o dobles)
- Funciones modulares y reutilizables
- Comentarios en secciones complejas
- Evitar variables globales

Referencia: [https://developer.mozilla.org/es/docs/Web/JavaScript](https://developer.mozilla.org/es/docs/Web/JavaScript)

#### Vue.js (para sprints futuros)

- Carpetas organizadas por módulos: `components/`, `views/`, `store/`
- Reutilización de componentes
- Separación clara entre lógica y vista
- Documentación interna con props, eventos y métodos

Referencia: [https://vuejs.org/guide/introduction](https://vuejs.org/guide/introduction)


### 5.1.4. Software Deployment Configuration

Para desplegar la **Landing Page** del proyecto **TocaAquí** usando **GitHub Pages**, se siguieron los siguientes pasos:

1. **Ubicar el repositorio del proyecto**  
   Se accede al repositorio público alojado en GitHub que contiene el código fuente del sitio:  
   ![Paso 1](../../assets/Deploy-first.png)

2. **Ir a la sección de configuración (Settings)**  
   En la barra superior del repositorio, se hace clic en la pestaña **Settings**.

   ![Paso 2](../../assets/Deploy-two.png)

3. **Configurar GitHub Pages desde una rama**  
   En la sección **Pages**, dentro de **Build and deployment**, se selecciona `Deploy from a branch`.  
   Luego, se elige la rama `main` y la carpeta raíz `/ (root)` como origen del contenido.

   ![Paso 3](../../assets/Deploy-three.png)

Una vez configurado, GitHub genera automáticamente la URL pública del sitio, que queda disponible para validación, pruebas o entrevistas con usuarios.

**URL:** [`https://1asi0730-2510-4370-g1-tocaaqui.github.io/Landing-Page/index.html`](https://1asi0730-2510-4370-g1-tocaaqui.github.io/Landing-Page/index.html)

## 5.2. Landing Page, Services & Applications Implementation
### 5.2.X. Sprint n
#### 5.2.X.1. Sprint Planning n
#### 5.2.X.2. Aspect Leaders and Collaborators
#### 5.2.X.3. Sprint Backlog n
#### 5.2.X.4. Development Evidence for Sprint Review
#### 5.2.X.5. Execution Evidence for Sprint Review
#### 5.2.X.6. Services Documentation Evidence for Sprint Review
#### 5.2.X.7. Software Deployment Evidence for Sprint Review
#### 5.2.X.8. Team Collaboration Insights during Sprint

## 5.3. Validation Interviews
### 5.3.1. Diseño de Entrevistas
### 5.3.2. Registro de Entrevistas
### 5.3.3. Evaluaciones según heurísticas

## 5.4. Video About-the-Product
