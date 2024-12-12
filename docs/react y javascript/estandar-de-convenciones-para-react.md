## Flujo de ramas de git y git hub
- Rama por defecto: `staging`
- Rama de produccion: `production`
- Las ramas de trabajo deben ser creadas desde `staging`, luego hacer las pull requests a esa misma rama `staging`
- Y despues de unir pull requests, se debe unir `staging` a `production` para que se publiquen los cambios

## Buenas prácticas en código
- En general el propósito es tener código limpio
- No escribir código en español, como: variables, clases y comentarios, entre otras cosas.
- No dejar código comentando, sino dejar siempre solo código que se usa
- Usar lineas de espacio entre bloques de código de una linea o 2 pero no más
- Organizar los importes por tipo

## Estructura de archivos y carpetas con buena manera de nombrarlos
```
react-website/
│
├── public/
│   └── favicon.ico
│
├── src/
│   ├── assets/
│   │   ├── images/
│   │   │   ├── logo.png
│   │   │   ├── home/
│   │   │   │   └── team-picture.jpg
│   │   ├── icons/
│   │   │   ├── arrow.svg
│   │   │   ├── person.svg
│   │   │   └── burger-menu.svg
│   │
│   ├── components/
│   │   ├── global/
│   │   │   ├── Header/
│   │   │   │   ├── Header.jsx
│   │   │   │   └── Header.css
│   │   │   ├── Footer/
│   │   │   │   ├── Footer.jsx
│   │   │   │   └── Footer.css
│   │   │
│   │   └── home/
│   │       ├── HeroBanner.jsx
│   │       └── HeroBanner.css
│   │
│   ├── pages/
│   │   ├── Home/
│   │   │   ├── Home.jsx
│   │   │   └── Home.css
│   │   │
│   │   ├── About/
│   │   │   ├── About.jsx
│   │   │   └── About.css
│   │   │
│   │   ├── Services/
│   │   │   ├── Services.jsx
│   │   │   └── Services.css
│   │   │
│   │   ├── Projects/
│   │   │   ├── Projects.jsx
│   │   │   └── Projects.css
│   │   │
│   │   └── Contact/
│   │       ├── Contact.jsx
│   │       └── Contact.css
│   │
│   ├── App.jsx
│   ├── App.css
│   └── main.jsx
│
├── .gitignore
├── index.html
├── package.json
├── vite.config.js
└── README.md
```

## Tabla de convención de nombres para tipos de carpetas y tipos de archivos
| File/Folder Type | Naming Convention | Examples | Notes |
|-----------------|-------------------|----------|-------|
| Project Folder | kebab-case | `my-react-project` | Use lowercase with hyphens |
| Source Folder | lowercase | `src` | Standard practice |
| Page Folders | PascalCase | `Home`, `About`, `Services` | Represents main routes/pages |
| Page Components | PascalCase with Page suffix | `HomePage`, `AboutPage`, `ServicesPage` | Clearly indicates it's a full page component |
| Regular Components | PascalCase | `Header`, `Button`, `UserCard` | Start with a descriptive noun |
| Component Subfolders | lowercase | `global`, `shared`, `layout` | Descriptive but simple |
| CSS Files | Same name as component | `Header.css`, `Button.css` | Matches corresponding component |
| Test Files | ComponentName.test.js | `Header.test.js`, `Button.test.js` | Add `.test` before extension |
| Hook Files | useCamelCase | `useAuth`, `useForm`, `useLocalStorage` | Start with `use` |
| Context Files | PascalCase with Context suffix | `AuthContext`, `ThemeContext` | Clearly indicates it's a context |
| Utility/Helper Files | camelCase | `formatDate`, `validateEmail` | Describes function purpose |
| Asset Folders | lowercase | `images`, `icons`, `fonts` | Plural, descriptive names |
| Configuration Files | lowercase | `vite.config.js`, `.eslintrc` | Standard naming |
