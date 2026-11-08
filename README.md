# AI Critical Thinking Wiki

A curated wiki distilling:

> Pearson H. (2026). "How to stay smart in the age of AI: the science of critical thinking." *Nature* 657, 873–875 (issue 8133), 23 September 2026. doi: [10.1038/d41586-026-02930-6](https://doi.org/10.1038/d41586-026-02930-6).

**Note:** The Nature article is subscription-gated; this wiki distills the freely available material — the lede, the opening paragraph, the nine cited studies, and the related-coverage list.

**Public copy:** https://iamflipse.github.io/ai-critical-thinking-wiki/ (read-only; static build served from the `gh-pages` branch)

## Layout

- `src/` — wiki pages as markdown (`index.md`, `about.md`, `concepts/`, `sources/`)
- `book/` — mdbook-generated static site (committed for GitHub Pages)
- `tools/mdbook` — mdbook v0.4.21 binary (aarch64 Linux, built from source)

## Rebuild + republish

```sh
./tools/mdbook build -d book
git add -A && git commit -m "update" && git push origin main
# republish gh-pages: check out orphan branch, copy book/* to root, add .nojekyll, force push
```
