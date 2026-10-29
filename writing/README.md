# Overleaf, thesis template, and references

Use the [UCL PhD thesis LaTeX template](https://github.com/YuxuanTang2002/ucl-phd-thesis-template) for the literature review and final report source. It provides `main.tex`, chapter files, and a bibliography starter. Add or rename chapters to match your supervisor-approved report outline. The template describes itself as an unofficial UCL PhD thesis format created by a Chemistry PhD student; check that it suits your Master’s report requirements before using it.

## Add the template and connect Overleaf

1. Create your project repository from `masters_repo_template` and push it to GitHub.
2. Download the UCL template as a ZIP. Copy its `main.tex`, `bibliography.bib`, and the `appendices/`, `conclusions/`, `front/`, `introduction/`, `methodology/`, and `research/` folders into the root of your project repository. Keep this repository's README and project folders. Copy the UCL template's MIT licence to `writing/UCL_TEMPLATE_LICENSE` so the project's root `LICENSE` remains in place.
3. Commit and push the template files to your project repository.
4. In Overleaf, choose **New Project → Import from GitHub** and select your project repository. This imports the UCL template files and links Overleaf sync to your project repository. Set the compiler to **LuaLaTeX**.

Importing the UCL template repository itself creates an Overleaf project connected to that template repository. Import your combined project repository to keep the thesis source and research project together. GitHub synchronization is manual and requires an Overleaf premium feature; sign up with your UCL account for the group’s access. Sync from the Overleaf project menu, and sync before switching editors or editing the same file in both places. See Overleaf’s [GitHub synchronization guide](https://docs.overleaf.com/integrations-and-add-ons/git-integration-and-github-synchronization/github-synchronization) for current setup and limitations.

The template includes a UCL logo. Its README notes that use of the logo is subject to UCL branding guidance; check permission or remove the logo if needed.

## Connect Zotero

Zotero integration is also an Overleaf premium feature, which should be available with your UCL account. In Overleaf account settings, link your Zotero account under **Reference Managers**. In the Overleaf project, import your Zotero library or a Group Library as a `.bib` file, then refresh that file in Overleaf after changing references in Zotero. A project-specific Zotero Group Library helps keep the imported references focused. Alternatively, use Overleaf's advanced reference search to add individual references to the project's editable bibliography.

If Zotero integration is unavailable, export the relevant collection from Zotero as a BibTeX `.bib` file and add it to the Overleaf project and GitHub repository. Keep Zotero as the library of record and refresh the exported file when citations change. See Overleaf's [Zotero guide](https://docs.overleaf.com/integrations-and-add-ons/reference-manager-integrations/zotero) for the current steps and options.
