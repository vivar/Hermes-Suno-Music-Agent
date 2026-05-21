---
name: ai-music-video-pipeline
description: Interactive end-to-end AI music video pipeline using Suno. Supports any music style and grows with the user. Includes comprehensive music production guidance for beginners.
tags: [suno, music, video, prompting, songwriting, production, mixing, arrangement, genres]
---

# AI Music Video Pipeline

## Purpose
A flexible, reusable skill for creating full AI music video packages with Suno. Designed to work with any music style or channel. Includes interactive setup and deep music production guidance so beginners can improve their songs beyond AI generation.

## How to Use
Load this skill when working on music video projects. It will first run a short setup to understand the current project context, then guide you through creation and production.

## Initial Setup Questions

When this skill is activated for the first time in a session, ask the following questions one at a time:

1. **Music Projects Root Folder**  
   Example: `/home/user/Projects/Music` or `~/Projects/Music`

2. **Music Channel / Project Name**  
   What is this music project or channel called? 

3. **Primary Music Style / Genre**  
   What is the main music style? (e.g. Country, Rockabilly, Modern Pop, Indie, Hip-Hop, K-Pop, etc.)

4. **Sub-genre or Vibe** (optional)  
   Any specific sub-genre, mood, or reference? (e.g. 90s country, dark synthwave, upbeat rockabilly)

5. **Full Package Creation**  
   Do you want to create the complete package? (lyrics.md + image.md + video.md + HTML song page)

After gathering this information, the skill should:
- Remember the context for the rest of the session
- Suggest next steps based on the answers

## Core Workflow

Once setup is complete, the skill should support these stages:

1. **Creative Ideation**
   - Generate song title ideas based on the channel/style
   - Help refine concepts and themes

2. **Songwriting & Suno Prompting**
   - Write lyrics with proper structure tags
   - Craft strong style prompts using best practices
   - Reference the `suno.md` guide when needed
   - Reference `references/suno-tags.md` for comprehensive Suno tag lists
   - Reference `references/songwriting.md` for expert-level songwriting techniques
   - Reference `references/parody-songwriting.md` when creating parodies

3. **Asset Generation**
   - Create the three markdown files:
     - `<songtitle>-lyrics.md`
     - `<songtitle>-image.md`
     - `<songtitle>-video.md`
   - Generate or assist with image and video prompts

4. **HTML Song Page**
   - Create a song page following the established template format

5. **Update Project Files**
   - Add the new song to the main index when appropriate

## Songwriting Guidance

This skill includes expert-level songwriting support. The goal is to move beyond generic AI-generated lyrics and into intentional, emotionally resonant songwriting.

### Available Songwriting References

The skill can reference the following songwriting guides:

- `references/songwriting.md` — Core principles, structure, lyric techniques, melody writing, genre-specific approaches, and working effectively with AI tools like Suno
- `references/parody-songwriting.md` — Specialized guide for writing parody songs: syllable matching, rhyme preservation, humor techniques, workflow, and working with AI tools for parody creation

### Songwriting Workflow

When helping with songwriting, the skill should:

1. **Establish the Emotional Core**
   - Help the user define what the song is really about (the feeling or story)
   - Suggest strong title ideas that capture the essence

2. **Guide Structure Decisions**
   - Recommend appropriate song forms based on genre and intent
   - Help decide between classic verse-chorus, modern short forms, or hybrid structures

3. **Lyric Development**
   - Apply “show, don’t tell” principles
   - Encourage specificity and vivid imagery
   - Help with rhyme schemes, prosody, and hook creation
   - Reference `references/songwriting.md` for advanced techniques

4. **Melody & Hook Focus**
   - Prioritize strong, memorable hooks
   - Suggest ways to create contrast between verse and chorus melodies

5. **Genre-Specific Songwriting**
   - Reference `references/genres.md` to understand the lyrical and structural conventions of the chosen style
   - Help the user blend songwriting approaches when creating hybrid genres

6. **AI Collaboration Strategy**
   - Treat Suno as a creative partner, not a replacement
   - Guide the user on how to write better prompts and how to edit/refine AI output
   - Emphasize human revision and personalization

### Songwriting Philosophy

The skill should always emphasize:
- Emotion and specificity create the strongest songs
- The hook is the most important element
- Contrast (verse vs chorus, energy, density) is a powerful tool
- Great songs are usually revised multiple times
- Human editing and intent almost always improve AI-generated material

## Image Prompt Generation Workflow

After lyrics and style prompt are complete, the skill should guide the user through image prompt creation:

1. Ask the user which image generation platform they want to use.
2. Present the options in clear categories:
   - **Local**: Qwen, Flux, SDXL
   - **Remote**: Nanobanna, Midjourney, SuperGrok
   - **Generic**: Universal prompting approach

3. Once the user selects a category and specific model, load the corresponding reference file from `references/`:
   - `qwen-image.md`
   - `flux-image.md`
   - `sdxl-image.md`
   - `nanobanna-image.md`
   - `midjourney-image.md`
   - `supergrok-image.md`
   - `generic-image.md`

4. Using the selected reference as guidance, generate a high-quality, model-appropriate image prompt based on the song’s theme, mood, and lyrics.

5. Save the final image prompt into `<songtitle>-image.md` in the project folder.

6. Offer to refine the prompt or generate variations before finalizing.

This workflow must remain flexible — the user can choose any model at any time, and the skill should adapt the prompting style accordingly.

## Music Video Guidance

This skill includes creative music video direction and prompting support. After the song and image concepts are complete, the skill can help develop strong video concepts and generate tool-specific prompts.

### Available Music Video References

The skill can reference the following video guides:

- `references/music-video.md` — Core creative principles, video styles, concept development, pacing, color/mood, and AI video workflow
- `references/ltx-video.md` — Local LTX video prompting, strengths, and best practices
- `references/wan-video.md` — Local WAN video prompting and motion control
- `references/supergrok-video.md` — xAI SuperGrok video guidance
- `references/veo3-video.md` — Google Veo 3 cinematic video prompting
- `references/klingai-video.md` — KlingAI character consistency and motion techniques
- `references/minimax-video.md` — Minimax stylized and artistic video approach
- `references/midjourney-video.md` — Midjourney video features and aesthetic motion

### Music Video Workflow

When helping with music video creation, the skill should:

1. **Develop the Creative Concept**
   - Extract emotional core and visual themes from the lyrics
   - Help choose the right video style (narrative, performance, abstract, hybrid, etc.)
   - Create a strong visual hook or recurring motif

2. **Guide Visual Storytelling**
   - Translate song emotion and lyrics into visuals
   - Suggest color palettes, lighting, and cinematography that match the mood
   - Consider pacing and editing synced to the music structure

3. **Tool Selection**
   - Ask which video generation platform the user wants to use
   - Present options: Local (LTX, WAN), Remote (Veo3, KlingAI, Supergrok, Minimax, Midjourney Video)

4. **Generate Tool-Specific Prompts**
   - Load the corresponding reference file for the chosen tool
   - Create detailed, platform-optimized video prompts
   - Maintain visual consistency with the song’s image concepts

5. **Save and Refine**
   - Save the final video prompts into `<songtitle>-video.md`
   - Offer to refine or generate variations

This workflow stays focused on creative execution.

## Music Production Guidance

This skill includes comprehensive production support for beginners. After generating a song with Suno, the skill can help improve it through arrangement, sound selection, mixing, and overall production decisions.

### Available Production References

The skill can reference the following production guides:

- `references/music-production.md` — High-level overview and philosophy
- `references/arrangement.md` — Song structure, energy mapping, and flow techniques
- `references/mixing.md` — Step-by-step mixing process, EQ, compression, and balance
- `references/reference-tracks.md` — How to choose and use reference tracks effectively
- `references/sound-design.md` — Sound selection, layering, and instrumentation
- `references/mastering.md` — Final mastering process and loudness guidelines
- `references/genres.md` — Comprehensive deep-dive into 13 major base genres (including K-Pop) with sub-genres, detailed instrumentation, rhythmic/harmonic traits, vocal approaches, arrangement structures, mixing priorities, production tips, AI/Suno prompting guidance, and classic reference tracks for each genre

### Production Workflow

When helping with production, the skill should:

1. **Analyze the Current Song**
   - Identify strengths and weaknesses in the AI-generated track
   - Suggest which areas need the most improvement (arrangement, instrumentation, mixing, etc.)

2. **Guide Arrangement Improvements**
   - Help restructure the song using proper sections and energy changes
   - Reference `references/arrangement.md`
   - Suggest where to add or remove elements

3. **Sound Selection & Instrumentation**
   - Recommend better sounds or layers to enhance the original idea
   - Reference `references/sound-design.md`
   - Help build a proper instrumental arrangement around the core hook

4. **Mixing Guidance**
   - Walk the user through a simplified mixing process
   - Reference `references/mixing.md`
   - Teach gain staging, EQ, compression, panning, and reference track usage

5. **Reference Track Strategy**
   - Encourage the user to pick 2–3 professional songs in the same style
   - Reference `references/reference-tracks.md`
   - Teach how to use them for arrangement, sound choices, and mixing decisions

6. **Genre-Specific Guidance**
   - Reference `references/genres.md` to understand the core characteristics of the chosen style
   - Help the user blend base genres when working with hybrid styles
   - Provide instrumentation and mixing priorities based on genre

7. **Mastering Guidance**
   - Provide light, corrective mastering advice when the mix is complete
   - Reference `references/mastering.md`
   - Focus on loudness, tonal balance, and translation

### Production Philosophy

The skill should always emphasize:
- Finishing tracks is more valuable than perfecting one
- Balance and intent matter more than expensive plugins
- Reference tracks are one of the most powerful tools for beginners
- Small, intentional changes often have the biggest impact
- A good mix needs very little mastering
- Understanding base genres helps when creating hybrid styles

## Reference File Rules (Critical)
- All files in `references/` must be kept **strictly style-agnostic** unless the user has chosen a specific genre.
- Never include genre-specific examples in general files.
- When creating or updating any reference file, always use neutral, reusable examples that work across any music style or channel.
- If the user corrects content for being too specific, immediately generalize the examples and best-practice notes.

## Notes for Future Expansion
- This skill should remain generic and not hardcoded to any specific channels.
- New styles, prompting techniques, and pipeline steps can be added over time.
- The skill can reference or load `suno.md` and `channel.md` from the active music folder when needed.
- Additional production or songwriting topics can be added as separate reference files.

## Current Status
- Suno prompting and image generation references: Complete
- Music production references: music-production.md, arrangement.md, mixing.md, reference-tracks.md, sound-design.md, mastering.md, genres.md (comprehensive deep-dive edition)
- Songwriting reference: songwriting.md (expert level) + parody-songwriting.md (specialized)
- Music Video reference: music-video.md (creative focus) + 7 tool-specific video references (LTX, WAN, Supergrok, Veo3, KlingAI, Minimax, Midjourney Video) — all created and registered in SKILL.md during video expansion pass
- Songwriting, production, music video, and song page workflow guidance fully integrated into skill

---

**Status**: Comprehensive music creation + production + expert songwriting + creative music video skill. Ready for further expansion, agent initialization, and practical use.

## Song Page & Interactive Workflow

This skill follows a strict 8-step interactive process for creating complete song packages and HTML pages.

### Core Principle: User-Controlled Pacing
The user must explicitly prompt before the agent advances to the next stage. Never generate multiple stages in one response. This prevents wasted tokens and respects the user's creative control.

### Reference
- `references/song-page.md` — Full workflow definition with pacing rules and YouTube metadata requirements

### Key Rules
- Never generate more than one stage without explicit user approval.
- Wait for the user to say “next”, “continue”, “ready for images”, etc.
- Each stage should be presented clearly and kept digestible.
- YouTube metadata (Step 8) must be output in easy-to-copy text boxes.
- Final HTML page generation only happens after the user explicitly requests it.

### Philosophy
This pacing prevents wasted tokens, allows real creative steering, and respects the user’s workflow preference for controlled, incremental progress.



## Agent Persona

This skill includes a dedicated agent persona defined in `Agent.md`. When activated, the agent should introduce itself and run the initial setup questionnaire before beginning creative work.


