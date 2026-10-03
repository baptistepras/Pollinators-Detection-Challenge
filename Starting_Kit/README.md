# Starting Kit

`README.ipynb` helps participants load, explore and model the data. Run its cells in order.

* **Data download**: the notebook downloads the dataset if it is not already present. For data confidentiality reasons, the data is no longer available.
* **Exploration**: class distribution, which shows the strong imbalance, visualization of frames and sequences, and a first look at feature extraction with PCA.
* **Baselines**: simple models and metrics suited to imbalanced binary classification, as a starting point rather than optimal solutions.
* **Submission**: the last cell builds a submission in the format expected by Codabench.

Each `.h5` file is a sequence of images, like a short stop-motion recording, with a single binary label telling whether a pollinator is present.

| Path | Content |
| --- | --- |
| `data/` | Where the notebook stores the data |
| `sample_code_submission/` | Baseline model and analysis scripts |
| `submission/` | Example of a submission archive |
