# Project Memory - Me, Myself & Claude Talk

## Project Overview
Quarto presentation (Reveal.js) for a 25-minute talk on AI-assisted R development. Title: "Me, Myself & Claude" - Category: AI-Assisted Development in R.

## Key Learning: Where AI Got It Wrong

### Initial Error: Misunderstanding the SHINYFA Package

**What Claude Code Did Wrong:**
- When asked to create presentation content about the `{shinyfa}` package, Claude **hallucinated the package's purpose entirely**
- Initial draft claimed shinyfa was for "Font Awesome icons in Shiny apps" with example code like `fa_icon("rocket", fill = "#0051BA")`
- This was completely fabricated - Claude made assumptions based on the package name without actually knowing what it did

**What the Package Actually Does:**
- `{shinyfa}` is a **file analysis tool** for large Shiny applications
- Analyzes Shiny app structure by extracting render functions, reactive functions, inputs, and file relationships
- Helps with developer onboarding to complex Shiny codebases
- Uses `analyze_shiny_reactivity()` function to catalog reactivity patterns

**How Jasmine Course-Corrected:**
1. Opened the generated .qmd file and noticed the Font Awesome references
2. Explicitly directed Claude to the actual package documentation: https://dalyanalytics.github.io/shinyfa/
3. Claude used WebFetch to read the real documentation
4. Claude then corrected ALL references to match the actual functionality

**The Meta-Lesson:**
This is a **perfect example** of the "Human in the Loop" principle from the talk itself:
- AI will confidently generate plausible-sounding content
- The human developer must verify accuracy, especially for domain-specific details
- Providing specific sources (URLs, documentation) helps AI self-correct
- This type of hallucination is exactly why you can't treat AI as "the boss" - you must maintain technical leadership

## Presentation Structure

### Four Main Parts (25 minutes)
1. **Strategic Thinking Unlocked** - Mental bandwidth shift (10-20% gained back)
2. **Saying Yes to Bigger Problems** - Scaling strategy, Cloudflare Workers example
3. **Building Intuition Through Volume** - Learning acceleration through iteration
4. **The Human in the Loop** - AI values, maintaining technical leadership

### Key Examples
- **SHINYFA Package**: Open source contribution for Shiny file analysis
- **Economic Development Dashboard**: Cloudflare Workers reverse proxy solution
- **Quarto Over JavaScript**: Staying in your lane example

## Technical Requirements
- Quarto with Reveal.js engine
- R code chunks for all examples
- Markdown-based (no over-abstraction)
- Maintainable, editable by human developer
- Emphasis on R functions and R ecosystem

## Philosophy Embedded in Code
- AI is a **colleague/intern**, not a boss
- Maintain "hand on the wheel"
- Code must be understandable 6 months from now
- Stay in your R lane while extending reach
- Human maintains technical leadership

## Files
- `me-myself-claude.qmd` - Main presentation file
- `CLAUDE.md` - This memory file for future sessions

---

**Final Quote:**
"When AI frees up your mental bandwidth, you don't get lazy—you get strategic."
