# Herramientas y conexiones para diagnosticar pedidos

Referencia revisada el 05/10/2026. Las capacidades, planes y disponibilidad cambian. Antes de indicar una instalación o compra, comprobar la documentación vigente y qué tiene habilitado el cliente. Estas herramientas son opciones, no dependencias de esta skill.

## Elegir la pieza que falta

| Necesidad | Pieza adecuada | Prueba mínima |
| --- | --- | --- |
| Repetir un método, formato o criterio | Skill o instrucciones estables | Ejecutar un caso normal y uno límite; comparar con ejemplos aprobados. |
| Aportar datos de la empresa | Proyecto, archivos o fuente conectada | Preguntar por un dato presente y otro ausente; comprobar que no invente. |
| Leer información actual en un servicio | Conector, MCP, API, exportación o navegador autorizado | Leer un registro conocido y confirmar cuenta, fecha y fuente. |
| Actuar en una app | Conector con capacidad de escritura o navegador autorizado | Preparar un borrador y verificar destino y permiso antes de ejecutar. |
| Analizar información pública a escala | Exportación, API o extractor especializado | Probar con una muestra pequeña, revisar campos, costo y límites. |

Una skill no concede acceso a servicios. Un prompt no instala herramientas ni supera un permiso denegado. En tareas simples, copiar una muestra o archivo puede ser el mejor primer paso.

## Instagram: cuatro objetivos distintos

1. **Ver o actuar en la cuenta propia desde Chrome.** La extensión de navegador de ChatGPT/Codex permite trabajar con el perfil y sesión ya abiertos en Chrome desde la aplicación de escritorio, sujeto a disponibilidad y permisos del sitio. Para instalarla, usar *Configuración > Computer Use > Chrome* en la app y verificar que la conexión figure activa. El navegador integrado de ChatGPT es otra opción cuando no se necesita ese perfil de Chrome. La extensión no garantiza por sí sola que se pueda publicar o acceder a mensajes. Fuente: https://learn.chatgpt.com/docs/chrome-extension
2. **Publicar contenido en una cuenta profesional.** Si el negocio usa HighLevel, Social Planner admite conectar cuentas Instagram Business o Creator para preparar, programar y publicar publicaciones compatibles. Una ruta técnica distinta es la API de Instagram con los permisos adecuados. Para una prueba inicial, preparar la publicación y revisar cuenta, pieza y fecha antes de enviarla. Fuentes: https://help.gohighlevel.com/support/solutions/articles/48001213003-how-to-connect-your-instagram-business-or-creator-account-with-your-facebook-account- y https://www.postman.com/meta/instagram/documentation/6yqw8pt/instagram-api
3. **Leer y seguir mensajes privados del negocio.** Si el negocio usa HighLevel, la integración Facebook & Instagram lleva los DM a *Conversations*; verificarla enviando un DM de prueba desde otra cuenta. Un scraper de publicaciones públicas no da acceso a esos mensajes. Fuente: https://help.gohighlevel.com/support/solutions/articles/155000005068
4. **Investigar publicaciones, perfiles o comentarios públicos.** El Actor `apify/instagram-scraper` de Apify extrae esos datos públicos y permite exportarlos o usarlos por API. Primero probar una muestra pequeña y revisar costo, calidad de datos y condiciones de uso. No sirve para publicar ni para leer DM privados. Fuente: https://apify.com/apify/instagram-scraper

Si el usuario solo dice «trabajar con Instagram», preguntar si quiere publicar, leer sus DM, analizar contenido público o revisar la cuenta en el navegador. Esas respuestas cambian por completo la recomendación.

## Prospección B2B

- **Apollo** sirve para buscar personas y empresas por filtros, guardar listas y, según configuración, organizar secuencias de contacto. Es una opción cuando el problema es construir una lista B2B y operar prospección. Confirmar mercado objetivo, calidad de datos, plan/créditos y el canal antes de sugerir automatizar envíos. Fuentes: https://knowledge.apollo.io/hc/en-us/articles/4412658716941-Search-for-People y https://knowledge.apollo.io/hc/en-us/articles/4409237165837-Sequences-Overview
- **LinkedIn Sales Navigator** sirve para descubrir y seguir leads y cuentas dentro de LinkedIn con filtros y señales. Algunas funciones de sincronización con CRM requieren un plan específico; no asumir que el usuario puede exportar o enviar mensajes automáticamente desde la IA. Fuente: https://business.linkedin.com/sell/sales-navigator

Si todavía no está definido el cliente ideal, empezar por un perfil y una muestra pequeña de prospectos antes de recomendar una base o automatización. Recomendar Apollo, Sales Navigator o ambos según origen de datos y flujo buscado; explicar la diferencia en una frase y no convertir los nombres en una lista de compras.
