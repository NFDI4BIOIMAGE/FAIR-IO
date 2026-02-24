# OME-Zarr

## What makes OME‑Zarr so appealing?

```{figure} monolithic-vs-chunked-300dpi-480x701.png
---
width: 50%
align: right 
name: chunkedDataCartoon
---
```

- **Instant, on‑demand chunk access** – Data is stored in small, independently addressable blocks, so you can stream, subset, or visualise only the pieces you need without loading the whole file.
- **Built in multiscale support** – OME‑Zarr natively handles image pyramids, letting you zoom from low‑resolution overviews straight down to full‑resolution pixels.
- **Fast parallel writes** – The format is optimised for concurrent writes, which is especially handy when saving data to networked or cloud storage systems.
- **Rich, community‑driven metadata** – A flexible, hierarchical metadata schema lets you bundle raw images, segmentation masks, and downstream analysis results together in a single, self‑describing container.
- **Growing ecosystem** – An expanding community contributes tools, plugins, and best‑practice guides, ensuring that OME‑Zarr stays up‑to‑date with the latest imaging workflows.


**Links:**
- [OME-Zarr Ambassador Toolkit](https://ngff.openmicroscopy.org/resources/ambassador-toolkit/index.html)
- [Checklist - When to choose OME-Zarr](guidelines:ref:checklistZarr)
