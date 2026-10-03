# Pollinators Detection Challenge

Design and resolution of a machine learning challenge on Codabench: detecting pollinators in image sequences. The repository contains everything needed to run the challenge (data loading, ingestion and scoring programs, web pages), a starting kit for participants, baseline models, and our solutions to two other challenges.

For data confidentiality reasons, the data is not included in this repository.

## The challenge

Each sample is a short sequence of frames, like a stop-motion video, stored in an HDF5 file and labeled 1 if a pollinator is visible and 0 otherwise. The classes are highly imbalanced, so the challenge is scored with metrics suited to imbalanced binary classification. Solutions should also stay lightweight, since such a detector is meant to run continuously on limited hardware.

## Repository layout

| Path | Content |
| --- | --- |
| `Competition_Bundle/` | The Codabench bundle: configuration, ingestion and scoring programs, sample submissions, web pages |
| `Starting_Kit/` | Notebook for participants: data download, exploration, baselines and submission |
| `resolution/` | Our solutions to the challenges of two other groups |
| `split_data.py` | Builds the train and test split while keeping all frames of a video in the same split |

Each folder has its own README.

## Getting started

1. Open `Starting_Kit/README.ipynb` and run it to explore the data and the baselines.
2. Write a model following `Competition_Bundle/sample_code_submission/model.py`.
3. Test it locally:

   ```bash
   cd Competition_Bundle
   python3 ingestion_program/run_ingestion.py
   python3 scoring_program/run_scoring.py
   ```

4. Submit it on Codabench.

Do not modify or delete the `metadata.yaml` files: Codabench needs them. Folder paths differ between a local run and Codabench, and the bundle handles both.

## Authors

Li Zeying, Charlotte Zuolong, Baptiste Pras, Martin Leiva, Vladimir Herrera-Nativi, and Javier Peña Castaño.
