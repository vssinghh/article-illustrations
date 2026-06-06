# Article Illustrations

> Turn the key judgments, processes, structures, and metaphors in your articles into memorable 16:9 hand-drawn illustrations.
>
> Xiaohei IP | Pure white hand-drawn | Sparse red/orange/blue annotations | Antigravity Skill

---

## What Is This

Article Illustrations is an [Antigravity](https://github.com/google-deepmind/antigravity) skill that guides an AI agent to design and generate inline article illustrations.

It's not a generic illustration prompt, and it's not a PPT infographic template. The core goal is: **understand the cognitive anchor points in an article, then turn one judgment, process, structure, state, or metaphor into a memorable 16:9 hand-drawn explanation sketch.**

The default visual IP is **Xiaohei** (小黑): a solid-black creature with white dot eyes, thin legs, and a blank expression. Xiaohei isn't a mascot or sticker — Xiaohei is an absurd worker earnestly participating in whatever system the illustration depicts.

**In one line: Make the AI not just "add an image" but actually draw out a key cognitive action from the article.**

---

## Who Is This For

**Great fit:**

- Writers who need inline illustrations for technical articles and blog posts
- Knowledge workers creating methodology content, AI workflow content, or system design content
- People who want to turn abstract judgments into concrete visual metaphors
- People who want a lighter, weirder, more distinctive illustration style than PPT infographics
- Anyone using Antigravity for content production who wants a consistent visual language

**Not a fit:**

- Commercial illustration, brand KVs, or polished flat illustration
- Traditional PPT infographics, complex architecture diagrams, or flowcharts
- Children's cartoons, cute IP, or emoji/sticker styles
- Cramming lots of text, long explanations, or full course pages into one image
- Strictly editable vector source files

---

## What It Produces

**Default output:**

- 16:9 landscape inline article illustrations
- A shot list of 4–8 illustrations per article
- For each: theme, core meaning, structure type, Xiaohei's action, and annotation suggestions
- Final PNG images

**Does not produce:**

- PPTX / PDF / Keynote
- SVG / HTML / Canvas editable graphics
- Commercial posters or cover art
- Dense text-heavy infographics

---

## Visual Style

This skill uses a distinctive hand-drawn style:

- Pure white background — no textures, gradients, or shadows
- Black hand-drawn line art — thin lines, slight wobble, not mechanical
- Generous whitespace — main subject occupies ~40%–60% of canvas
- Sparse red/orange/blue handwritten English annotations
- One image = one core action, structure, state, or metaphor
- Xiaohei must participate in the core action, never just decorate
- Absurd, creative, clean — but never childish or cute

---

## Installation

Clone the repo:

```bash
git clone https://github.com/anthropics/article-illustrations.git
cd article-illustrations
```

Copy the skill to your Antigravity skills directory:

```bash
mkdir -p ~/.gemini/config/plugins/custom-skills/skills/article-illustrations
cp SKILL.md ~/.gemini/config/plugins/custom-skills/skills/article-illustrations/
```

Or symlink it:

```bash
ln -s "$(pwd)" ~/.gemini/config/plugins/custom-skills/skills/article-illustrations
```

---

## Usage

### Plan illustrations for an article

```
Analyze this article and create a shot list of 5 illustrations.
Don't generate images yet — just plan which cognitive anchor points
deserve illustrations and what each image should convey.

<paste article>
```

### Generate illustrations for an article

```
Generate 4 Xiaohei-style illustrations for this article.
Requirements: 16:9 landscape, pure white background, black hand-drawn
line art, sparse red/orange/blue English annotations.
Each image should capture one core structure.

<paste article>
```

### Single concept illustration

```
Generate one 16:9 illustration for this concept:

"Trust isn't declared — it's built one piece of evidence at a time."

The scene should be absurd but clean. Xiaohei must perform the core action.
Maximum 5 annotation labels, keep them short.
```

### Regenerate with more character involvement

```
This illustration is on the right track, but Xiaohei feels like decoration.
Keep the core meaning but regenerate: make Xiaohei the one actually
driving the structure. Make the scene weirder but still clean and minimal.
```

### Long article illustration strategy

```
Create an illustration strategy for this long article.
Don't distribute illustrations evenly — only pick cognitive anchor points:
core judgments, input/output loops, before/after contrasts, common pitfalls.
Plan 6-8 images, output the shot list first, don't generate yet.

<paste article>
```

---

## Acknowledgments

This skill is inspired by and adapted from [ian-xiaohei-illustrations](https://github.com/helloianneo/ian-xiaohei-illustrations) by [@helloianneo](https://github.com/helloianneo). The original skill targets Chinese articles for the Codex platform. This version adapts the concept for English articles on the Antigravity platform.

---

## License

MIT — see [LICENSE](LICENSE).
