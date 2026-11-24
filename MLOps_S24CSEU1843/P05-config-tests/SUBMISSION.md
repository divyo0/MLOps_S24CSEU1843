# P05 — Submission evidence checklist

Name: Divy Mathur
Enrollment: s24cseu1843
Batch: [enter your actual batch]
Laboratory session date: [enter actual date]
Repository (planned, publish first): https://github.com/divyo0/MLOps_S24CSEU1843/tree/main/P05-config-tests

AI use disclosure: I used ChatGPT to review, debug and organize my MLOps lab files and to help prepare execution instructions.

## config.yaml
```yaml
# Settings for the delivery-time model.
# Change values here, never in the code.

data:
  path: ../data/delivery_times.csv
  features:
    - distance_km
    - prep_time_min
    - traffic_level
    - rain
  target: delivery_min

split:
  test_size: 0.2
  seed: 42

model:
  name: linear_regression
```

## Refactor
Measured test MAE before: 1.92 minutes; after: 1.92 minutes. Limited 300-row task: 2.178175 minutes.

## Evidence
Actual tool run: 10 pytest tests passed; see pytest_result.txt. Run `python -m pytest -v` from work and capture your own screenshot.
