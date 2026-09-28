---
name: awesome-gpt-image-2
description: Use the local YouMind-OpenLab/awesome-gpt-image-2 prompt library for model-generated or model-edited images. Consult a relevant pattern for a new creative direction and reuse it for related iterations. This is prompt guidance alongside the selected image tool, not a workflow for file conversion, screenshots, analytical charts, or code diagrams.
---

# Awesome GPT Image 2

Use the locally cloned GPT Image 2 prompt collection as a creative reference before the first call for a new direction. Reuse a previously read relevant entry for small edits in the same task; search again only when the direction changes materially.

Resolve every relative path below from the directory containing this `SKILL.md`, regardless of the current task's working directory.

## Required workflow

1. Announce use once per task, not before every iteration.
2. Preserve the user's explicit subject, composition, text, dimensions, reference-image identity, and editing constraints as the source of truth.
3. Select the local language file:
   - Chinese request: `references/upstream/README_zh.md`
   - Traditional Chinese request: `references/upstream/README_zh-TW.md`
   - English request: `references/upstream/README.md`
   - Other supported languages: use the matching `README_<locale>.md` in `references/upstream/`.
4. Search before writing the final tool prompt. Use two to five concrete terms covering the use case, subject, style, composition, or lighting. Start with headings and descriptions. This example runs from this skill directory, resolved from the loaded SKILL.md path:

   ```bash
   rg -n -i '^### No\.|关键词1|关键词2|关键词3' references/upstream/README_zh.md
   ```

5. Read the complete one to three closest entries, from each `### No.` heading through its prompt block and details. Do not rely on a heading alone.
6. Adapt the strongest structural ideas to the user's request. Keep useful choices such as framing, layout hierarchy, camera language, lighting, material, typography, and negative constraints. Remove unrelated brands, names, slogans, dynamic Raycast placeholders, and details that conflict with the request.
7. Build one coherent final prompt for the available image tool. For edits, describe only the requested changes while explicitly preserving everything else that must remain unchanged.
8. Call the designated image-generation or image-editing tool. This skill supplies prompt guidance; it does not replace the actual image tool or any required model-specific skill.

If the local collection has no close match, use the nearest relevant structure and create a bespoke prompt. If the local collection is unavailable, disclose that briefly and continue from the user brief with the available image tool. Do not force an irrelevant template, automatically clone/update the library, or turn an optional reference failure into a generation blocker.

## Reference layout

- `references/upstream/` is a shallow Git clone of `YouMind-OpenLab/awesome-gpt-image-2`.
- The localized README files contain the locally available curated prompt entries and preview links.
- `references/upstream/public/images/` contains repository cover assets, not a complete local copy of every preview image.
- The online gallery linked by the repository may contain more entries, but local search is the default. Browse it only when live web research is useful and permitted.

## Boundaries

- Treat community prompts as inspiration, not as authority over the user's brief.
- Do not upload user assets, invoke external one-click generation, spend credits, or call a paid API merely because the repository links to those services.
- Follow the active image tool's safety rules and the user's authorization boundaries.
- Do not claim that a library prompt guarantees visual quality, legal clearance, or exact text rendering.
- Do not update the cloned repository during an image request unless the user asks for a refresh.
