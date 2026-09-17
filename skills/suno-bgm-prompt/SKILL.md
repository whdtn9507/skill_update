---
name: suno-bgm-prompt
description: "Create copy-ready Suno prompts for original stream and short-video BGM when the user provides a topic, mood, duration, or production preferences."
---

# Suno Bgm Prompt

Create a concise, copy-ready prompt for Suno. This skill is for instrumental or vocal background music for livestreams, games, and short-form videos; it does not create prompts intended to imitate a named artist, song, franchise, or copyrighted character/image.

## Gather the brief

Use any conditions the user supplies. The preferred selectable fields are:

- purpose: stream opening, stream BGM, game/FC Online, YouTube video, short-form video, general listening, or other
- genre, mood, tempo, vocal type, duration, arrangement/progression, main instruments or sounds
- one-line topic and lyric language (none, Korean, English, or mixed)

If the user provides only a topic, mood, and duration, proceed without asking further questions. Infer the remaining production choices from the intended use. If they ask to choose conditions first, present the fields as numbered choices and combine their selections.

## Compose the prompt

Write the main prompt in natural English, under 1,000 characters. Lead with the overall style and mood, then specify genre, core instruments/sound design, tempo/energy, and the progression. Include the requested target duration naturally, such as “a focused 25-second cue” or “a seamless 2-minute background loop.”

Match the arrangement to the format:

- For 15–30 second shorts, use an immediate hook, one clear build or impact, and a clean ending; avoid long intros.
- For 30–60 second videos, give the cue a compact rise and resolution.
- For 1–3 minute streams or gameplay, prioritize a loop-friendly structure, stable focus, and transitions that do not distract from speech or play.
- For openings, allow a stronger identity and climax; for background use, avoid overly dominant lead melodies and sudden volume shifts unless requested.

Use original descriptive language. Do not reference named artists, specific songs, original-game soundtracks, fictional characters, logos, or visual IP as a sonic target. When a user names a game or content theme, translate it into general qualities such as competitive, energetic, playful, underdog, cinematic, or sporty.

For BGM, default to instrumental. Add vocals only when requested. If lyrics are requested, supply a separate short lyric section in the chosen language and avoid copyrighted phrases or franchise references.

## Response format

Return:

1. `Suno prompt` — one English prompt in a code block, with no headings inside it.
2. `Applied settings` — a compact Korean line listing purpose, duration, and the inferred or selected style.
3. `Lyrics` only when requested.

Keep the response practical and avoid multiple variants unless the user asks for options.
