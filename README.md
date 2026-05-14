# MGS-1 Reduced-Mass Geotechnical Index Testing

This repository contains the data, analysis notebook, generated tables, and thesis-ready figures for reduced-specimen-mass geotechnical index testing of the MGS-1 Mars regolith simulant.

The purpose of the repository is to make the calculations behind the thesis figures and tables reproducible from the included CSV input data.

## Repository Structure

- `MGS1_analysis_.ipynb` - main reproducible analysis notebook used to generate the final thesis figures and tables.
- `data/` - input CSV files used by the notebook.
- `tables/` - generated CSV tables used in the thesis.
- `figures/` - generated archival PDF figures.
- `figures_word/` - Word-ready figure exports.
  - `svg/` contains vector figures recommended for Word.
  - `png_450dpi/` contains high-resolution PNG fallback files.
- `requirements.txt` - Python package requirements.

## Reproducing the Results

From the repository root, install the required packages:

```bash
pip install -r requirements.txt
```

Then open the notebook:

```bash
jupyter notebook MGS1_analysis_.ipynb
```

Run all cells from top to bottom. The notebook regenerates:

- CSV tables in `tables/`
- PDF figures in `figures/`
- SVG and PNG figure exports in `figures_word/`

## Figure Export Notes

The figures are exported at the intended thesis text width rather than as oversized images that must be downscaled in Word. This helps preserve consistent text size, marker size, line weight, and PDF export quality.

Use the SVG files in `figures_word/svg/` when inserting figures into Word. They are vector graphics and should remain sharp in exported PDFs. If Word has trouble with a specific SVG file, use the matching PNG file from `figures_word/png_450dpi/`.

## Tables

The notebook regenerates all thesis tables in `tables/`, including water content, particle density, sieve summaries, hydrometer quality, stitched gradation metrics, loose/tapped density, and mineralogical density estimates.

The stitched gradation table uses the same stitched curves as the exported PSD figures.

## Notes

Generated figures and tables are included so the results can be inspected without rerunning the notebook. The source CSV files in `data/` are the reproducible inputs.
