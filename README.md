<div align="center">

# 📅 DateJS Library - Manipulación avanzada de fechas

### Librería JavaScript para trabajar con fechas de forma inteligente
*Extensión completa del objeto Date con localización en español*

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/es/docs/Web/JavaScript)
[![ES6+](https://img.shields.io/badge/ES6+-Ready-brightgreen?style=for-the-badge)](https://www.ecma-international.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

</div>

---

## 📚 Tabla de Contenidos

- [📖 Descripción](#-descripción)
- [✨ Características](#-características)
- [🗂️ Estructura](#️-estructura)
- [🚀 Instalación](#-instalación)
- [💡 Ejemplos](#-ejemplos-de-uso)
- [📚 Módulos](#-módulos-disponibles)
- [👨‍💻 Autor](#-autor)

---

## 📖 Descripción

**DateJS Library** es una librería JavaScript que extiende el objeto `Date` nativo, añadiendo funcionalidades avanzadas para manipular, parsear y formatear fechas. Incluye localización en español (ES-ES) y sintaxis natural.

---

## ✨ Características

- 🌍 **Localización en español (ES-ES)**
- 📝 **Parser avanzado**: Interpreta "15 de marzo de 2024"
- 🔧 **Funciones helper**: addDays, addMonths, isAfter, etc.
- 🎯 **Sugar Syntax**: `Date.today()`, `(3).days().ago()`
- ⚡ **Sin dependencias**: JavaScript puro
- 📦 **Modular**: Carga solo lo que necesitas

---

## 🗂️ Estructura

```
JS-Date-Library/
├── libreria.minima.datejs/
│   ├── date-es-ES.js       # Localización española
│   └── datejs/
│       ├── core.js         # Núcleo
│       ├── date.js         # Extensiones Date
│       ├── parser.js       # Parser de fechas
│       ├── extras.js       # Funciones adicionales
│       ├── sugarpak.js     # Sintaxis simplificada
│       └── time.js         # Utilidades de tiempo
└── README.md
```

---

## 🚀 Instalación

```bash
git clone https://github.com/albertogarciaquintana5-jpg/JS-Date-Library.git
cd JS-Date-Library
```

### Incluir en HTML

```html
<script src="libreria.minima.datejs/datejs/core.js"></script>
<script src="libreria.minima.datejs/datejs/date.js"></script>
<script src="libreria.minima.datejs/date-es-ES.js"></script>
<script src="libreria.minima.datejs/datejs/parser.js"></script>
<script src="libreria.minima.datejs/datejs/sugarpak.js"></script>
```

---

## 💡 Ejemplos de uso

```javascript
// Fecha actual
var hoy = Date.today();

// Parsear fechas
var fecha = Date.parse('15 de marzo de 2024');

// Manipular
fecha.addDays(7);        // +7 días
fecha.addMonths(2);      // +2 meses

// Sugar Syntax
Date.tomorrow()
(3).days().ago()
Date.monday()

// Formatear
fecha.toString('dd/MM/yyyy');
```

---

## 📚 Módulos disponibles

| Módulo | Descripción |
|--------|-------------|
| **core.js** | Configuración base |
| **date.js** | Extensiones principales |
| **parser.js** | Interpretación de texto |
| **sugarpak.js** | Sintaxis azucarada |
| **date-es-ES.js** | Localización español |

---

## 👨‍💻 Autor

**Alberto García Quintana**

- 📧 Email: albertogarciaquintana5@gmail.com
- 🔗 GitHub: [@albertogarciaquintana5-jpg](https://github.com/albertogarciaquintana5-jpg)

---

<div align="center">

### ⭐ Si te resulta útil, ¡dale una estrella!

**Desarrollado con 💙 para la comunidad JavaScript 📅**

</div>
