# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management
### 5.1.1. Software Development Environment Configuration
### 5.1.2. Source Code Management
### 5.1.3. Source Code Style Guide & Conventions

As a general rule, all code must be written in English and follow the conventions defined in the following reference guides:

* **HTML Style Guide and Coding Conventions**
* **Google HTML/CSS Style Guide**
* **Vue Style Guide**
* **Google JavaScript Style Guide**
* **MDN JavaScript Guidelines**
* **W3C JavaScript Style Guide**
* **Gherkin Conventions for Readable Specifications**
* **C# Coding Conventions**
* **Microsoft ASP.NET Core Coding Guidelines**

## HTML

* **Element names in lowercase**
```html
<body> <p>This is a paragraph</p> </body>
```

* **Close all elements**
```html
<p>First paragraph</p> <p>Second paragraph</p>
```

* **Attribute names in lowercase**
```html
<img src="logo.png" alt="Logo">
```

* **Always use** `alt`, `width` and `height` in `<img>`
```html
<img src="avatar.jpg" alt="User avatar" width="128" height="128">
```

* **No spaces around** `=`
```html
<link rel="stylesheet" href="styles.css">
```

## CSS

* **Meaningful IDs and classes**, in kebab-case
```css
#gallery { … } .video-player { … }
```

* **Shorthand properties**
```css
margin: 0; padding: 0 1em; font: 100%/1.6 serif;
```

* **Zero value without unit**
```css
margin: 0; padding: 0;
```

* **Alphabetical order of declarations**
```css
background: #fff; border-radius: 4px; color: #000;
```

* **Single quotes for attribute selectors**
```css
font-family: 'Open Sans', sans-serif;
```

## JavaScript

* **One statement per line**, braces on the same line as declaration
```js
function calculateTotal(a, b) { return a + b; }
```

* **lowerCamelCase** for variables and functions
```js
let eventCount = 0; function registerUser() { … }
```

* **Use** `const` and `let`, avoid `var`
```js
const maxEvents = 10; let currentUser = null;
```

* **Spaces around operators and after commas**
```js
let sum = x + y; const genres = ['rock', 'jazz', 'pop'];
```

## C#

* **PascalCase** for classes, methods and properties
```csharp
public class EventManager { public void ProcessBooking() { … } }
```

* **camelCase** for local variables and parameters
```csharp
int eventId; string venueName;
```

* **Reasonable line length** (max. ~120 characters)
* **Clear and concise comments**
* **Single responsibility principle**: each class or method with a single function

## Gherkin

* **Descriptive scenario titles**
```gherkin
Feature: User login Scenario: Successful authentication Given a registered user When they enter valid credentials Then they see the dashboard
```

* **Always use Given-When-Then**, indent `And` with two additional spaces
* **Scenario Outline** for parameterized examples
* **Business-readable language**, without implementation details
* **Separate scenarios with comment**
```gherkin
# -------------------------- Scenario: Password reset …
```


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
