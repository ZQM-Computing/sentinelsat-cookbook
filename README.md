# sentinelsat Cookbook

<!-- ZQM-START -->
<!-- markdownlint-disable MD033 -->
<p align="center">
  <strong>ZQM Computing — Geospatial Engineering & Scientific Computing</strong><br>
  <a href="https://github.com/ZQM-Computing">ZQM Computing</a>
</p>
<!-- markdownlint-enable MD033 -->
<!-- ZQM-END -->

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

A **sentinelsat cookbook** for Copernicus Sentinel search and download patterns. Patterns are drawn from the ZQM fleet's sentinelsat 1.2.1 installs (import- and version-verified). Live use is blocked on the owner's free Copernicus account, so the patterns are written for that account, not run against it here. It is intended for Earth-observation practitioners who fetch Sentinel imagery programmatically. Validate each pattern against your own data, software versions, and operating environment before adopting it.

## Repository role and status

**Status:** Active, public — seeding. Pattern passes land in follow-up work from fleet-verified setups; the tables below list what is planned, not what is already written.

**What this repository is:** sentinelsat patterns — see the table below.

**What it contributes:** Part of the ZQM Computing geospatial portfolio. Intended to provide geospatial data feeds (satellite imagery, weather, routing, geocoding) for the ZQM game platform. The umbrella index for the series is [geospatial-cookbooks](https://github.com/ZQM-Computing/geospatial-cookbooks).

**Standing:** This repository is maintained independently. Automated checks cover only the paths and environments configured in its workflows; they do not establish production readiness or operational certification.

## Who this is for

Earth-observation practitioners who fetch Sentinel imagery programmatically.

## Prerequisites

- sentinelsat 1.2.1
- A free Copernicus account, kept out of repos
- Python 3.11+

## Patterns (planned)

| # | Example | What it will demonstrate |
|---|---------|--------------------------|
| 01 | `01-search` | Searching the catalog by footprint and date |
| 02 | `02-download` | Downloading products and verifying checksums |
| 03 | `03-full-workflow` | End-to-end: search → download → COG-ready raster (see cog-cookbook) |

## Repository layout

```text
sentinelsat-cookbook/
├── examples/          # pattern passes, landing in follow-up work
├── README.md
└── LICENSE
```

## Roadmap

- First pattern pass: the first two table rows
- Second pass: the remaining rows, from fleet-verified setups

## Contributing

A contributing guide lands with the first pattern pass. Report security issues to <zqmcomputing@gmail.com> — please do not open a public issue for those.

## More from this series

- [cog-cookbook](https://github.com/ZQM-Computing/cog-cookbook) — Cloud Optimized GeoTIFF creation, validation, TiTiler serving
- [stac-cookbook](https://github.com/ZQM-Computing/stac-cookbook) — STAC catalog creation, item validation, search API, bulk ops
- [pgstac-cookbook](https://github.com/ZQM-Computing/pgstac-cookbook) — STAC catalogs in PostGIS, stac-fastapi APIs, bulk ingest
