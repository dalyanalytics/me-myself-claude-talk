# Adding Images to Your Presentation

## Quick Start

Place your images in this `images/` directory, then reference them in your `.qmd` file.

## Image Syntax Options

### Basic Image
```markdown
![Alt text](images/your-image.png)
```

### Image with Size Control
```markdown
![Alt text](images/your-image.png){width=50%}
```

### Centered Image
```markdown
::: {.center}
![Alt text](images/your-image.png){width=60%}
:::
```

### Image with Caption
```markdown
![This is my caption text](images/your-image.png){width=70%}
```

### Side-by-Side Images
```markdown
::: {.columns}
::: {.column width="50%"}
![Left image](images/image1.png)
:::
::: {.column width="50%"}
![Right image](images/image2.png)
:::
:::
```

### Image as Background (full slide)
Add this to your slide header:
```markdown
## My Slide Title {background-image="images/background.jpg" background-size="cover"}
```

### Image with Link
```markdown
[![Alt text](images/your-image.png)](https://your-link.com)
```

## Example Slide with Image

```markdown
---

## The SHINYFA Package

::: {.columns}
::: {.column width="50%"}
**What it does:**
- Analyzes Shiny app structure
- Catalogs reactive functions
- Helps with onboarding
:::

::: {.column width="50%"}
![SHINYFA in action](images/shinyfa-demo.png){width=100%}
:::
:::

---
```

## Tips

1. **Use web-friendly formats**: PNG, JPG, SVG
2. **Optimize file sizes**: Keep images under 500KB when possible
3. **Alt text matters**: Always provide descriptive alt text
4. **Relative paths**: Images are relative to the `.qmd` file location
5. **Test locally**: Run `quarto preview me-myself-claude.qmd` to test
