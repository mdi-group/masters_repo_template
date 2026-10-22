# Reproducibility and handover checklist

Complete this before sending a result for review and again before project handover. Mark items not applicable with a short reason.

## Data

- [ ] Each input dataset has a source, version/date, access conditions, and checksum recorded.
- [ ] Original data are preserved; processing steps produce separately identified derivatives.
- [ ] Any privacy, consent, licence, or sharing restrictions are followed.

## Code and environment

- [ ] The code used for the result is committed, and the commit ID is recorded.
- [ ] Commands, configuration, random seeds where relevant, and software versions are recorded.
- [ ] A new user can follow the setup and run instructions without relying on undocumented local files.

## Results and models

- [ ] Each important result can be traced to its inputs, code, configuration, and output files.
- [ ] Figures can be regenerated from documented scripts and inputs.
- [ ] Model cards and checkpoint locations identify the training data, code version, and evaluation.
- [ ] Failed runs, exclusions, and limitations relevant to the conclusion are recorded.

## Writing and sharing

- [ ] Citations and literature notes are complete enough to trace claims to sources.
- [ ] The report and repository agree on the final methods and results.
- [ ] Names, contributions, permissions, and repository visibility have been reviewed with the supervisor.
- [ ] No credentials, restricted data, or unapproved files are included in the repository.
