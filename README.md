# Safe paw site

Plataforma profesional diseñada para optimizar la operativa diaria de centros veterinarios. Interfaz clara, rendimiento excepcional y herramientas enfocadas en el bienestar animal y la eficiencia del equipo.

## Arquitectura
El proyecto sigue una estructura modular con responsabilidades bien definidas. 
La interfaz de usuario se construye con componentes reutilizables,
mientras que la lógica de negocio y el acceso a datos permanecen desacoplados.  

Se adopta un enfoque **static-first** con generación híbrida, lo que permite:
- Carga inicial ultrarrápida y navegación fluida.
- JavaScript mínimo en el cliente, solo donde es estrictamente necesario.
- Optimización SEO granular para cada página.
- Escalabilidad sin complicaciones gracias a la separación de capas.

## Stack Tecnológico
El sistema está construido sobre un stack moderno y probado en producción, seleccionado por su equilibrio entre rendimiento, seguridad y experiencia de desarrollo.

| Capa | Tecnología | Justificación |
| :--- | :--- | :--- |
| **Frontend** | Astro + Alpine.js | Astro genera HTML estático con cero JS por defecto, Alpine añade interactividad ligera sin complejidad de SPA. Bundle final ínfimo. |
| **Estilos** | UnoCSS | Motor de utilidades atómicas bajo demanda, más rápido que Tailwind, con un bundle CSS mínimo y personalización total. |
| **Backend** | Hono + Cloudflare Workers | Hono es un framework ultrarrápido para el edge. Desplegado en Workers proporciona latencia global baja y escalado automático. |
| **Base de Datos** | Neon | PostgreSQL serverless con branching instantáneo y escalado a cero. Ideal para entornos de desarrollo y producción sin gestión de servidores. |
| **ORM / Query** | Kysely | Query builder type-safe para TypeScript. Control total sobre el SQL generado, sin magia, y con soporte excelente para PostgreSQL. |
| **Autenticación** | Lucia | Librería agnóstica de framework para manejo de sesiones. Simple, flexible y compatible con múltiples adaptadores de base de datos. |

## Estado actual
La plataforma está **desplegada y operativa**, cubriendo las funcionalidades esenciales de la clínica:
- Página de inicio con información de servicios, equipo veterinario y valores del centro.
- Sistema de citas online con confirmación por email.
- Panel administrativo para gestionar horarios, mascotas y clientes.
- Integración con Google Maps y formulario de contacto.

## Proyección
Las próximas iteraciones se centrarán en añadir valor tanto para el personal como para los tutores:
- Portal del cliente con historial médico completo de sus mascotas.
- Recordatorios automáticos de vacunación y desparasitación vía SMS/WhatsApp.
- Pasarela de pagos para abonar servicios en línea.
- Módulo de fidelización con descuentos y promociones personalizadas.

## Paleta de colores
- `#0B4F6C` Azul marino – Encabezados, botones principales, confianza.
- `#3A7D8C` Verde azulado – Acentos, hover, elementos secundarios.
- `#F9F6F0` Beige claro – Fondo principal, tarjetas.
- `#E29578` Melocotón – Llamadas a la acción, iconos destacados.
- `#2B2D42` Gris oscuro – Texto principal, pie de página.

## Fuentes
- **Títulos:** Satoshi (moderna, geométrica, excelente legibilidad en pantalla).
- **Cuerpo de texto:** General Sans (elegante y versátil).
