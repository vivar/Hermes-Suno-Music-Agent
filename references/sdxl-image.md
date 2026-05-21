# SDXL Image Generation Reference

This guide covers best practices for prompting SDXL (Stable Diffusion XL) models, whether running locally via ComfyUI, Automatic1111, or Forge, or through online platforms.

## Overview

SDXL is a powerful open-source image model that responds well to both detailed natural language prompts and traditional Stable Diffusion prompting styles. It excels at artistic control, style consistency, and high-quality outputs when given clear instructions.

## Prompt Structure Recommendations

SDXL works well with this general approach:

1. **Subject description** (detailed)
2. **Environment and setting**
3. **Pose / Action**
4. **Lighting and mood**
5. **Art style / aesthetic / artist references**
6. **Camera and composition**
7. **Quality boosters** (highly recommended)

## Example Prompt Format

```
A mysterious figure standing on a foggy mountain ridge at dawn, wearing a long dark coat, wind blowing through their hair, dramatic golden light breaking through the clouds, cinematic composition, highly detailed, atmospheric, 8k
```

## Best Practices

- SDXL responds well to both natural sentences and comma-separated keyword prompts
- Be specific about lighting, atmosphere, and mood
- Include art style references when you want a particular aesthetic (e.g., "in the style of [artist]")
- Use quality boosters at the end of the prompt for better results
- Consider using negative prompts to avoid unwanted elements (blurry, low quality, deformed, etc.)
- SDXL handles complex scenes and multiple subjects reasonably well
- Describe textures and materials relevant to the scene

## Quality Boosters

These commonly improve SDXL results:

- masterpiece
- best quality
- highly detailed
- intricate details
- sharp focus
- cinematic lighting
- atmospheric
- photorealistic
- 8k
- ultra-detailed

## Things SDXL Excels At

- Artistic styles and artist references
- Consistent aesthetic control
- Anime, illustration, and painterly styles
- Realistic photography when prompted properly
- Complex compositions and detailed scenes
- Good handling of text and symbols in images

## Things to Avoid

- Very short or vague prompts (SDXL benefits from detail)
- Overly conflicting style instructions
- Expecting perfect anatomy without additional guidance or models

## Advanced Tips

- SDXL works especially well when you combine subject description with style references
- Negative prompts are very effective with SDXL (e.g., "blurry, lowres, deformed, bad anatomy")
- You can use weighting syntax `(word:1.2)` if your interface supports it
- Many users combine SDXL with ControlNets or LoRAs for even more control

---

**Note**: This reference will be updated as new SDXL fine-tunes and prompting techniques are discovered.