<div align="center">

# ⏰ JS-Date-Library 📅

### Librería JavaScript para manipulación avanzada de fechas

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/es/docs/Web/JavaScript)
[![ES6+](https://img.shields.io/badge/ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://www.ecma-international.org/)
[![Library](https://img.shields.io/badge/Type-Library-blue?style=for-the-badge)](https://github.com/albertogarciaquintana5-jpg/JS-Date-Library)
[![MIT License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

```
╔══════════════════════════════════════════════════════════════╗
║                                                              ║
║     ██████╗  █████╗ ████████╗███████╗     ██╗███████╗      ║
║     ██╔══██╗██╔══██╗╚══██╔══╝██╔════╝     ██║██╔════╝      ║
║     ██║  ██║███████║   ██║   █████╗       ██║███████╗      ║
║     ██║  ██║██╔══██║   ██║   ██╔══╝  ██   ██║╚════██║      ║
║     ██████╔╝██║  ██║   ██║   ███████╗╚█████╔╝███████║      ║
║     ╚═════╝ ╚═╝  ╚═╝   ╚═╝   ╚══════╝ ╚════╝ ╚══════╝      ║
║                                                              ║
║          🕐 Manipulación Avanzada de Fechas 🕐              ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝
```

</div>

---

## 📖 Descripción

**DateJS** es una librería JavaScript robusta y completa para la manipulación avanzada de fechas con localización en español. Extiende el objeto nativo `Date` de JavaScript con funciones poderosas, un parser inteligente de fechas en lenguaje natural y una sintaxis elegante y expresiva.

**Características principales:**
- 🌍 Localización completa en español (ES-ES)
- 📝 Parser avanzado que interpreta fechas en lenguaje natural
- 🔧 Amplias utilidades para manipulación de fechas
- 🎯 Sugar Syntax para código más legible y expresivo
- ⚡ Librería ligera sin dependencias externas
- 📦 Arquitectura modular con core + extensiones opcionales
- 🔄 Métodos encadenables para operaciones fluidas

---

## ✨ Características principales

| Característica | Descripción |
|----------------|-------------|
| 🌍 **Localización** | Soporte completo para español (ES-ES) con nombres de meses y días |
| 📝 **Parser avanzado** | Interpreta fechas en lenguaje natural como "15 de marzo de 2024" |
| 🔧 **Utilidades** | Funciones helper para añadir días, comparar fechas, formatear, etc. |
| 🎯 **Sugar Syntax** | Sintaxis simplificada y elegante: `Date.today()`, `(3).days().ago()` |
| ⚡ **Ligera** | Sin dependencias externas, JavaScript puro |
| 📦 **Modular** | Core + extensiones opcionales según necesidades |
| 🔄 **Chainable** | Métodos encadenables para operaciones secuenciales |

---

## 🗂️ Estructura del Proyecto

```
JS-Date-Library/
├── libreria.minima.datejs/
│   ├── date-es-ES.js       # Localización española
│   └── datejs/
│       ├── core.js         # Núcleo de la librería
│       ├── date.js         # Extensiones de Date
│       ├── extras.js       # Funciones adicionales
│       ├── parser.js       # Parser de fechas
│       ├── sugarpak.js     # Sintaxis simplificada
│       └── time.js         # Utilidades de tiempo
└── README.md
```

---

## 🚀 Instalación

### Descarga manual

```bash
git clone https://github.com/albertogarciaquintana5-jpg/JS-Date-Library.git
cd JS-Date-Library
```

### Incluir en HTML

```html
<!-- Cargar núcleo -->
<script src="libreria.minima.datejs/datejs/core.js"></script>
<script src="libreria.minima.datejs/datejs/date.js"></script>

<!-- Cargar localización española -->
<script src="libreria.minima.datejs/date-es-ES.js"></script>

<!-- Cargar módulos opcionales -->
<script src="libreria.minima.datejs/datejs/parser.js"></script>
<script src="libreria.minima.datejs/datejs/sugarpak.js"></script>
<script src="libreria.minima.datejs/datejs/extras.js"></script>
<script src="libreria.minima.datejs/datejs/time.js"></script>
```

---

## 💡 Ejemplos de uso

### Crear fechas

```javascript
// Fecha actual
var hoy = Date.today();

// Fechas específicas
var fecha = Date.parse('15 de marzo de 2024');
var navidad = Date.parse('25 diciembre 2024');

// Con sintaxis natural
var manana = Date.today().addDays(1);
var proximaSemana = Date.today().next().week();
```

### Manipular fechas

```javascript
// Sumar/restar tiempo
var fecha = new Date();
fecha.addDays(7);        // +7 días
fecha.addMonths(2);      // +2 meses
fecha.addYears(1);       // +1 año

// Comparaciones
if (fecha1.isAfter(fecha2)) {
    console.log('fecha1 es posterior');
}

// Formatear
var texto = fecha.toString('dd/MM/yyyy');
var hora = fecha.toString('HH:mm:ss');
```

### Sugar Syntax

```javascript
// Sintaxis natural y legible
Date.today()
Date.yesterday()
Date.tomorrow()

(3).days().ago()
(2).weeks().fromNow()
Date.monday()
Date.march()
```

---

## 🛠️ Módulos disponibles

| Módulo | Archivo | Descripción |
|--------|---------|-------------|
| **Core** | `core.js` | Funciones base y configuración |
| **Date** | `date.js` | Extensiones principales de Date |
| **Parser** | `parser.js` | Interpretación de fechas en texto |
| **Extras** | `extras.js` | Utilidades adicionales |
| **SugarPak** | `sugarpak.js` | Sintaxis azucarada |
| **Time** | `time.js` | Manipulación de tiempo |
| **ES-ES** | `date-es-ES.js` | Localización español |

---

## 📚 API Reference

### Métodos principales

```javascript
// Obtención
Date.today()              // Fecha actual (00:00:00)
Date.yesterday()          // Ayer
Date.tomorrow()           // Mañana
Date.parse(string)        // Parsear string a fecha

// Manipulación
.addDays(n)              // Añadir días
.addMonths(n)            // Añadir meses
.addYears(n)             // Añadir años
.addHours(n)             // Añadir horas
.addMinutes(n)           // Añadir minutos
.addSeconds(n)           // Añadir segundos

// Comparación
.equals(date)            // Igualdad
.isAfter(date)           // Es posterior
.isBefore(date)          // Es anterior
.between(start, end)     // Está entre
.isToday()               // Es hoy
.isSameDay(date)         // Es el mismo día

// Formateo
.toString(format)        // Convertir a string
.toISOString()           // Formato ISO
```

---

## 🌍 Localización

Actualmente soporta:
- ✅ **Español (ES-ES)**: `date-es-ES.js`

### Configurar idioma

```javascript
Date.CultureInfo = Date.CultureInfo.ES;
```

**Nombres de meses en español:**
- enero, febrero, marzo, abril, mayo, junio, julio, agosto, septiembre, octubre, noviembre, diciembre

**Nombres de días en español:**
- domingo, lunes, martes, miércoles, jueves, viernes, sábado

---

## ⚡ Performance

- 📦 **Tamaño**: ~99KB total (todos los módulos)
- ⚡ **Carga rápida**: Módulos independientes para cargar solo lo necesario
- 🔧 **Sin dependencias**: JavaScript puro, sin librerías externas
- 🎯 **Optimizado**: Listo para uso en producción

---

## 🧪 Testing

```bash
# Abrir en navegador para testing manual
# Los archivos incluyen ejemplos de uso
```

Para probar la librería, simplemente incluye los archivos en una página HTML y abre la consola del navegador para experimentar con las funciones.

---

## 📸 Casos de uso

- ✅ Aplicaciones de calendario
- ✅ Sistemas de reservas
- ✅ Gestión de eventos
- ✅ Recordatorios y alarmas
- ✅ Reportes temporales
- ✅ Análisis de datos por fecha
- ✅ Formularios con validación de fechas
- ✅ Dashboards con filtros temporales

---

## 🤝 Contribuir

Las contribuciones son bienvenidas. Para contribuir:

1. Fork el proyecto
2. Crea tu rama de feature (`git checkout -b feature/NuevaFuncion`)
3. Commit tus cambios (`git commit -m 'Add: Nueva función'`)
4. Push a la rama (`git push origin feature/NuevaFuncion`)
5. Abre un Pull Request

---

## 📄 Licencia

MIT License - ver [LICENSE](LICENSE)

Este proyecto está bajo la Licencia MIT, lo que significa que puedes usarlo libremente en proyectos personales y comerciales.

---

## 👨‍💻 Autor

**Alberto García Quintana**

- 📧 Email: albertogarciaquintana5@gmail.com
- 🔗 GitHub: [@albertogarciaquintana5-jpg](https://github.com/albertogarciaquintana5-jpg)
- 💼 LinkedIn: [Alberto García Quintana](https://linkedin.com/in/albertogarciaquintana)

---

## 🔗 Enlaces útiles

- 📖 [Documentación original DateJS](http://www.datejs.com/)
- 📘 [MDN - Date Object](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/Date)
- 🌐 [JavaScript Info - Date and Time](https://javascript.info/date)

---

<div align="center">

**⭐ Si este proyecto te resulta útil, considera darle una estrella en GitHub ⭐**

Made with ❤️ by [Alberto García Quintana](https://github.com/albertogarciaquintana5-jpg)

</div>
