# Disclaimer and Scope

This repository documents an **educational digital-forensics investigation** performed on the public NIST CFReDS `2020JimmyWilson.E01` training image.

## Scope Notes

- The raw forensic image is not distributed in this repository.
- The evidence source was a forensic disk image rather than a live endpoint.
- `Amcache.hve` was not available in the analyzed dataset.
- ShimCache/AppCompatCache can support historical file presence or possible execution traces, but does not independently prove execution.
- USB artifacts confirm device attachment, but do not independently prove that a specific file was copied to the device.
- Conclusions in this repository are based only on the artifacts available in the analyzed image.

This material is intended for learning, portfolio demonstration, and defensive cybersecurity education.
