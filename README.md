#PAGINA DE INICIO 

Technical & UX Design Review: tecno mobile
Este documento recopila las observaciones de testing de interfaz (UI), experiencia de usuario (UX) y consistencia de contenido para la reestructuración del sitio web, enfocándolo hacia la nueva oferta de servicios: venta de productos de tecnología, desarrollo de software, testing, fotografía y reparación de computadores.

1. Hallazgos Críticos y Errores de Consistencia
Incongruencia en Textos (Copywriting): Se detectó que la sección de beneficios incluye referencias a "vehículos" y "financiamiento de automóviles". Al ser una plataforma tecnológica, este contenido genera fricción cognitiva y debe ser depurado por completo para alinearse a la nueva oferta técnica.

Problema de Accesibilidad (Contraste): El botón de llamada a la acción (CTA) principal utiliza texto blanco sobre un fondo naranja con un ratio de contraste que dificulta la legibilidad. Toda la paleta debe migrar al estándar monocromático solicitado.

Erratas Tipográficas: El botón principal presenta una omisión de tilde en la palabra "catalogos" (debe ser "catálogos").

Control de Desbordamiento (Overflow): El menú de navegación superior experimenta problemas de empaquetado y solapamiento de elementos al alterar el zoom del navegador. Se requiere una reestructuración con Flexbox/Grid responsivo.

2. Nueva Propuesta de Diseño: Minimalismo Monocromático
Para proyectar una identidad corporativa sólida que abarque tanto la ingeniería de software como la fotografía, el sitio adoptará un estilo Strictly Black & White.

Arquitectura del Nav (Menú de Navegación)
Comportamiento: Posición fija (sticky / fixed) con transiciones suaves en scroll.

Secciones Reorganizadas: Inicio | Servicios (Desarrollo, Tienda Tech, Fotografía, Soporte) | Portafolio | Quiénes Somos | Contacto.

Sistema Tipográfico Sugerido (Google Fonts)
Combinación Tech/Modern:

Títulos (H1, H2, H3): Space Grotesk o Syne (Fuentes geométricas con mucha personalidad).

Cuerpo de texto: Inter o Roboto (Alta legibilidad para especificaciones técnicas y documentación).