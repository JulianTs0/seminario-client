# 🎸 Fortune Client - Professional Web Interface

Este proyecto es la interfaz de usuario moderna y escalable para la plataforma social Fortune. Ha sido diseñada con un enfoque en la experiencia del usuario (UX) para músicos, bandas y gestores culturales, permitiendo una gestión fluida de comunidades artísticas desde un entorno web de alto rendimiento.

---

## 🚀 1. ¿De qué se trata el proyecto?
**Fortune Client** es una aplicación web de última generación construida con **React 19**, **TypeScript** y **Vite**. La arquitectura del proyecto sigue rigurosamente los principios de **Clean Architecture** y **Hexagonal**, lo que garantiza una separación clara entre la lógica de negocio (dominio) y el framework de UI. La interfaz se organiza mediante la metodología de **Atomic Design**, proporcionando un sistema de componentes modular, mantenible y consistente.

---

## 🎯 2. ¿Para qué sirve?
El sistema proporciona un ecosistema digital completo para la comunidad musical, integrando:
- **Red Social Interactiva:** Publicaciones multimedia, sistema de votos y comentarios anidados para artistas y fans.
- **Perfiles Dinámicos:** Páginas especializadas para músicos individuales, bandas y espacios culturales con gestión de membresías.
- **Comunicación en Tiempo Real:** Mensajería instantánea mediante WebSockets para la interacción fluida entre miembros de la comunidad.
- **Gestión de Eventos:** Calendarios interactivos y administración de fechas con control de asistencia y cronogramas en tiempo real.
- **Control Administrativo:** Herramientas integradas para moderación de contenido, gestión de catálogos y gobernanza de la plataforma.

---

## 👥 3. ¿A quién le sirve?
- **Artistas y Músicos:** Que busquen una plataforma profesional para difundir su trabajo, conectar con colegas y hacer crecer su audiencia local.
- **Bandas y Colectivos:** Que necesiten un espacio centralizado para gestionar su presencia digital, integrantes y agenda de presentaciones.
- **Gestores y Locales Culturales:** Que deseen promocionar sus eventos y alcanzar a un público objetivo segmentado por intereses musicales.
- **Ingenieros de Software:** Que busquen un caso de estudio real sobre la implementación de microservicios (Backend) y Clean Architecture (Frontend).

---

## ⚙️ 4. Configuración y Setup

### Requisitos previos
- **Node.js 20+**: Entorno de ejecución recomendado.
- **NPM o PNPM**: Gestor de paquetes para la resolución de dependencias.

### Preparación del Entorno
1. Navega al directorio raíz del cliente:
   ```bash
   cd seminario-client
   ```
2. Instala las dependencias del proyecto:
   ```bash
   npm install
   ```

### Variables de Entorno (`.env`)
Configura la comunicación con el backend creando un archivo `.env` en la raíz de `seminario-client` con los siguientes parámetros:

| Variable | Descripción | Valor Predeterminado |
| :--- | :--- | :--- |
| `VITE_BASE_URL` | URL del API Gateway (Backend) | `http://localhost:4040/api/v1` |
| `VITE_WEBSOCKET_URL` | Endpoint para la conexión de Chat | `ws://localhost:4040/ws` |

### Comandos de Desarrollo
| Comando | Función |
| :--- | :--- |
| `npm run dev` | Inicia el entorno de desarrollo con recarga rápida (HMR). |
| `npm run build` | Genera el bundle optimizado para producción. |
| `npm run preview` | Previsualiza localmente la versión productiva generada. |

---

## 🏛️ Organización Técnica (`/src`)
La estructura de directorios refleja el compromiso con la arquitectura de capas y la calidad del software:
- **Domain:** Entidades de negocio, DTOs y contratos (interfaces) de repositorios.
- **Infrastructure:** Implementaciones concretas de servicios, APIs y adaptadores de datos.
- **UI:** Componentes organizados por niveles (Atoms, Molecules, Organisms), Hooks personalizados y ViewModels de vista.
- **Core:** Adaptadores base (Axios), proveedores de estado global y utilidades transversales.
