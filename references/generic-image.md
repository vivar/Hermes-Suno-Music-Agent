# Generic Image Generation Reference

This guide provides universal best practices for prompting AI image generators. Use this when you want a flexible, model-agnostic approach that works reasonably well across most systems (local or remote).

## Overview

A good generic prompt focuses on clarity, structure, and descriptive language. While each model has its preferences, the principles below produce solid results on a wide range of image generators.

## Recommended Prompt Structure

Use this general order for most models:

1. **Main Subject** — Who or what is the focus
2. **Environment / Setting** — Where the scene takes place
3. **Action / Pose** — What the subject is doing
4. **Lighting & Atmosphere** — Time of day, mood, light quality
5. **Art Style / Aesthetic** — Realistic, cinematic, painterly, etc.
6. **Camera / Composition** — Angle, shot type, framing
7. **Quality Boosters** — Detail and technical enhancers

## Example Prompt Format

```
A mysterious figure standing on a foggy mountain ridge at dawn, wearing a long dark coat, wind blowing through their hair, dramatic golden light breaking through the clouds, cinematic composition, highly detailed, atmospheric, 8k
```

## Best Practices

- Be specific and descriptive rather than vague
- Use natural language or clear comma-separated phrases
- Mention lighting and atmosphere — this dramatically improves most models
- Include textures, materials, and environmental details
- Specify camera angles when composition matters
- Add quality boosters at the end
- Keep the prompt focused — too many conflicting ideas can confuse the model

## Quality Boosters

These work well across most image generators:

- highly detailed
- intricate details
- sharp focus
- cinematic lighting
- atmospheric
- photorealistic
- masterpiece
- 8k
- ultra detailed

## Universal Strengths

Most modern image models perform well when you provide:
- Clear subject + environment
- Specific lighting references
- Texture and material details
- Composition guidance

## Common Pitfalls to Avoid

- Overly short or generic prompts ("a man in a forest")
- Too many conflicting styles in one prompt
- Vague emotional terms without visual translation
- Ignoring lighting and atmosphere

## Adaptation Tips

- For models that prefer natural language (Flux, Grok): Write in full sentences
- For models that like keywords (SDXL, Midjourney): Use comma-separated style
- When moving between platforms, start with a solid base prompt and adjust length/detail as needed
- Always test a few variations when switching models

---

**Note**: This generic reference serves as a solid foundation. For best results, combine it with the specific recommendations from the model you are using.