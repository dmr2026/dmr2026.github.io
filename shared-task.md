## Shared Task: Parsing to Uniform Meaning Representation

DMR 2026 features a shared task evaluating approaches to automatic prediction of UMR annotation, including sentence graph structure, node attributes, alignment with surface text, and document-level relations. UMR is a relatively new formalism designed for multilingual semantic representation across typologically diverse languages. While based on AMR, it differs substantially, and parsing into UMR remains largely unexplored compared to AMR, which was the focus of CoNLL shared tasks in 2019 and 2020.

**The official shared task website is hosted at Charles University: [https://ufal.mff.cuni.cz/umr-parsing](https://ufal.mff.cuni.cz/umr-parsing)**

### Timeline

| Training/development data release | February 1, 2026 |
|:----------------------------------|:-----------------|
| **Test phase**                    | **February 16 - 27, 2026** |
| **Results announcement**          | **March 1, 2026** |
| **Paper writing period**          | **March 2 - 15, 2026** |
| **Review period**                 | **March 16 - 22, 2026** |

### Data

Training data will be based on UMR 2.1. The shared task will include English, Chinese, and Czech (both training and test data), and possibly other languages (test data only). Test data will consist of approximately 100 sentences per language.

All training/development data will be freely available, without need for registration or signing a contract. The previously unpublished test data will be published under similar conditions after the shared task.

Blind data provided as system input will be tokenized and segmented to sentences; system outputs must preserve tokenization and segmentation.

### Evaluation

The evaluation methodology will use smatch or AnCast, as well as a node-mapping algorithm developed by the organizers. Details and an evaluation implementation will be provided by February 1, 2026.

A main metric will be defined for ranking participating systems, with additional metrics computed (e.g., separate F1-score for concepts). While the main evaluation focuses on sentence graphs, additional metrics will include document-level relations (for systems that predict them) and alignments between nodes and words.

The shared task will not be divided into tracks—all submissions will be evaluated along the same set of metrics.

### Participation

**Registration:** Individuals and teams considering participation should register via the [Google form](https://forms.gle/pc2c7A27TxeHjRKZ7). There is no deadline for registration, but early registration is encouraged as important information will be sent to registered participants by email.

**Submission:** Participants will submit system outputs (parsed data), not the systems themselves. The submission form will be hosted at Charles University and the URL will be available on the shared task website. Each submission will be automatically checked for validity.

There are no restrictions on who can participate.

### Organizers

The shared task is led by Daniel Zeman and Jan Štěpánek (Charles University, Prague), both experienced organizers of past shared tasks, including CoNLL and MRP shared tasks on multilingual Semantic Role Labeling, Universal Dependency parsing, multilingual Meaning Representation Parsing, and more.
