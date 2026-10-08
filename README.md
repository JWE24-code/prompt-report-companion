# Prompt Report Companion

An unofficial study companion to **The Prompt Report: A Systematic Survey of Prompt Engineering Techniques** (Schulhoff, Ilie, Balepur et al., arXiv:2406.06608, v6, 26 Feb 2025).

Two views in one static page:

- **Reference**: vocabulary, a searchable taxonomy of text-based prompting techniques, multilingual/multimodal, agents and RAG, evaluation, security, alignment, charts, the case study, and an appendix wordlist that explains the acronyms and general terms.
- **Lessons**: 12 lessons from basics to advanced, with takeaways, a check question, and progress saved in the browser.

## Publish on GitHub Pages

1. Create a new repository on GitHub (public, or private if your plan allows Pages).
2. Upload `index.html`, `.nojekyll` and `README.md` to the repository root.
   - On the web: **Add file → Upload files**, drag the files in, **Commit changes**.
   - Or with git:
     ```
     git init
     git add .
     git commit -m "Add Prompt Report Companion"
     git branch -M main
     git remote add origin https://github.com/<you>/<repo>.git
     git push -u origin main
     ```
3. In the repository, open **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose branch **main** and folder **/ (root)**, then **Save**.
4. After a minute the site is live at `https://<you>.github.io/<repo>/`.

No build step and no dependencies. Fonts load from Google Fonts and fall back to system fonts if blocked.

## Sources and attribution

All research content comes from the paper:

- Paper: https://arxiv.org/abs/2406.06608
- Dataset: https://huggingface.co/datasets/PromptSystematicReview/Prompt_Systematic_Review_Dataset
- Authors' companion guides: https://learnprompting.org

Technique descriptions are paraphrased. Attributions such as "Wei et al., 2022" are the citations the paper gives, and each technique card links to an arXiv title search for the original. Charts are redrawn from numbers reported in the paper. Teaching examples are original.

Cite the paper itself, not this site:

> Schulhoff, S., Ilie, M., Balepur, N., et al. (2025). The Prompt Report: A Systematic Survey of Prompt Engineering Techniques. arXiv:2406.06608v6 [cs.CL].

This site is not affiliated with the authors.

## Editing

Everything is in `index.html`. Technique data lives in the `TECH` array, the appendix wordlist in the `GLOSS` array, and lesson text in the `LESSONS` array inside the script.
