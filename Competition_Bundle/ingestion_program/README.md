# Ingestion Program

Loads the training data, training labels and test data from `input_data/`, trains the model of `sample_code_submission/`, and saves its predictions in `sample_result_submission/`.

To run it locally:

```bash
cd Competition_Bundle
python3 ingestion_program/run_ingestion.py
```

Do not modify or delete `metadata.yaml`: Codabench uses it to run the program. Folder names differ between a local run and Codabench, and the program handles both without any change.
