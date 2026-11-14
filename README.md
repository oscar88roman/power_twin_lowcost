# Power Twin: low-cost mapping to Building Energy Models

Project page and results for the ISPRS LC3D 2026 paper

**Towards Building Energy Digital Twins with a Low-Cost Portable Mobile Mapping System**
Oscar Roman, Paweł Trybała, Elisa Mariarosaria Farella, Fabio Remondino
3D Optical Metrology (3DOM) unit, Bruno Kessler Foundation (FBK), Trento, Italy

## What is here

- `index.html` is the project page. It follows the paper (abstract, method, results, case study, conclusions). After the paper sections come a few videos and extra figures, and then an explorer for all 312 ScanNet scans.
- `assets/` has the paper figures.
- `media/` has the videos, the extra figures and an interactive 3D view of the case-study flat.
- `data/scenes.json` holds the reconstructed model and the metrics for every scan. `data/pts/` has a 45,000-point sample of each scan, and `data/thumbs/` has the gallery thumbnails.

## Viewing the page

The page is a static site and is published with GitHub Pages. To open a specific scan, add its ID to the address, for example `#scene0025_00`.

To view it on your own computer, start a small web server in this folder (opening the file directly will not load the data):

```
python -m http.server 8000
```

Then go to http://localhost:8000.

## Citation

```
@inproceedings{roman2026lowcost,
  title     = {Towards Building Energy Digital Twins with a Low-Cost Portable Mobile Mapping System},
  author    = {Roman, O. and Trybała, P. and Farella, E. M. and Remondino, F.},
  booktitle = {ISPRS LC3D 2026},
  year      = {2026}
}
```

This work was carried out within the Power Twin project, supported by the 2026 PoC by Trentino – Test Your Idea! programme, promoted by Fondazione Bruno Kessler and the University of Trento (Italy).
