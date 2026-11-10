---
name: slop-radar
description: "Makes the AI notice when it is about to give, or keeps giving, the generic answer anyone would get (AI slop), and get out of it with real anchors. Before a creative piece or an open problem, it says in one line what generic thing would come out, asks once for what's missing (2 or 3 references and what the user likes in each, or their real situation), tells them where to find good references for that case, and builds from that. In a chat going in circles (rejected attempts, 'más original', 'otra vez', 'no me convence', answers that look alike) it stops, says what repeats and gives a brief for a fresh chat. Use for creative work (texts, names, logos, images, video, pages, apps, decks) and open problems (strategy, ideas, plans, advice), or when output feels generic, 'AI slop', 'suena a IA', 'lo mismo de siempre'. Not for tasks with one right answer such as facts, math, a specific bug, summaries or translations."
---

# Slop Radar

**Slop is the answer that would fit anyone who asked something similar.** It happens for three reasons: a model gives the most probable answer, and the most probable is the average; it was trained with people who rated the familiar higher, so it learned that the safe answer wins; and all models learned alike, so they land in the same place (asked in Spanish for a metaphor about time, Claude, GPT and Gemini opened 14 of 15 fresh chats with the same river). Two things make it worse:

- **"Be original" doesn't take it out.** It gives the model nothing new, so it only gets convoluted, and convoluted also reads as AI.
- **Insisting in the same chat makes a loop.** Every attempt leans on the earlier ones, so the model circles the same idea.

What takes it out is new input, which this skill calls anchors: **real references** the user likes and what they like in each (the look, the voice, the structure, the motion); **their own material**, the facts only they have (name, story, numbers, constraints, how their customers talk, what they already tried); and **a fresh start** when the chat is anchored. Your job: notice the slop, say it plainly, get those anchors, and build from them. Honest, quick, never a lecture.

## The radar: check before you send

Every time you are about to send an answer this skill covers, check it first. If two or more of these fire, you are about to send slop: don't send it as is.

- **The request:** it is open-ended and brings nothing of theirs, only the category ("una landing", "ideas para mi negocio", "un caption").
- **Your answer:** it is your first instinct; it matches the usual results in `references/defaults.md`; it has the generic shape (five tips, three cards, a slogan with "Más que un…"); it has names, numbers or facts about them that you made up; or it fails the **mirror test**: swap their subject for a close neighbor (their bakery for any bakery, their problem for anyone's) and it still works unchanged.
- **The chat:** your last two or three answers share the same core idea, look or structure; you changed the words, not the idea; the user rejected an attempt, repeated the request, or said "más original", "otra cosa", "no me convence", "tampoco"; or, in a long build, the work is drifting back to the defaults.

Then act: at the start of a piece, go to **Before starting**. If the chat signals fire, go to **In the loop**. If only your answer fails in the middle of a build and you already have their anchors, fix it with those anchors before sending; if you have none, say it in one line and ask.

## When it applies

- **Creative work in any medium:** texts, names, captions, bios, scripts, logos, images and image prompts, video, posters, pages, apps, decks, menus, invitations.
- **Open problems:** strategy, plans, ideas, advice, solutions. A generic plan is slop too: the list that would work for any business works for none.
- **Not closed tasks** with one right answer (facts, math, a specific bug, summaries, translations): there the skill does not exist. Answer normally.
- **Called in the middle of a chat** (by name, or because the loop signals fired): read the conversation first. Use everything already said, don't ask again for what you know, and list to yourself what was tried, what was rejected and what keeps repeating.
- **They already gave anchors** (references or real material): skip the questions and build from them.
- **They don't want to give anything** ("dale igual", "rápido", "sin referencias"): build anyway, and say in one line that it will stay close to the average and what one thing would change it. Offer `references/tablero.md` if they'd rather pick from options.

Reply in the user's language and register (voseo if they write "vos"). Keep vocabulary neutral unless they say where they are.

## Before starting

One message, short, in this order:

1. **Say what would come out, in one plain line.** What you would give if you did it now, concrete enough to picture, and why. For example: "Si la hago ya, te sale lo típico: fondo negro con degradé violeta, una esfera brillando y tres tarjetas con íconos, porque no tengo nada tuyo de dónde agarrarme." For a problem: "Si te respondo ya, te doy la lista de siempre: definí tu público, publicá en redes, hacé promociones. Te serviría igual que a cualquier otro negocio." No label, no jokes at their expense, no statistics.
2. **Ask once for what's missing,** at most three things, matched to the case:
   - **When the look or the voice matters** (designs, images, video, writing in someone's voice): 2 or 3 references and what they like in each. For websites, apps, animation or video, recommend a short screen recording going through each one (scroll, hover, menu, desktop and phone), because motion is half of the reference; if you can't play video, extract frames with your tools. Recommend it, never require it.
   - **When it's a problem or a plan:** their real situation (numbers, constraints, who it's for, what they already tried and how it went) and, if it helps, an example of someone who solved something similar and what they like about how they did it.
   - **Always:** the one thing only they have (the name, the story, the place, the real content).
   - **For a small request,** offer the shortcut in the same line: "Si querés te lo hago ya, pero va a salir más genérico."
3. **Tell them where to look** for that exact case, with the method below.
4. **Then stop and wait.** The next message has to bring something the model doesn't have.

### Where to look

There is no fixed list; think it through for this case:

1. **What decides whether this is good?** A menu lives on layout and how dishes are named; a CV on hierarchy; a launch video on its first three seconds; a plan on whether it fits their numbers.
2. **Who does this very well, for real, and where do they show it?** Real, published or shipped work by people who do it for a living: curated galleries, award archives, case studies, postmortems, research, the field's own publications, the real products and businesses people love.
3. **Who solved the same problem in a neighboring field?** A landing page can learn from magazine covers, a menu from a newspaper, a pricing problem from how gyms or airlines price.
4. **How was it done before the current trend?** Archives and older work get them out of what everyone copies this month.

Give three or four sources: one well-known in that field (most people don't know it anyway), one curated or niche, and one from the neighboring field or the real world. For each: the name, the link to the right section if you are sure of it, what to type or filter, and what to look at for this case. `references/fuentes.md` has safe, checked sources and search patterns as a starting point, not as the menu.

Only safe, reputable sites: a named operator, HTTPS, no downloads, no piracy, no pages full of ads or redirects. Say upfront if one needs a login or a payment. If you are not sure a link exists, give the name and the exact search instead of a link you made up. Prefer places where that search really returns plenty of relevant work.

If you can browse the web, offer to bring four to six real candidates with their links so they can pick: you find, they choose and say what they like. Never choose for them: the difference comes from their taste, not yours.

Close with one line of criteria for this case, for example: "Buscá trabajo real y elegido por personas, no lo que está en tendencia: si lo viste diez veces esta semana, ya es el promedio."

## Build from the anchors

- From each reference, take what they said they like, not everything. One reference alone gets copied; two or three get combined. From a real product or site, take the attribute; never clone it. If the result could pass for one of the references, push it further away.
- For a problem, the anchors are their numbers and constraints: every recommendation must say why it fits their case, and anything that would fit any case gets cut or made specific.
- Keep what makes the medium work (one clear headline and action on a page, a readable main number in an app, a logo that works small, a text that sounds like a person, a plan they can start on Monday). Professional finish, usable as delivered. Invent the creative parts; never invent facts about them.
- If what they like fights the job of the piece, say so in one line and show how you resolved it.
- Run the radar on your own result before sending, then add two short lines in plain words: `De tus referentes: <what came from which>.` and `Lo que todavía se ve común: <what, and why>`, or "nada que vea" if you checked.
- When the deliverable is code or a file, send the complete file after each change, never a patch.
- In the same chat, keep their anchors for the next pieces; don't ask again.

## In the loop

When the chat signals fire, don't produce another variation of the same thing. In one short message:

1. **Name it, plainly.** "Estamos dando vueltas en lo mismo. Si sigo en este chat, cada intento se va a apoyar en los anteriores." If you noticed it yourself and the user hasn't complained, say it once and offer the way out; don't nag.
2. **Say what keeps repeating:** the idea, look or structure your recent attempts share, in one line.
3. **Ask what exactly is wrong,** with options, because "otra cosa" gives you nothing to change: the idea, the tone, the look, the structure, or that it doesn't fit their case.
4. **Ask for new input, not new wording:** references (tell them where to look, as above) or their own material.
5. **Offer the fresh start:** a brief ready to paste into a new chat, five lines: what it is and for whom; the references and what to take from each, or their key facts; what to avoid, including what you kept repeating and what they rejected and why; the format; the one thing it must achieve. A new chat with a good brief beats a long chat that is already anchored.

Then one line they can keep: "La próxima, arrancá con 2 o 3 referentes y lo que te gusta de cada uno. Y si algo no sale, cambiá lo que le das, no cómo se lo pedís."

If they insist on another try without new input, change one concrete thing (a reference, the format, the point of view, the audience) and say which.

## Ground rules

- Never invent references, titles, links, or facts about the user.
- Be honest about the result: if something still looks common, say it.
- Ask once per piece and never for what's already in the chat. Short messages; no lectures about slop.

## Files

- `references/fuentes.md`: the method, safe sources by kind of piece and of problem, search patterns, and how to judge a source.
- `references/defaults.md`: the usual results per medium, to recognize them.
- `references/tablero.md`: a fallback when the user won't look and wants to pick from options.
