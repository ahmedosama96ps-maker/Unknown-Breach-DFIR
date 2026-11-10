# Investigation Timeline

This timeline summarizes the most relevant events correlated from file-system, Recycle Bin, USB, browser, registry, ShimCache, and Velociraptor evidence.

| Date / Time (as recorded) | Event | Artifact / review source | Interpretation / limit |
|---|---|---|---|
| 2014-02-03 | Lexar JumpDrive Secure 64MB attached | USB artifacts (see [artifact summary](artifact_summary.md) and [full report](../docs/Digital_Forensics_Investigation_Report.pdf)) | Removable-media activity; specific file movement not established |
| 2014-02-17 | `factory2000Plus-tables.mdb` deleted from Jimmy Wilson's Documents | Recycle Bin | Deleted structured/business data artifact |
| 2014-02-17 | `New Prices` folder and related text files appeared in deleted-file evidence | Recycle Bin | Indicates deletion or cleanup of pricing-related data |
| 2014-02-20 | Kingston DataTraveler 100 attached | USB artifacts (see [artifact summary](artifact_summary.md)) | Additional removable-media activity; not proof of transfer |
| 2014-02-20 | SanDisk Card Reader identified | USB artifacts (see [artifact summary](artifact_summary.md)) | Additional removable-media device present; timing/transfer not independently reverified |
| 2015-05-26 14:45 | `New Price List.txt` identified | File system / Autopsy | Pricing-related data under Jimmy Wilson's profile |
| 2015-05-26 14:45 | `New Price List Encoded.txt` identified | File system / Autopsy | Encoded version of the pricing data |
| 2015-05-26 14:45 | Browser/search artifacts referenced “How to Hide Money From the Government” | Browser / keyword artifacts | Relevant to possible financial concealment intent |
| 2015-05-26 14:45 | `BCTextEncoder.exe` identified on Jimmy Wilson's Desktop | ShimCache + Velociraptor | Encoding tool potentially linked to the encoded price list |
| 2015-05-26 14:46 | LNK/recent-document artifacts referenced `New Prices` and related files | Recent Documents / LNK | Supports user interaction with the pricing files |

## Timeline Assessment

The strongest cluster of evidence centers on Jimmy Wilson's pricing-related files, the encoded price list, `BCTextEncoder.exe`, and concealment-related browser artifacts. USB activity provides a possible data-movement path, but the available evidence does not establish a specific file transfer.


## Timestamp and provenance limitations

These timestamps are **reported from the existing project investigation**, not independently re-extracted in this documentation revision. The dates/times in this high-level summary are *not* accompanied by per-event raw record IDs, filesystem timestamp type (created/modified/accessed/changed), time-zone conversion details, or exported source offsets. Accordingly, the chronology should be treated as **an investigation summary**, not a courtroom-grade timestamp reconstruction.

Before using this timeline as formal forensic evidence, re-open the source image in the documented tools, export each relevant artifact with its exact path and record identifier, note whether timestamps are UTC or local, preserve timezone assumptions, and link the screenshot or exported record to each event. The linked [full forensic report](../docs/Digital_Forensics_Investigation_Report.pdf), [artifact summary](artifact_summary.md), and [screenshots](../screenshots/) provide existing review context but should not be confused with a complete artifact-by-artifact chain of custody.

**Interpretation:** ShimCache file references and Velociraptor file presence do not alone prove program execution. A connected USB device does not by itself prove that an identified pricing file was copied to it. Browser or search keywords establish an artifact, not a person's intent.
