# Retail Sales Analytics & Forecasting

Download **retail-sales-project.zip** and extract it to access the complete project with its original folder structure.

## Deliverables
- Retail_Analysis.xlsx: cleaned data, calculated columns, conditional formatting, charts and two native pivot tables (Analysis!J4 and J14).
- sql/: SQLite database, schema, ten analysis queries, import script and executed query outputs.
- Retail_PowerBI/Retail.pbip: Power BI report project, embedded data model, DAX and optional CSV refresh query.
- python/Retail_Analysis.ipynb: executed pandas/matplotlib analysis and linear regression sales forecast.
- Project_Report.pdf: six-page methodology, findings, evaluation and recommendations.
- data/: unchanged source, cleaned data, analysis summaries and prediction outputs.

## Open and run
Extract the entire ZIP before opening files. Open the Excel workbook directly. Refresh pivot tables after changing source data. The existing ranges cover the supplied 9,994 lines.

For Python, install `python -m pip install -r python/requirements.txt`, then open the notebook in Jupyter and run all cells from the python folder. The notebook already includes outputs. SQL uses SQLite; open sql/retail.db or rebuild it with `python sql/import_data.py` from the project root.

For Power BI, open Retail_PowerBI/Retail.pbip, click Refresh and review the report. Save As PBIX if your institution requires PBIX. Report definitions pass Microsoft JSON schema validation, but Power BI Desktop rendering and refresh have not been verified. Native Excel pivot refresh was also not available for testing; pivot/cache definitions and saved values were checked structurally.

## Key findings
Sales $2,297,200.86; profit $286,397.02; margin 12.47%. West leads sales. No main category is loss-making; Tables, Bookcases and Supplies lose money. Monthly regression holds out 2017 and achieves MAE $10,793.89 and R-squared 0.681, versus baseline MAE $15,467.89. The 2018 projection is historical, not a current-year forecast.


