# Master’s project template

Welcome. This repository is the working record for a research project: it should help someone else understand what you did, where the inputs came from, and how you produced the results in your report.

Use this checklist as you set up and work on the project. You do not need to fill every folder: if a section does not apply, note that in the relevant README or project log.

## 1. Create your project repository

- [ ] On GitHub, open this repository and choose **Use this template**.
- [ ] Create a new repository with a short, descriptive name. Keep it **private** while the project is in progress unless your supervisor has agreed otherwise.
- [ ] Add your supervisor and any project collaborators with the appropriate access.
- [ ] Clone your new repository to your computer and open this README in your editor.
- [ ] Replace the project details below and in [AUTHORS.md](AUTHORS.md).
- [ ] Make an initial commit, then push it to your GitHub repository.

```text
Project title:
Student:
Supervisor:
Start date:
Repository URL:
Overleaf URL:
```

## 2. Learn the project folders

| Folder | Put here | Keep in mind |
| --- | --- | --- |
| `data/` | Data manifests and instructions for accessing raw and processed data | Data payloads are ignored by Git by default. Record their source and checksum; use approved storage for the files. |
| `scripts/` | Small, reusable scripts that process data, run analyses, or create figures | Give each script a clear purpose and document how to run it. |
| `figures/` | Figures used in drafts or the final report, plus a figure register | Keep the script and input data needed to regenerate each important figure. |
| `models/` | Model cards and a register of trained models | Store large checkpoints in approved storage, not in Git or Overleaf. |
| `results/` | Run records and small, useful summaries | Keep enough configuration and version information to connect a result to its inputs and code. |
| `writing/` | Literature review notes, references, and report sections | The LaTeX starter at the repository root is ready to import into Overleaf. |
| `docs/` | Project log, decisions, environment notes, and reproducibility checklist | Update these as you work, not only at submission time. |

## 3. Start with a research record

- [ ] Add the project aim, research questions, and planned outputs to [docs/PROJECT_LOG.md](docs/PROJECT_LOG.md).
- [ ] Start a literature search and keep a record in [writing/reading_log.csv](writing/reading_log.csv). Save citation details in [writing/references.bib](writing/references.bib).
- [ ] Record decisions that affect the method, data, or interpretation in [docs/DECISIONS.md](docs/DECISIONS.md), including why you made each decision.
- [ ] Agree with your supervisor where data, code, and model files may be stored and who may access them. Do not commit passwords, API keys, personal data, or material whose licence or consent does not allow sharing.

## 4. Keep data and results traceable

- [ ] For every dataset, record its source, version or date, access conditions, and checksum in `data/manifest.csv` or a fuller dataset record based on [templates/dataset_record.md](templates/dataset_record.md).
- [ ] Keep original data unchanged. Put downloaded originals in `data/raw/` and generated data in `data/processed/`; record the script and settings that produced each derivative.
- [ ] The data folders are ignored by Git by default to prevent accidental uploads. Use storage approved for the project and put access instructions or a stable link in the manifest. Only change `.gitignore` to track files after checking size, licence, privacy, and supervisor approval.
- [ ] For each substantial analysis, copy [templates/experiment_record.yml](templates/experiment_record.yml) and record the input data version, code commit, command, settings, random seed (if relevant), environment, and output location.
- [ ] Keep the configuration and code that generated a result. Do not rely on an undocumented manual edit or a notebook cell that only exists in one person’s session.

## 5. Record the computing environment

- [ ] Write down the operating system, language and package versions, and any required external software in [docs/ENVIRONMENT.md](docs/ENVIRONMENT.md).
- [ ] Keep an environment file or lock file with the project when practical (for example, `environment.yml`, `requirements.txt`, or a package-manager lock file).
- [ ] Record code changes in small, meaningful Git commits. Push regularly so the work is backed up and the project history stays useful.

## 6. Work on the literature review and report in Overleaf

- [ ] Push the initial project repository to GitHub.
- [ ] In Overleaf, create a **new project from GitHub** and select this project repository. `main.tex` is the report entry point; the literature review and other chapters are in `writing/sections/`.
- [ ] Link GitHub to Overleaf in your Overleaf account settings if prompted. GitHub synchronization is a premium Overleaf feature. It is not automatic: use the GitHub option in the Overleaf project menu to pull or push changes.
- [ ] Treat Overleaf and GitHub as two editors of the same writing files. Sync before switching editors, and avoid editing the same file in both places before syncing.
- [ ] Keep `writing/references.bib` and the report source in the repository. Save the Overleaf project URL in the project details above and in [writing/README.md](writing/README.md).

Overleaf’s GitHub sync creates GitHub commits under the connected GitHub account owner, and several Overleaf edits may be bundled into one commit. Keep `AUTHORS.md` and the project log current so contributions and decisions remain clear. See the [Overleaf GitHub synchronization guide](https://docs.overleaf.com/integrations-and-add-ons/git-integration-and-github-synchronization/github-synchronization) for current setup steps and limitations. If GitHub sync is unavailable, use Overleaf’s Git integration or upload the writing files; record which workflow you chose.

## 7. Before sharing a result

- [ ] Can you identify the exact input data and its source/version?
- [ ] Can you identify the code commit, configuration, and environment used?
- [ ] Can you regenerate the figure or summary from the recorded inputs?
- [ ] Are limitations, failed runs, and exclusions recorded rather than silently omitted?
- [ ] Have your supervisor and any relevant data owner approved sharing the repository and its contents?

Use the fuller checklist in [docs/REPRODUCIBILITY_CHECKLIST.md](docs/REPRODUCIBILITY_CHECKLIST.md) before handover or submission.

## 8. Handy Git commands

Run these from the project folder:

```bash
git status
git add -A
git status
git commit -m "Document project setup and literature review"
git push
```

Review the second `git status` before every commit: it shows what will be included. The ignored data and checkpoint files will not be staged. If a file should not be shared, do not add it; tell your supervisor and document where the approved copy is stored. GitHub Desktop is also a good option if you prefer a graphical interface.
