# Dataset and Evidence Validation

## Dataset

- **Repository:** NIST CFReDS
- **Image Name:** `2020JimmyWilson.E01`
- **Image Format:** E01

The dataset was selected because it is a publicly available Windows forensic image containing realistic user activity suitable for disk-forensic investigation and Windows artifact analysis.

## Evidence Integrity

FTK Imager was used to validate the forensic image before analysis.

| Hash | Value |
|---|---|
| MD5 | `b267fb0cd94645425eee00258d3a9b58` |
| SHA1 | `a1102c70a50768b588225fdcad6efa5d5d57341b` |

**Verification result:** Both hashes matched.

## Handling

The image was inspected and mounted read-only for analysis. The raw E01 evidence file is not included in this GitHub repository.
