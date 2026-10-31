# My Foodbook

My personal recipe collection, kept open source. Save recipes, find something to cook, and read or print them in the kitchen.

## Import recipes with AI

The [recipe-import skill](.agents/skills/recipe-import/SKILL.md) is the main way I add recipes. Give it a URL, recipe text, or a photo of a magazine or book page. It prepares an English, metric recipe with a local photo and source attribution, then opens a recipe-only pull request after confirmation.

> Use $recipe-import to add this recipe to My Foodbook: [recipe URL].

Use it with Codex or Claude Code and a write-capable GitHub connector. Eligible recipe PRs merge after validation; Cloudflare deploys changes to `main`. See the [setup guide](docs/recipe-import.md).

## The cookbook

Recipes are Markdown files in `recipes/`, with photos in `recipes/images/`. The Astro site includes search, cuisine filters, recipe suggestions, and a print layout.

- [Recipe format](docs/recipes.md)
- [Development and hosting](docs/development.md)
- [Design system](DESIGN.md)

This is my cookbook and its application. Third-party recipes and photos retain their own rights; attribution does not grant permission to redistribute them.
