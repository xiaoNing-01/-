---
name: airy-tea-editorial-image
description: >
  Generate original images for any subject while preserving a light, contemporary
  tea-inspired editorial language: warm off-white space, restrained botanical
  greens, a small bright accent, flat hand-drawn illustration, tactile paper grain,
  generous whitespace, asymmetric composition, and calm modern typography. Use when
  the user asks for image generation, posters, social cards, packaging, editorial
  illustrations, or a visual style similar to clean Chinese tea-brand design; keep
  the visual system but do not copy a reference image, logo, mascot, or proprietary artwork.
---

# Airy Tea Editorial Image

Translate any requested subject into an original image using the visual system in
[references/visual-style.md](references/visual-style.md). Treat the subject as the
variable layer and the visual system as the persistent layer: the topic, objects,
metaphors, and copy may change, while the palette logic, spatial rhythm, illustration
finish, and typographic temperament stay recognizable.

## Workflow

1. **Extract the brief.** Identify the subject, intended audience, use case, aspect
   ratio, required text, language, and emotional emphasis. If the user gives no
   format, choose a vertical 4:5 social/editorial canvas.
2. **Separate content from style.** Write a one-line content concept first. Then
   apply the style constraints from the reference file. Do not let a topic such as
   food, travel, technology, or finance force a different visual language.
3. **Choose one visual metaphor.** Prefer one memorable central metaphor and a small
   supporting detail over a literal collection of objects. Keep the illustration
   readable at thumbnail size.
4. **Design the layout before the prompt.** Place the main subject off-center, leave
   roughly 45–65% quiet breathing room, and reserve a clean text zone if copy is
   needed. Use a clear scale hierarchy: one hero element, one or two secondary
   elements, then tiny accents.
5. **Compose a generation prompt.** Put the requested subject first, followed by the
   persistent style system, layout, texture, and output constraints. Ask for an
   original illustration rather than naming a brand or saying “copy this image.”
6. **Handle text deliberately.** Image models often render Chinese characters poorly.
   If exact wording matters, request a blank, high-contrast text area and add the
   copy during layout/post-processing. If the generator supports reliable text,
   keep wording short and specify the hierarchy rather than filling the canvas.
7. **Generate and self-check.** Before returning an image, check that the subject is
   clear, the negative space is intentional, colors remain muted and coordinated,
   texture is tactile but not noisy, and no logo, trademarked character, or copied
   composition has appeared. If a check fails, regenerate with a targeted correction.

## Prompt construction

Build prompts with these blocks, in this order:

- **Subject:** the user's topic and the single chosen metaphor.
- **Medium:** contemporary editorial flat illustration, simplified organic shapes,
  hand-drawn contour, subtle screen-print/paper texture.
- **Palette:** warm off-white base, tea green as the dominant chromatic color,
  deep ink for linework, and at most one restrained accent.
- **Composition:** asymmetric but balanced, generous negative space, small number of
  elements, clear focal point, calm pacing, specified aspect ratio.
- **Typography:** modern rounded humanist sans-serif mood, sparse dark lettering,
  generous margins and tracking; reserve a text area when exact text is required.
- **Exclusions:** no photorealism, glossy 3D, dense background, neon gradients,
  generic stock-vector look, excessive shadows, brand logos, or direct recreation
  of any reference.

A useful prompt skeleton is:

> Original editorial illustration about **[subject]**, expressed through **[one
> metaphor]**. Contemporary flat hand-drawn illustration with simplified organic
> forms and subtle tactile paper grain. Warm off-white background, restrained tea
> green dominant, deep ink details, one small **[accent color]** accent. Asymmetric
> balanced composition, hero object placed **[left/right/lower area]**, generous
> quiet negative space for **[text/use]**, sparse supporting details, calm and
> friendly modern Chinese design mood, **[ratio]**. Typography area has a clean
> rounded humanist sans-serif temperament. Original arrangement and artwork, no
> logos, no copied characters, no imitation of a specific existing poster.

## Output contract

- If an image-generation capability is available, generate the image and provide a
  concise note naming the chosen metaphor and format.
- If it is unavailable, return a ready-to-use prompt plus a negative prompt and a
  compact layout specification; do not pretend an image was generated.
- For a series, keep the same palette ratios, line/texture treatment, whitespace
  discipline, and type mood across all images. Vary only the content metaphor,
  supporting objects, and accent placement.

## Safety and originality

Preserve abstract visual properties, not identifiable expression. Do not reproduce
an uploaded/reference image's exact subject arrangement, unique illustration,
character, logo, packaging, slogan, or distinctive lettering. When the user asks to
copy a particular image, explain that you can retain its high-level visual grammar
while creating a materially different composition and artwork.
