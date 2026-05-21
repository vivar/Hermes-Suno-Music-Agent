# LTX Video Reference (Local)

## Overview
LTX is a local/open-source video generation model focused on high-quality, controllable motion with strong temporal consistency. It excels at turning static images or short clips into smooth video sequences, especially when run locally with good hardware (high VRAM recommended).

## Prompt Structure
- Start with a strong visual description of the scene and subject
- Add motion and camera movement instructions
- Specify duration, frame rate, and resolution where supported
- Include style and lighting cues
- Use clear, descriptive language rather than heavy keyword lists

**Example Prompt:**
"A mysterious figure walks slowly along a foggy mountain ridge at dawn. Camera slowly pans right while the figure moves forward. Soft golden light, cinematic atmosphere, gentle wind moving through tall grass. Smooth, realistic motion with natural breathing and footsteps."

## Best Practices
- Use high-quality starting images (from Flux, Qwen, or SDXL) for best results
- Keep initial motion simple and build complexity in follow-up generations
- Specify camera moves explicitly (slow pan, dolly zoom, tracking shot)
- Use "smooth motion", "natural physics", "consistent lighting" in prompts
- Generate short clips (4–8 seconds) and stitch in post if needed
- Run at 24–30fps for cinematic feel

## Strengths
- Excellent temporal consistency and reduced flickering
- Strong at realistic human/animal movement when given good input images
- Good control over camera movement
- Works well for atmospheric and moody scenes
- Local processing means no API costs or limits

## Things to Avoid
- Overly complex multi-character interactions in one shot
- Rapid camera movements or extreme angles without good starting frames
- Heavy text or logos (tends to distort)
- Very long generations (stability drops after ~10 seconds)

## Advanced Tips
- Combine with image-to-video workflow: generate keyframe with Flux/Qwen → feed to LTX
- Use negative prompts for "blurry, jittery, morphing, deformed hands, text"
- Experiment with motion strength / guidance scale parameters
- For music videos, generate multiple short clips that match lyric timing and edit together
- Pair with music-production references for pacing decisions

---

**Status**: Ready for use in ai-music-video-pipeline skill.