# What is a FAIR-IO
A FAIR-IO (FAIR Image Object) bundle combines acquisition and provenance metadata together with multi-resolution, chunked binary pixel data in a single cloud-compatible format for simplified sharing and re-use. As such, FAIR-IO implements
a FAIR Digital Object (FDO, [DOI:10.5281/zenodo.7824714](https://doi.org/10.5281/zenodo.7824714)) as illustrated below.

![FAIR-IO concept](FAIR-IO_10.5281-zenodo.10512531.png)

FAIR-IO is based on the following recommendations for binary (pixel) data and textual metadata.
## Recommendations for easily shareable binary data:
- Use data formats that store binary data with multiple resolutions in a single cloud-compatible, chunkable format. These enable web-optimised data access and high-performance cloud storage
- Store data in a public available space accessible via a data specific URL
**Example format:** ome-zarr ([About]("https://doi.org/10.1007/s00418-023-02209-1") | [Tools](tools:ref:main))


**Example format**: OME-Zarr ([About](https://doi.org/10.1007/s00418-023-02209-1) | [Tools](../tools/index.md))

## Recommendations for easily shareable metadata:
- Ensure that the relationship and meaning of the data is clear described or linked</li>
- Use metadata formats that store metadata in a machine readable form, that means </li>
- store data in a public available space accessible via a data specific URL</li> 

**Example formats:** JSON-LD [About](https://json-ld.org/) | [Tools](tools:ref:main), Turtle [About](https://www.w3.org/TR/turtle/)







