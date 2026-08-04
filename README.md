# Create Seedream Product Posters

Turn one casual product photo into a planned, polished Chinese or English commercial poster with Seedream 5.0 Pro.

This TRAE Skill is designed for product-poster workflows such as e-commerce hero images, promotional long posters, new product launch visuals, English campaign posters, and product-photo-to-poster tasks. It helps the agent plan the theme, define the copy hierarchy, choose a commercial visual direction, build a Seedream prompt, and run visual QA before accepting the final poster.

## Skill Description

`create-seedream-product-posters` transforms a product snapshot into a complete commercial poster concept and generation workflow.

It is useful when the user asks for:

- 策划商品海报
- 商品图生海报
- 电商主图
- 促销长图
- 新品发布图
- 英文海报
- English product poster
- Campaign poster
- A polished commercial poster from a phone product photo

The skill treats the product photo as the source of truth. It should not silently replace the product, change the product category, or substitute another generation model when the request specifically requires Seedream 5.0 Pro.

## Install

Use the standalone `SKILL.md` file if your agent supports installing skills from a raw skill definition:

```text
https://raw.githubusercontent.com/Lucc222/create-seedream-product-posters/main/SKILL.md
```

Use the complete skill package if your agent needs the references, scripts, and agent configuration files:

```text
https://github.com/Lucc222/create-seedream-product-posters/raw/main/create-seedream-product-posters-v18.zip
```

Repository homepage:

```text
https://github.com/Lucc222/create-seedream-product-posters
```

## How To Use

1. Provide at least one product photo.
2. Ask for a product poster, e-commerce main image, promotional poster, launch poster, English product poster, or campaign poster.
3. The skill analyzes the product and campaign intent.
4. The skill chooses a commercial visual direction from the reference system.
5. The skill plans the copy hierarchy, layout, background, lighting, and product placement.
6. The skill writes a Seedream 5.0 Pro prompt.
7. The skill checks the generated result against the QA rubric and suggests revisions if needed.

## Example Prompts

```text
帮我把这张商品图做成一张高级感电商海报。
```

```text
用这张产品照片，做一张新品发布海报，中文文案。
```

```text
Create an English campaign poster from this product photo.
```

```text
帮我策划一张促销长图，要有主标题、副标题、卖点和购买氛围。
```

## Inputs

- Required: one product image.
- Optional: product name, selling points, target audience, language, campaign theme, dimensions, brand tone, price, discount, platform, and preferred visual style.

If the user does not provide a complete brief, the skill should infer a reasonable commercial direction from the product category and image signals.

## Outputs

- Poster theme and campaign concept.
- Visual style direction.
- Chinese or English commercial copy.
- Layout and composition plan.
- Seedream 5.0 Pro generation prompt.
- Visual QA checklist.
- Revision suggestions when the result is weak, generic, inaccurate, or not commercially complete.

## Reference Files

The complete workflow depends on these reference documents:

- [reference-grammar.md](references/reference-grammar.md): Extracts reference composition, density, rhythm, visual richness, and commercial poster grammar.
- [style-atlas.md](references/style-atlas.md): Helps choose the visual family and map product categories to suitable poster styles.
- [style-recipes-18.md](references/style-recipes-18.md): Provides eighteen concrete commercial art directions that can be safely adapted.
- [layout-system.md](references/layout-system.md): Defines grid, copy hierarchy, product placement, visual flow, and poster structure.
- [prompting-and-api.md](references/prompting-and-api.md): Guides Seedream 5.0 Pro prompting and generation behavior.
- [qa-rubric.md](references/qa-rubric.md): Defines quality gates before accepting the final poster.
- [commercial-completeness.md](references/commercial-completeness.md): Checks whether the output feels like a complete commercial poster rather than a catalog still.
- [universal-router.md](references/universal-router.md): Routes ambiguous products or campaign requests to the right visual strategy.
- [reference-corpus.md](references/reference-corpus.md): Provides reference patterns and examples for campaign planning.
- [benchmark-regression.md](references/benchmark-regression.md): Tracks benchmark behavior and regression risks.
- [execution-patterns.md](references/execution-patterns.md): Describes robust execution patterns for planning, generation, and revision.

## Included Package

The repository also includes:

- `SKILL.md`: standalone skill definition.
- `create-seedream-product-posters-v18.zip`: complete packaged skill archive.
- `references/`: supporting knowledge files for style, layout, prompting, QA, and execution.

## Notes

- Use the raw `SKILL.md` link for simple skill installation.
- Use the zip package when the agent needs all supporting references and scripts.
- Use the GitHub repository page when sharing the project with people.
