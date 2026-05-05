# MGS-1 Reduced-Mass Geotechnical Index Testing

This repository documents the calculation and plotting workflow used for the master's thesis on reduced-specimen-mass geotechnical index testing of MGS-1 Mars regolith simulant.

## Repository Contents

- `MGS1_analysis.ipynb` - streamlined thesis notebook
- `data/` - cleaned input data and source calculation workbooks
- `tables/` - generated CSV tables used in the thesis
- `figures/` - generated PDF figures used in the thesis
- `figures_word/png_600dpi/` - high-resolution Word-ready PNG exports for thesis document assembly
- `requirements.txt` - Python package requirements

## Reproducing the Outputs

From the repository root:

```bash
pip install -r requirements.txt
jupyter notebook MGS1_analysis.ipynb
```

Run all cells in `MGS1_analysis.ipynb`. The notebook regenerates the thesis PDF figures in `figures/`, table CSV files in `tables/`, and high-resolution Word-ready PNG files in `figures_word/png_600dpi/`.

## Notes

The notebook is based on the final thesis plotting style from `MGS1_Samlet_Analyse_komplett5.ipynb`, but has been reduced to the thesis-relevant figures and reorganised in English for review and reuse. Hydrometer calculations retain raw quality-control values where relevant while the plotted PSD values are clipped to the conventional 0-100% range.

For Word on macOS, use the PNG files in `figures_word/png_600dpi/` rather than inserting the PDF figures directly. These PNGs preserve the original legend layout and are exported directly from Matplotlib at high resolution. In Word, disable image compression if possible before exporting the thesis to PDF.
