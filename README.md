# Skills de LYP

Un paquete de skills para trabajar con IA en tu empresa, con Claude o con Codex.

Una **skill** es un procedimiento guardado: le enseña a la IA cómo hacer una tarea que se repite, con tus reglas, y la usa cada vez que esa tarea aparece. No tenés que volver a explicarle todo en cada conversación.

## Qué trae

| Skill | Para qué sirve | Autor |
|---|---|---|
| [`mejora-tu-pedido`](skills/mejora-tu-pedido) | Convierte lo que le querés pedir a una IA, escrito o dictado como te salga, en un pedido claro y comprobable. Si lo que falta no es redacción sino una herramienta, una conexión o un permiso, te lo dice. | LYP |
| [`informe-semanal`](skills/informe-semanal) | Arma el informe semanal de tu empresa con lo que haya en tu carpeta y en tus aplicaciones conectadas: qué pasó, los números con su fuente, lo pendiente y lo que conviene decidir. No inventa números. | LYP |
| Las 15 skills de n8n (`n8n-…` y `using-n8n-mcp-skills`) | Para construir automatizaciones en n8n con Claude o con Codex: patrones de flujos, configuración de nodos, expresiones, código, validación, agentes y errores. | [Romuald Członkowski](https://github.com/czlonkowski/n8n-skills), licencia MIT |

**Las skills de documentos de Anthropic** (Word, Excel, PowerPoint y PDF) no están copiadas acá porque su licencia no lo permite. En el chat de Claude ya vienen incluidas en todas las cuentas, con la opción de ejecución de código activada ([ayuda de Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude)). Para usarlas en Claude Code, seguí las instrucciones del [repositorio oficial de Anthropic](https://github.com/anthropics/skills).

## Cómo se instala

La forma más simple es pedírselo a la IA, dentro de la carpeta donde la vas a usar.

1. Abrí en Claude Code o en Codex la carpeta principal de tu empresa, o el proyecto donde quieras la skill.
2. Copiá el mensaje que corresponde, cambiá el nombre de la skill si querés otra y envialo.
3. Cuando termine, pedile que te muestre qué instaló y dónde.

**En Claude Code:**

```
Instalá la skill mejora-tu-pedido del repositorio https://github.com/lautaropuebla-ia/skills-lyp en este proyecto, dentro de la carpeta .claude/skills. Copiá la carpeta completa de la skill sin cambiarle nada y después decime qué instalaste.
```

**En Codex:**

```
Instalá la skill mejora-tu-pedido del repositorio https://github.com/lautaropuebla-ia/skills-lyp en este proyecto, dentro de la carpeta .agents/skills. Copiá la carpeta completa de la skill sin cambiarle nada y después decime qué instalaste.
```

Para instalar varias, nombralas en el mismo mensaje. Para las de n8n: «todas las skills que empiezan con n8n- y using-n8n-mcp-skills».

**Dónde queda disponible:** una skill instalada en una carpeta se usa cuando trabajás en esa carpeta. Si la querés en todos tus proyectos, pedí que la instale en tu carpeta personal de skills: `~/.claude/skills` para Claude Code y `~/.agents/skills` para Codex.

**En el chat de Claude o en Cowork**, las skills se suben como un archivo ZIP desde la configuración de Claude, en el apartado de skills ([ayuda de Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude)). Si no sabés armar el ZIP, pedíselo a Claude Code: «Armame un ZIP de la carpeta de la skill mejora-tu-pedido para subirla al chat de Claude».

## Cómo se usa

No hace falta llamarla: la IA lee la descripción de cada skill y la usa cuando tu pedido coincide. Si querés llamarla a propósito, en Claude Code escribí `/` y su nombre, y en Codex escribí `$` y su nombre.

Probala con un caso real y mirá lo que devuelve. Si algo no sale como esperabas, contale qué esperabas y qué hizo: es la forma más rápida de ajustarla.

## Cuidado

- Una skill es texto con instrucciones. Antes de instalar una de otro autor, leé su `SKILL.md`: es como contratar a alguien, querés saber qué le estás pidiendo que haga.
- Ninguna skill de este paquete envía mensajes, publica ni borra nada por su cuenta. `informe-semanal` arma y guarda el informe; mandarlo es una decisión tuya.

## Licencias

- Las skills de n8n son de Romuald Członkowski, con licencia MIT. Cada una lleva su `LICENSE.txt`. Versión del 16/09/2026 (v1.35.0), tomada de [czlonkowski/n8n-skills](https://github.com/czlonkowski/n8n-skills), donde están las actualizaciones.
- `mejora-tu-pedido` e `informe-semanal` son de Lautaro Puebla (LYP), con [licencia MIT](LICENSE): las podés usar, copiar y adaptar para tu empresa manteniendo el aviso. Cada una lleva su `LICENSE.txt`.
