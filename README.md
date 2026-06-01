ENLACE VIDEO CONTEXTO GRUPO: https://www.youtube.com/watch?v=FfrXUTNh3lQ
ENLACE INDIVIDUAL DUAL: https://www.youtube.com/watch?v=XVfCcizEyXc

# 🥖 Prácticas Duales — Panadería Confitería Salvador

**Alumno:** José María López González  
**Empresa:** Panadería Confitería Salvador  
**Duración:** Febrero 2026 – Mayo 2026 (~16 semanas)  
**Ciclo:** Desarrollo de Aplicaciones Multiplataforma (DAM)

---

## 📋 Descripción del proyecto

Migración de una aplicación web interna desarrollada en **ASP clásico** a una arquitectura moderna:

- **Frontend:** Angular 20 + Ionic 8 (TypeScript, SCSS, Tailwind CSS)
- **Backend:** Node.js + Express.js
- **Base de datos:** Microsoft SQL Server (ERP Sage, sin modificar)
- **Móvil:** Compilación nativa iOS/Android con Capacitor

La aplicación controla la fabricación, el consumo de materias primas, las rutas de reparto y las compras de la panadería, integrada directamente con el ERP Sage.

---

## 🛠️ Herramientas utilizadas

| Categoría | Herramienta |
|---|---|
| Frontend | Angular 20, Ionic 8, TypeScript, HTML5, SCSS, Tailwind CSS |
| Backend | Node.js, Express.js, librería `mssql` |
| Base de datos | Microsoft SQL Server (ERP Sage) |
| Móvil | Capacitor (compilación nativa iOS/Android) |
| Control de versiones | Git, GitHub |
| IDE | Visual Studio Code |
| Gestión de paquetes | npm |
| Depuración | Chrome DevTools, consola de Node.js |
| Despliegue | Servidor local de la empresa |

---

## 📅 Progreso por semanas

| Período | Tarea |
|---|---|
| Semanas 1–2 (3–14 Feb) | Análisis del sistema legacy, configuración del entorno, autenticación |
| Semanas 3–4 (17–28 Feb) | Primeras pantallas, componentes base, ajustes de estilos |
| Semanas 5–8 (Marzo) | Componentes avanzados, optimización de backend y consultas SQL |
| Semanas 9–10 (1–16 Abr) | Pantallas de fabricación y rutas, adaptación a tablets/móvil |
| Semanas 11–13 (17 Abr – 5 May) | Pantalla central del obrador (más compleja), migración de lógica legacy |
| Semanas 14–16 (Mayo) | Refinamiento, corrección de consumos, testing con datos reales |

---

## 📚 Conocimientos aplicados por módulo

<details>
<summary><strong>📦 Acceso a Datos (AD)</strong></summary>

- Consultas SQL complejas con múltiples JOINs entre tablas relacionadas
- Procedimientos y transacciones (`BEGIN TRANSACTION`, `COMMIT`, `ROLLBACK`) para garantizar integridad
- Consultas parametrizadas para prevenir SQL Injection
- Paginación y filtrado de datos por fechas, turnos, series y ejercicios
- Mapeo de resultados de BD a objetos TypeScript (DTOs)
- Pool de conexiones a SQL Server con la librería `mssql`
- CRUD completo: INSERT de movimientos de stock, SELECT de órdenes, UPDATE de cantidades fabricadas
- Relaciones entre tablas: `Articulos`, `MovimientoStock`, `AcumuladoStock`, `_PS_NececidadesFAbricacion`

</details>

<details>
<summary><strong>🖥️ Desarrollo de Interfaces (DI)</strong></summary>

- Componentes reutilizables (standalone components en Angular)
- Uso de pipes de Angular (`date`, `number`, `slice`) para formatear datos en la vista
- Directivas estructurales: `@if`, `@for` (nueva sintaxis de Angular 17+)
- Binding de datos: one-way (`[prop]`), event binding (`(click)`), two-way (`[(ngModel)]`)
- Señales reactivas (`signal`, `computed`, `update`) de Angular 20 para gestión de estado
- Lazy loading de módulos y rutas para optimizar la carga inicial
- Guardas de ruta (`CanActivate`) para proteger páginas con autenticación
- Servicios e inyección de dependencias con `Injectable` y `inject()`
- Gestión de estado sin librerías externas (usando solo signals y computed)
- Observables y RxJS (`subscribe`, `pipe`, `map`, `catchError`) para llamadas HTTP

</details>

<details>
<summary><strong>📱 Programación Multimedia y Dispositivos Móviles (PMDM)</strong></summary>

- Ionic Framework con componentes nativos (`IonButton`, `IonList`, `IonRefresher`...)
- Capacitor para generar APK nativa desde código web
- Diseño responsive adaptado a tablets y móviles con CSS Grid y Flexbox
- Gestos táctiles y botones grandes adaptados a uso con guantes en entorno industrial
- Teclado numérico personalizado en pantalla (sin teclado físico)
- Mapas interactivos con posicionamiento de elementos sobre imagen de planta real
- Pull to refresh con `IonRefresher` para actualizar datos manualmente
- Toast notifications y `AlertController` para feedback al usuario
- Navegación con parámetros por URL (`ActivatedRoute`, `Router`)

</details>

<details>
<summary><strong>🏢 Sistemas de Gestión Empresarial (SGE)</strong></summary>

- Integración con ERP Sage directamente sobre su base de datos SQL Server
- Comprensión del flujo de fabricación: orden → consumo MMPP → registro de stock → cierre
- Autoconsumo de materias primas: el sistema descuenta stock automáticamente al anotar
- Gestión de almacenes con control de stock por partidas, lotes y fechas de caducidad
- Valoración de stock FIFO/LIFO en los movimientos
- Escandallo: cálculo proporcional de ingredientes según la cantidad a fabricar
- Migración de lógica legacy de ASP clásico a arquitectura moderna manteniendo compatibilidad
- API REST diseñada siguiendo convenciones estándar (verbos HTTP, códigos de estado, JSON)
- JWT (JSON Web Tokens) para autenticación sin estado entre cliente y servidor
- Variables de entorno (`.env`) para gestión segura de credenciales

</details>

---

## 💬 Valoración personal

### Lo que más valoro

- Trabajar con un **proyecto real en producción**: los datos son reales y los errores tienen consecuencias reales en el stock y la fabricación.
- Aprender a leer y entender **código legacy** (ASP clásico) para traducirlo a tecnologías modernas, respetando la lógica de negocio existente.
- La experiencia de trabajar con una base de datos de empresa real con millones de registros y comprender cómo funciona un ERP como Sage por dentro.
- Desarrollar habilidades de **resolución de problemas** en un entorno profesional: debugging con datos reales, comunicación con el equipo y pruebas en producción.

### Dificultades superadas

- La complejidad de las **consultas SQL**, especialmente las transacciones de stock que implican múltiples tablas y deben ser atómicas.
- Entender la **lógica de negocio del sector panadero** (escandallo, masas, partidas, autoconsumo).
- Adaptar interfaces para **uso industrial** (tablets con pantallas sucias/guantes).

---

> Prácticas realizadas en el marco de la Formación Dual del ciclo **Desarrollo de Aplicaciones Multiplataforma (DAM)** · 2026
