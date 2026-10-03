# Scoring Program

Loads the test labels from `reference_data/` and the predictions from `sample_result_submission/`, computes the score, and saves it in `scoring_output/`.

To run it locally, after the ingestion program:

```bash
cd Competition_Bundle
python3 scoring_program/run_scoring.py
```

Do not modify or delete `metadata.yaml`: Codabench uses it to run the program. Folder names differ between a local run and Codabench, and the program handles both without any change.
