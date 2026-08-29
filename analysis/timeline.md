# Investigation Timeline

This timeline summarizes the most relevant events correlated from file-system, Recycle Bin, USB, browser, registry, ShimCache, and Velociraptor evidence.

| Date / Time | Event | Source | Interpretation |
|---|---|---|---|
| 2014-02-03 | Lexar JumpDrive Secure 64MB attached | USB artifacts | Confirms removable-media usage |
| 2014-02-17 | `factory2000Plus-tables.mdb` deleted from Jimmy Wilson's Documents | Recycle Bin | Deleted structured/business data artifact |
| 2014-02-17 | `New Prices` folder and related text files appeared in deleted-file evidence | Recycle Bin | Indicates deletion or cleanup of pricing-related data |
| 2014-02-20 | Kingston DataTraveler 100 attached | USB artifacts | Additional removable-media activity |
| 2014-02-20 | SanDisk Card Reader identified | USB artifacts | Additional removable-media device present |
| 2015-05-26 14:45 | `New Price List.txt` identified | File system / Autopsy | Pricing-related data under Jimmy Wilson's profile |
| 2015-05-26 14:45 | `New Price List Encoded.txt` identified | File system / Autopsy | Encoded version of the pricing data |
| 2015-05-26 14:45 | Browser/search artifacts referenced “How to Hide Money From the Government” | Browser / keyword artifacts | Relevant to possible financial concealment intent |
| 2015-05-26 14:45 | `BCTextEncoder.exe` identified on Jimmy Wilson's Desktop | ShimCache + Velociraptor | Encoding tool potentially linked to the encoded price list |
| 2015-05-26 14:46 | LNK/recent-document artifacts referenced `New Prices` and related files | Recent Documents / LNK | Supports user interaction with the pricing files |

## Timeline Assessment

The strongest cluster of evidence centers on Jimmy Wilson's pricing-related files, the encoded price list, `BCTextEncoder.exe`, and concealment-related browser artifacts. USB activity provides a possible data-movement path, but the available evidence does not establish a specific file transfer.
