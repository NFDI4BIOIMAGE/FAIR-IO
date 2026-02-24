# Guidelines

## RO-Crate quick checklist – are you building the right type?

1. Do you know the total size of the files?
        < 5 GB → attached is fine.
        > 5 GB → think detached.

2. Do you control the licence of the files?
        Yes, you can share them → attached.
        No, you can only provide a citation → detached.

3. Will the data ever be updated?
        No, it’s a static snapshot → attached.
        Yes, you’ll keep a “live” version → detached.

4. Do you need an easy, single‑file transfer?
        Yes → attached.
        No, you’re fine with a list of URLs → detached.

If you answer “yes” to 1–3, go with attached; otherwise, go detached.

(guidelines:ref:checklistZarr)=
## Checklist – When to choose OME‑Zarr
|✅ Condition |	Why OME‑Zarr is beneficial|
| --- | --- |
| Dataset is large (multi‑GB to TB) |	Chunked storage and lazy loading keep memory use low.|
| Data need to be accessed remotely or collaboratively |	Zarr’s cloud‑native layout works with object storage (S3, GCS, Azure) and enables parallel reads/writes.|
| Multiscale or pyramidal representations are required |	Built‑in multiscale groups let you store and retrieve low‑resolution views efficiently.|
| Rich metadata (OME‑NGFF) must be preserved | 	Standardized JSON metadata keeps experimental context, acquisition parameters, and provenance together with the pixels.|
| You need on‑the‑fly transformations (e.g., stitching, reprojection, channel mixing) |	Upcoming spec features will allow transformation pipelines to be stored alongside the data.|
| Your workflow involves chunk‑wise processing or analysis pipelines |	Each chunk can be read/written independently, ideal for distributed or HPC pipelines.|
| Long‑term archival and format stability are a priority |	The open‑source Zarr format is versioned, community‑maintained, and well‑documented.|
| You want to avoid monolithic files that are hard to update |	Adding or modifying a single chunk does not require rewriting the whole file.|
| Your data will be shared publicly or deposited in repositories |	Zarr’s transparent directory structure is easy to host on public cloud buckets or institutional servers.|
