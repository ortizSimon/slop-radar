# slop-radar

**Ayuda a tu IA a ser creativa de verdad y a salir del slop.**

La IA no es creativa porque se lo pidas: es creativa cuando le das de dónde agarrarse. slop-radar te dice dónde buscar buenos referentes para lo que estés haciendo, construye desde ellos y te saca del bucle cuando todo empieza a salir igual.

*Helps your AI be truly creative and get out of the slop: it teaches you where to find good references for whatever you're making, builds from them, and gets you out of the loop when everything starts coming out the same. [English below](#english).*

```
npx skills add ortizSimon/slop-radar -g -a claude-code
```

## El problema

Le pedí una metáfora sobre el tiempo a Claude, GPT y Gemini, en 15 chats nuevos. **14 empezaron con "El tiempo es un río".**

Sin un referente, la IA te da el centro de todo lo que vio: el promedio. Todas se entrenaron parecido, así que todas caen en el mismo lugar ([Jiang et al., NeurIPS 2025](https://arxiv.org/abs/2510.22954)). Y lo que hace casi todo el mundo empeora las cosas:

- **Pedirle "sé original"** no la saca: la vuelve rebuscada, y lo rebuscado también se nota hecho con IA.
- **Insistir en el mismo chat** arma un bucle: cada intento se apoya en los anteriores, y la IA da vueltas a la misma idea ([Laban et al., 2025](https://arxiv.org/abs/2505.06120)).

Lo único que la saca es algo que no tiene: **referentes reales y tu propio material.**

## Qué hace

**Un radar que la IA corre antes de mandarte algo.** ¿Es lo primero que se le ocurrió? ¿Le serviría igual a cualquiera que pidiera algo parecido? ¿Se parece a sus últimas respuestas? Si sí, no te lo manda así.

**En un chat nuevo**, si pedís algo creativo o la solución a un problema sin darle nada tuyo:
1. **Te dice en una línea qué te saldría** si lo hiciera ya, y por qué.
2. **Te pide una sola vez lo que falta:** 2 o 3 referentes y qué te gusta de cada uno (si es una web, una app o un video, mejor un video recorriéndolos), o tu situación real si es un problema, y lo que solo vos tenés.
3. **Te dice dónde buscar para ese caso:** quién lo hace bien de verdad y dónde lo muestra, qué campo vecino resolvió lo mismo y cómo se hacía antes de la moda. Sitios seguros, con qué buscar en cada uno. Si puede buscar en internet, te trae opciones con link y vos elegís.
4. **Construye desde eso** y te dice qué tomó de cada referente y qué sigue viéndose común.

**En un chat que ya da vueltas** (le rechazaste intentos, le pediste "más original", o todo empieza a salir igual), aunque la llames a mitad de camino:
1. **Te dice que están dando vueltas** y qué se repite en los intentos.
2. **Te pregunta qué está mal exactamente:** la idea, el tono, el look, la estructura.
3. **Te pide material nuevo, no otra versión.**
4. **Te da un brief para pegar en un chat nuevo**, porque un chat largo ya se ancló.

Sirve para textos, nombres, logos, imágenes, videos, páginas, apps, presentaciones, menús, y también para planes, ideas y consejos, donde lo genérico es igual de inútil. Si la tarea tiene una sola respuesta correcta (una cuenta, un error de código, un dato), no aparece. Si ya le das referentes, arma directo. Si le decís "rápido", lo hace y te avisa que sale más genérico. Te contesta en tu idioma.

## Así se ve

Respuestas reales de Claude Opus con la skill.

**Una página, en un chat nuevo:**

> **Vos:** Haceme una landing para mí. Soy creador de contenido de IA.
>
> **IA:** Si te la hago ya, te sale lo típico: fondo casi negro con un degradé violeta, un titular centrado tipo "Explorando el futuro de la IA", dos botones, tu foto con un brillo detrás, tres tarjetas con íconos y una fila de números de seguidores. Podría ser la de cualquier creador de IA porque no tengo nada tuyo.
>
> Para que sea tuya necesito: **2 o 3 webs que te gusten y qué te gusta de cada una** (si podés, una grabación de pantalla de cada una: la mitad de una web es cómo se mueve), **lo que solo tenés vos** y **para qué es la landing.**
>
> **Dónde buscar:** Recent (recent.design/websites), Typewolf › Portfolio sites…

**Un problema:**

> **Vos:** ¿Cómo consigo más clientes para mi panadería?
>
> **IA:** Si te respondo ya, te doy la lista de siempre: "define tu público, publica en Instagram, haz promociones, pide reseñas en Google". Esa lista le sirve igual a cualquier panadería, así que en la práctica no le sirve a ninguna.
>
> Me faltan: tu situación real (dónde está, cuántos clientes atendés, qué vendés más), qué ya probaste y cómo te fue, y lo que solo tiene la tuya. Y mirá cómo lo resuelven otros: leé las reseñas de 5 y de 1 estrella de las panaderías mejor calificadas de tu zona en Google Maps…

**Un chat que ya da vueltas** (después de tres bios rechazadas para un estudio de tatuajes):

> **IA:** Estamos dando vueltas en lo mismo. Si sigo en este chat, cada intento se apoya en los anteriores y no salimos de ahí.
>
> **Lo que se repite:** las tres bios tienen la misma estructura. Una frase poética sobre piel, tinta o alma, después "personalizado" y al final "escribinos por DM". Cambié las palabras, pero la idea fue siempre la misma. Y ninguna dice nada de *tu* estudio.
>
> **¿Qué es lo que no te cierra?** La idea, el tono, la estructura, o que no te representa…

## ¿Hace la diferencia?

La probamos en un juego de roles: un agente hizo de usuario real en tres casos (el logo de una panadería, la página de una app de finanzas, el menú de un restaurante). Sin la skill, pidió la pieza y después "hacelo más original". Con la skill, entró a los sitios que le recomendó, sacó capturas, eligió referentes y dijo qué le gustaba de cada uno. En los tres casos eligió la pieza hecha con la skill, y en una comparación a ciegas de esas piezas, yo elegí la de la skill en 2 y empaté en 1.

Lo que hay que decir: los usuarios fueron simulados y la muestra es chica. La skill no vuelve creativa a la IA por arte de magia: te pide 5 o 10 minutos para buscar referentes, y funciona mejor cuanto mejor es el modelo. Sin tus referentes, el resultado queda cerca de lo que daría cualquier IA.

## Instalar

- **Claude Code:** `npx skills add ortizSimon/slop-radar -g -a claude-code`
- **Claude (web y app):** bajá [`slop-radar.zip`](https://github.com/ortizSimon/slop-radar/raw/main/slop-radar.zip) de este repo, y en Claude andá a Personalizar → Skills → + → Crear skill → Subir una skill.
- **ChatGPT o Gemini:** pegá [`pegar/corta.md`](pegar/corta.md) en las instrucciones personalizadas, o [`pegar/completa.md`](pegar/completa.md) en las instrucciones de un proyecto, un GPT o un Gem.

## Adentro

- `SKILL.md`: el radar, el chat nuevo y el chat que da vueltas.
- `references/fuentes.md`: el método para encontrar referentes para cualquier pieza, cómo saber si una fuente es buena y segura, búsquedas listas para usar, y un banco de fuentes comprobadas por tipo de pieza (webs, apps, logos, tipografía, afiches, foto, 3D, video, textos, presentaciones, carruseles, packaging, menús, invitaciones, CV, ilustración, música, y problemas, planes y consejos).
- `references/defaults.md`: lo que la IA da por defecto en cada medio.

Las ideas se apoyan en [Verbalized Sampling](https://arxiv.org/abs/2510.01171) (por qué la IA arranca en lo típico), [Artificial Hivemind](https://arxiv.org/abs/2510.22954) (por qué todas caen en lo mismo) y [Laban et al.](https://arxiv.org/abs/2505.06120) (por qué los chats largos se traban). Licencia MIT. Hecha por [Simón Ortiz](https://simonortiz-ai.vercel.app).

---

## English

**slop-radar** helps your AI be truly creative and get out of the slop. An AI isn't creative because you ask it to be; it's creative when you give it something to hold on to.

**A radar the AI runs before sending you anything:** is it its first instinct, would it work the same for anyone who asked something similar, does it look like its last answers? If so, it doesn't send it as is.

**In a new chat**, when you ask for something creative or the solution to a problem without giving it anything of yours, it tells you in one line what would come out and why, asks once for what's missing (2 or 3 references and what you like in each, ideally a screen recording for sites, apps and video; or your real situation for a problem), teaches you where to find good references for that exact case (with safe sources and what to search in each), and builds from that.

**In a chat that's going in circles** (rejected attempts, "more original", everything looking the same), even if you call it midway, it says what keeps repeating, asks what exactly is wrong, asks for new input instead of a new version, and gives you a brief to paste into a fresh chat.

Works for creative pieces and for open problems (plans, ideas, advice). Stays out of the way when a task has one right answer. Replies in your language.

**Install:** `npx skills add ortizSimon/slop-radar -g -a claude-code`. For Claude on the web, download [`slop-radar.zip`](https://github.com/ortizSimon/slop-radar/raw/main/slop-radar.zip) from this repo and upload it under Customize → Skills. For ChatGPT or Gemini, paste [`pegar/short-en.md`](pegar/short-en.md) into custom instructions.

MIT license. Made by [Simón Ortiz](https://simonortiz-ai.vercel.app).
