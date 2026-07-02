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

#Prompt para mejorar la pagina...

4. Prompts de IA Refactorizados (Glassmorphism, Nav Isla y Secciones de Fotos)
Prompt para el Navbar Tipo Isla (Glassmorphism Dark/Light)

Actúa como un desarrollador frontend experto en UI/UX moderna. Genera el código HTML y CSS (usando Tailwind CSS) para una barra de navegación (Navbar) tipo ISLA FLOTANTE. 
Especificaciones de diseño:
- Debe estar centrada en la parte superior, separada de los bordes de la pantalla (con un margen superior de p. ej., mt-4), esquinas completamente redondeadas (rounded-full) y un borde sutil de 1px (#FFFFFF con opacidad baja o #222222 según el modo).
- Aplica un efecto Glassmorphism estricto: fondo blanco o negro con alta transparencia (p. ej., bg-white/10 o bg-black/40) y un desenfoque de fondo fuerte (backdrop-blur-md).
- El esquema es monocromático. El logo a la izquierda es solo texto: "tecno mobile" (fuente 'Space Grotesk' en negrita).
- Los enlaces a la derecha usan jerga paisa: Inicio, El Camello (Servicios), Visajes (Portafolio), La Historia, y un botón destacado tipo isla pequeña para "Contáctenos pues".
- Debe ser fixed en la parte superior y encogerse o mantenerse estilizada al hacer scroll, siendo 100% responsiva.

Prompt para la Sección Hero (Con Espacio para Fotografía Artística)

Genera el código para una sección Hero de impacto en blanco y negro, dividida en dos columnas responsivas (se vuelve 1 columna en móviles). 
- Columna Izquierda (Texto): Centrada verticalmente. Título principal (H1) en fuente 'Syne' extra-bold: "Tecnología con berraquera: Código, fierros y buena fotografía." Subtítulo en jerga paisa profesional: "Aquí no nos varamos por nada. Nos le medimos al desarrollo de software, al testing más riguroso, a equipos premium y a dejar su computador volando." Abajo, dos botones: uno negro sólido ("Ver el camello") y uno transparente con borde ("Hablemos pues").
- Columna Derecha (Fotografía): Un contenedor de imagen grande con esquinas redondeadas. Debe incluir un efecto de tarjeta flotante encima con Glassmorphism (bg-white/5, backdrop-blur-sm, borde fino) que muestre un texto minimalista como "Calidad 100% garantizada". La imagen de fondo simulada debe ser una fotografía artística de tecnología en blanco y negro de alta calidad.

Prompt para la Sección de Servicios ("El Camello" con Tarjetas Glass)

Diseña una sección de servicios llamada "El Camello" utilizando un sistema de Grid de 4 columnas responsivo. 
Para romper con el fondo plano, esta sección tendrá un fondo oscuro o un patrón geométrico muy sutil en blanco y negro, y las 4 tarjetas de servicios tendrán un diseño Glassmorphic premium:
- Fondo de las tarjetas: Negro translúcido (bg-black/30) o gris muy claro translúcido con un 'backdrop-blur-lg' potente.
- Bordes: Un contorno ultrafino de 1px brillante o semi-transparente para que resalten sobre el fondo.
- Iconos: Únicamente vectores lineales (Outline SVGs) en blanco o negro.
Genera el código para mostrar los 4 servicios con sus títulos en jerga paisa y descripciones profesionales:
1. Desarrollo & Testing a la Medida: "Programamos software robusto y le hacemos un testing tan fino que no se nos escapa nada. Código bien melo."
2. Fierros y Tecnología: "Venta de equipos, componentes y gadgets premium para que rinda en el día a día."
3. Fotografía Profesional: "Producción visual y dirección de arte digital. Capturamos la esencia de su proyecto con la mejor definición."
4. Soporte y Arreglo de Computadores: "Mantenimiento preventivo, diagnóstico y reparación para dejar su equipo como un cohete."

Prompt para la Sección "Visajes" (Galería/Portafolio de Fotografías y Proyectos)

Crea una sección de portafolio tipo Landing Page llamada "Visajes" en estricto blanco y negro. Esta sección está destinada a mostrar los trabajos de fotografía, desarrollo y maquetación.
- Estructura: Un sistema de galería tipo Masonry o Grid asimétrico para fotos de diferentes orientaciones (verticales y horizontales).
- Los contenedores de las imágenes deben tener esquinas redondeadas elegantes. 
- Al pasar el cursor sobre cada foto (hover), debe aparecer un "overlay" o capa flotante con efecto Glassmorphism (transparencia y desenfoque) que cubra la imagen suavemente y muestre en texto blanco el nombre del proyecto o la sesión fotográfica (ej. "Desarrollo Web", "Sesión de Producto", "Testing QA").
- Añade un espaciado limpio (gap amplio) entre las fotos para mantener la estética minimalista y limpia.

Prompt para la Sección "La Historia" (Storytelling Emprendedor)

Genera el código para la sección "La Historia: De la tierrita pal mundo." usando un bloque asimétrico en blanco y negro. 
A la izquierda, un bloque de texto con tipografía limpia ('Inter') que narre la historia de tecno mobile con tono paisa y honesto: "En tecno mobile empezamos con una caja de herramientas, muchas ganas de camellar y la firme convicción de que la tecnología no tiene por qué ser un dolor de cabeza...".
A la derecha, un contenedor grande para una fotografía del equipo o del taller en blanco y negro, la cual debe estar enmarcada por un contenedor contenedor externo que use un degradado suave o bordes flotantes para darle tridimensionalidad a la landing page.

https://claude.ai/share/64a95704-d28b-4cbb-84ef-9dc090133552
