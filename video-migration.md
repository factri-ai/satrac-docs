# Video Migration Guide

## Google Drive to S3 Video Mapping

Download each video from Google Drive and rename with descriptive names before uploading to S3.

### production_tracking.md
| Google Drive ID | New Filename | Description |
|-----------------|--------------|-------------|
| 1Wv5AyxRQI3ba510egsT8xykDCOwLFSg1 | production-tracking-01.mp4 | |
| 1aqqISucoafqT0oXPnGAsCL9dVANP27XX | production-tracking-02.mp4 | |
| 12ee3Afg5nzglqKpgP4muEgZdcIxQ3apI | production-tracking-03.mp4 | |
| 1haiSs9bWlL4LpBPuhpOp2yMh9HL3Tv68 | production-tracking-04.mp4 | |
| 1TGfPjTcYPD_q9hJZa3Q1mHXX2QZlklMf | production-tracking-05.mp4 | |
| 1unhBlNbAEzuj1bnNLZN_hyU9RXMhBcJi | production-tracking-06.mp4 | |
| 1c5jf_4goKuyYesI8ybekcw-w5uj8dgsn | production-tracking-07.mp4 | |
| 1T3IU9HzeOmQlIQx6p_TpbtcpS45wBO6D | production-tracking-08.mp4 | |

### quality_checksheets.md
| Google Drive ID | New Filename | Description |
|-----------------|--------------|-------------|
| 1N4Wt5gQx3grH5vvstpMDhKcflRg5jJHw | quality-checksheet-01.mp4 | |
| 1wyXtORO2UotBV2B8JHnyb_Sf_piCq7jj | quality-checksheet-02.mp4 | |
| 1oqrOqLL9EwAicRlZvULwojifaZhq_s7R | quality-checksheet-03.mp4 | |
| 1clZVOx2MOrLjrNzIYFvpT8WBuaNaqGlB | quality-checksheet-04.mp4 | |
| 1JW8mgsDhgeQGybbyH_sxnE7kptrdj5Kb | quality-checksheet-05.mp4 | |
| 1L-XAUeC7veeIbiGmvW7LBEAHUkh9MT2D | quality-checksheet-06.mp4 | |

### subassembly_tracking.md
| Google Drive ID | New Filename | Description |
|-----------------|--------------|-------------|
| 1LapwsqpRuPPB5aXEaOkIJlThpfNlr7So | subassembly-01.mp4 | |
| 1_Wi-A6u4HsnTXS3fCMdci4_0ZYs1UeIC | subassembly-02.mp4 | |
| 17wkQzEF9pMk86YJCOneoKYI4CyZB-3SD | subassembly-03.mp4 | |
| 1l_-_v4ZdusvngTrEE1Yb7ZdolkjScfBG | subassembly-04.mp4 | |
| 1SnNpuQ4FYf9gc8XvYCKvXIeqPC2bBBTu | subassembly-05.mp4 | |
| 1ZhgFf4tBlh6U_BI5yYLWak22bUGDI-3- | subassembly-06.mp4 | |

### line_stoppage.md
| Google Drive ID | New Filename | Description |
|-----------------|--------------|-------------|
| 1nVzgkS09hIkZZLDTU-4ArpIPMaqjloRR | line-stoppage-01.mp4 | |
| 1D8yhVzK606o5qJSNggmwMp6EmDpoRfyw | line-stoppage-02.mp4 | |
| 1tUgAgLtK4yqdOXwQBiU1atCnzq4vNVJD | line-stoppage-03.mp4 | |
| 1eF4a7UW7boK3CE3uWfpFb4giPuOBv-ue | line-stoppage-04.mp4 | |
| 1b538XADdHfsUNVQj5KXlOTTE3yJbUcfP | line-stoppage-05.mp4 | |

## Download Commands

```bash
# Install gdown
pip install gdown

# Download each video (example)
gdown https://drive.google.com/uc?id=1Wv5AyxRQI3ba510egsT8xykDCOwLFSg1 -O videos/production-tracking-01.mp4
```

## New Embed Format

Replace Google Drive iframes:
```html
<!-- Old (Google Drive) -->
<iframe src="https://drive.google.com/file/d/FILE_ID/preview" width="711" height="400"></iframe>

<!-- New (CloudFront) -->
<video width="711" height="400" controls>
  <source src="/videos/video-name.mp4" type="video/mp4">
</video>
```

### subassembly_tracking_v2.md (added 2026-08-18)
| Google Drive ID | New Filename | Description |
|-----------------|--------------|-------------|
| 1Zm2IpsKdppVmBa7-JJg8sd6Kn_dVEQcy | subassembly-tracking-v2-01.mp4 | Scan standing QR + Move to Stock confirmation (SO/SF linkage, photo, confirm) |
| 1Of5BLDp7gHh8VT-I0gp61COA0N-4b6lI | subassembly-tracking-v2-02.mp4 | Chassis search + Consumed Sub-Assemblies view |
| 1nfMer4sm1p-HXFq5ChGfNCAIzpj8wprb | subassembly-tracking-v2-03.mp4 | PPC Dashboard Sub Assembly tab: trend + daily report |
