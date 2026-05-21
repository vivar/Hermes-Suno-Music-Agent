# WAN Video Reference (Local)

## Overview
WAN (often referring to models like Wan 2.1 or similar local video diffusion models) is a powerful open-source video generation tool optimized for local hardware. It offers strong motion coherence, good prompt adherence, and is particularly effective for stylized or artistic video clips.

## Prompt Structure
- Lead with subject and environment
- Describe desired motion and camera behavior
- Add artistic or cinematic qualifiers
- Keep prompts focused and descriptive

**Example Prompt:**
"Neon-lit cyberpunk street at night. A lone character runs through rain-slicked alleys while holographic ads flicker overhead. Camera tracks alongside the runner with subtle handheld shake. Vibrant blues and purples, moody atmosphere, cinematic lighting."

## Best Practices
- Start from strong, detailed images for image-to-video mode
- Use motion descriptors like "slow motion", "dynamic tracking shot", "gentle floating camera"
- Specify lighting changes or particle effects (rain, sparks, fog)
- Generate 5–10 second clips for easier editing
- Maintain consistent character appearance across clips by reusing seed images

## Strengths
- Good balance of realism and artistic control
- Strong at environmental effects (weather, lighting shifts)
- Solid prompt following for scene changes
- Local execution with reasonable VRAM requirements compared to some alternatives

## Things to Avoid
- Extremely fast cuts or chaotic multi-subject scenes
- Overloading with too many simultaneous actions
- Tiny text or fine details that can break during motion

## Advanced Tips
- Use as a "motion brush" tool — generate base motion then refine in another pass
- Combine with sound design references for syncing movement to music beats
- For music videos: generate abstract visualizers or performance shots separately and composite
- Experiment with different model checkpoints for stylized vs realistic output
- Pair with arrangement.md timing notes when planning clip lengths

---

**Status**: Ready for use in ai-music-video-pipeline skill.