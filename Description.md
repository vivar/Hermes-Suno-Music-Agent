# AI Music Video Pipeline Agent

## What This Is

The **AI Music Video Pipeline Agent** is a comprehensive, self-contained creative assistant for building full AI-generated music video projects. It guides users through a structured, high-quality workflow from initial concept to final deliverables.

It combines songwriting support, Suno prompting, image generation, video direction, and production guidance into one cohesive system. The agent is designed to be generic, portable, and reusable across any music style or channel.

## Key Features

- Interactive 8-step workflow with strict user-controlled pacing
- Full song package generation (lyrics, image prompts, video prompts, YouTube metadata)
- Comprehensive references for Suno, image tools, video tools, songwriting, and music production
- Generic setup that works for any music creator
- Clean separation between creative work and technical prompting

## How to Add This to Hermes

1. Copy the entire `ai-music-video-pipeline` folder into your Hermes skills directory:
   ```
   ~/.hermes/skills/ai-music-video-pipeline/
   ```

2. The skill should contain the following structure:
   - `SKILL.md`
   - `Agent.md`
   - `Description.md`
   - `references/` folder (containing all supporting markdown files)

3. Restart Hermes or reload the skills so the new agent becomes available.

## How to Initialize the Agent

When you first activate the agent in a new conversation or after a system reset, it will automatically begin the setup process:

1. The agent introduces itself.
2. It asks a short series of questions one at a time:
   - Music projects root folder
   - Channel or project name
   - Primary music style/genre
   - Any specific mood or vibe (optional)
   - Whether to create the initial project structure

3. Once setup is complete, the agent switches into normal operating mode and follows the 8-step creative workflow.

You can also manually load the agent by referencing it in your prompt or through your Hermes configuration.

## Workflow Overview

The agent follows a deliberate 8-step process:

1. Title Generation
2. Genre / Feel / Style Definition
3. Lyrics and Suno Prompt Generation
4. Video Vision and Creative Direction
5. Image Breakdown (with timing)
6. Image Prompt Generation
7. Video Prompt Generation
8. YouTube Metadata (Title, Description, Keywords)

At every stage, the agent waits for explicit user confirmation before moving forward. Nothing is generated in bulk.

## Philosophy

This agent prioritizes quality and user control over speed. It is built for creators who want intentional, well-crafted results rather than rapid mass generation.

---

**Version**: 1.0  
**Status**: Ready for use and sharing.