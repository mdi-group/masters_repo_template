# Literature review and report

The report starts at [`../main.tex`](../main.tex). It imports the chapter files in `sections/`; begin with the literature review, then update the methods and results as the project develops. Use your department's required structure and formatting when it is available.

## Overleaf and GitHub

The simplest linked workflow is to push this repository to GitHub, then create a **new Overleaf project from that GitHub repository**. Overleaf GitHub sync is manual and requires a premium feature; the linked project is synchronized from its menu. It imports the whole repository, so keep data and model payloads out of Git, avoid Git LFS and submodules, and keep the repository small. Overleaf recommends less than 100 MB for a GitHub-synced project.

Overleaf cannot connect an existing Overleaf project to an existing GitHub repository through GitHub sync. For an existing Overleaf project, consult Overleaf's [Git integration guide](https://docs.overleaf.com/integrations-and-add-ons/git-integration-and-github-synchronization/git-integration) for the separate Git-remote workflow. The [GitHub synchronization guide](https://docs.overleaf.com/integrations-and-add-ons/git-integration-and-github-synchronization/github-synchronization) describes setup, manual sync, authorship, size limits, and other current limitations.

Save the Overleaf project URL in the project details at the top of the root README. Sync before changing editors, and review changes on GitHub. Overleaf pushes are attributed to the connected GitHub account owner, so keep [AUTHORS.md](../AUTHORS.md) and [the project log](../docs/PROJECT_LOG.md) up to date.

## Literature review practice

- Record the search date, search terms, inclusion/exclusion reason, and citation details in [`reading_log.csv`](reading_log.csv).
- Add complete citation metadata to [`references.bib`](references.bib) and cite claims close to where they appear.
- Compare and synthesize sources by question, method, evidence, and limitations; avoid writing one isolated summary paragraph per paper.
- Make clear which statements are established findings, disagreements in the literature, or your interpretation.

## Figures and references

The report can include a tracked figure using `\includegraphics{figures/<filename>}`. Record the figure's inputs and generating script in [`../figures/figure_register.csv`](../figures/figure_register.csv). Keep figure files small enough for the chosen GitHub/Overleaf workflow.

Add references in BibTeX format to `references.bib`. Cite with `\citep{key}` for parenthetical citations or `\citet{key}` for author-in-text citations. Replace the example chapter prompts with the required thesis format before final submission.
