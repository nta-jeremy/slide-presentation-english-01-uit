# Plan: Add Group 2 Member Slide (Option B)

## Context
- Static HTML slide deck at `index.html`
- 7 slides exist; JS auto-counts `.slide` elements
- Insert new slide **after slide 1** (`.full-bleed`) and **before slide 2** (`.content.split`)

## Expected Output
- New `<section class="slide">` with 7 member cards in a responsive flex grid (4 top + 3 bottom centered)
- CSS additions under existing `<style>` block

## Acceptance Criteria
1. Slide renders correctly in deck with consistent styling (gradient bg, rounded border, `.eyebrow` + `h2`)
2. 7 members displayed with MSSV (gold) + full name
3. Grid layout: 4 cards first row, 3 cards second row centered
4. No JS changes needed; slide navigation works automatically
5. No visual regression on existing slides

## Scope
- **In scope**: Add CSS + HTML slide only
- **Out of scope**: Photos, role highlights, animations, JS changes

## Implementation Steps
1. Add `.member-grid` and `.member-card` CSS inside `<style>` block (after `.mini` block)
2. Insert HTML slide after closing `</section>` of slide 1 (line ~453)

## Touchpoints
- `index.html` — add CSS + HTML only
