# Song Page Generation Workflow

This reference defines the structured, interactive process for creating a complete song package and final HTML song page. The workflow is deliberately broken into clear stages so the user can review, adjust, and approve each part before moving forward.

## Core Principle

**The user must explicitly prompt when they are ready to move to the next step.**  
Never generate the entire package at once. Generate one stage, present the output, then wait for the user to say “next”, “continue”, “ready for images”, etc. This prevents wasted tokens and allows the user to steer the creative direction at every stage.

## The 8-Step Workflow

Follow this order for every new song:

### 1. Title Generation / Suggestions
- Generate 8–10 strong song title ideas based on the channel and style.
- Keep titles concise, evocative, and searchable.
- Present them in a clean numbered list and wait for user selection or refinement.

### 2. Genre / Feel / Style Definition
- Confirm or refine the genre, sub-genre, mood, and overall sonic feel.
- Ask clarifying questions if needed (energy level, era influence, hybrid elements).
- Lock this in before moving to lyrics.

### 3. Lyrics and Suno Prompt Generation
- Write full lyrics with proper structure tags ([Verse], [Chorus], etc.).
- Create a strong, detailed Suno style prompt.
- Present both the lyrics and the style prompt together.
- Wait for user feedback before proceeding.

### 4. Vision of How the Song Should Feel in the Video
- Develop the overall creative direction and emotional tone for the music video.
- Define the visual style (narrative, performance, abstract, hybrid, etc.).
- Establish recurring motifs, color palette, and pacing feel.
- Get user approval on the high-level vision.

### 5. Image Breakdown
- Ask the user for timing details (example: Instrumental 0:00–0:10 = 1 image).
- Break the song into logical visual segments with timestamps.
- Suggest number of images and rough duration for each section.
- Confirm the breakdown with the user before generating prompts.

### 6. Image Prompt Generation
- Ask which image generation tool the user wants to use.
- Generate detailed, tool-optimized image prompts for each segment in the breakdown.
- Include style consistency notes so all images feel cohesive.
- Present prompts one section at a time or in small batches if requested.
- Wait for user approval or edits before moving to video.

### 7. Video Prompt Generation
- Ask which video generation tool the user wants to use.
- Convert the approved image prompts into image-to-video or text-to-video prompts.
- Include camera movement, pacing, and motion direction tailored to the chosen tool.
- Maintain visual consistency with the image concepts.
- Present video prompts and wait for user feedback.

### 8. YouTube Metadata Generation
- Generate the following (each in its own clearly labeled copy-friendly box):

  **YouTube Title**  
  (SEO-optimized, under 70 characters when possible)

  **YouTube Description**  
  (Engaging, includes relevant context, calls to action, and timestamps if applicable)

  **YouTube Keywords**  
  (Comma-delimited list, maximum 400 characters including spaces and commas)

- Present all three in easy-to-copy format.
- This metadata is intended to be passed to the user’s separate YouTube posting agent.

## HTML Song Page Creation

Once all eight steps are complete and approved, the skill can generate the final `<songtitle>.html` page using the established template format. This should only be done after the user explicitly requests it.

The HTML page should incorporate:
- Song title and player/embed
- Lyrics section
- Visual concept notes (optional)
- Any approved imagery or video links (when available)

## Rules

- Always wait for explicit user confirmation before advancing to the next step.
- Never auto-generate the full package in one response.
- Keep each stage focused and digestible.
- Allow the user to go back and revise earlier steps at any time.
- All prompts and outputs must stay consistent with the chosen genre and video vision.

---

**Status**: Workflow defined. Ready to be integrated into the main ai-music-video-pipeline skill.