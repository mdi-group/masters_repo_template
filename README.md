# Master’s project template

Use this repository as the shared home for your project code, notes, and links to its data and results. Keep enough context that your supervisor or a future student can follow what you did.

## Set up your project

- [ ] On GitHub, choose **Use this template** and create a new repository with a short, descriptive name.
- [ ] Keep the project repository **private** while the work is in progress unless your supervisor agrees otherwise.
- [ ] Add your supervisor and collaborators with the appropriate access.
- [ ] Clone the new repository to your computer. If you are new to Git or GitHub, start with the [group Git and GitHub workshop](https://github.com/mdi-group/intro-to-git-workshop).
- [ ] Replace the project details below and update this README as the project changes.
- [ ] Make an initial commit and push it to GitHub. GitHub Desktop is fine if you prefer a graphical interface.

```text
Project title:
Student:
Supervisor:
Start date:
Repository URL:
Overleaf URL:
```

## Where things go

| Folder | Use it for |
| --- | --- |
| [`data/`](data/README.md) | Notes about raw and processed data, where it came from, and how to access it |
| [`scripts/`](scripts/README.md) | Reusable code for processing data, analysis, and figures |
| [`figures/`](figures/README.md) | Figures used in drafts and reports |
| [`models/`](models/README.md) | Model descriptions and checkpoint storage guidance |
| [`results/`](results/README.md) | Run notes and useful result summaries |
| [`writing/`](writing/README.md) | Overleaf and Zotero workflow; the group report template can be added here later |

## Keep the work traceable

- [ ] Record where data came from, its version or date, and any access or sharing conditions in the data folder README.
- [ ] Keep original data unchanged. Put local raw and processed files in their matching folders; these payloads are ignored by Git by default.
- [ ] Keep the script and settings that produced each important result. Record the Git commit, input data, command, and software versions in a short run note or configuration file.
- [ ] Use small, meaningful commits and push regularly.
- [ ] Before sharing, check that the repository contains no credentials, personal data, restricted material, or files whose licence does not allow sharing.

## Store larger files with GitHub Releases

For large, versioned datasets or model checkpoints that are approved for GitHub, attach the files as assets to a GitHub Release instead of committing them to the repository. Give each release a clear version and describe the asset, source/version, access conditions, and SHA-256 checksum in the release notes. Each release asset must be under 2 GiB. Release assets are separate from Git history: they are not included when someone clones the repository or syncs it with Overleaf, so provide download instructions in the relevant folder README. Release access follows repository access; use approved institutional storage for restricted data.

See GitHub’s [release documentation](https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases) for current limits and details.

## Write in Overleaf

- [ ] Push the initial project repository to GitHub.
- [ ] In Overleaf, create a **new project from GitHub** and select this project repository. The report template can be added when the group template is available.
- [ ] GitHub synchronization is manual and requires an Overleaf premium feature. Sync from the Overleaf project menu; sync before switching between editing in Overleaf and GitHub.
- [ ] Save the Overleaf project URL above. See [`writing/README.md`](writing/README.md) for the Zotero connection and reference-sync steps.

Overleaf GitHub sync attributes pushes to the connected GitHub account owner, and can bundle several edits into a single commit. Record contributions and important project decisions in the repository README or a brief project note. See Overleaf’s [GitHub synchronization guide](https://docs.overleaf.com/integrations-and-add-ons/git-integration-and-github-synchronization/github-synchronization) for current setup and limitations.

## Handy Git commands

Run these from the project folder:

```bash
git status
git add -A
git status
git commit -m "Describe the change"
git push
```

Review the second `git status` before committing. The ignored data and checkpoint payloads will not be staged. Do not force-add a file unless you have checked that it is allowed to be shared.
