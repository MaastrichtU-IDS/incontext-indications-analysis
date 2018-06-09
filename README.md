
# DrugCentral Indication Quality Analysis

Materials and data generated and analysed to assess the quality of the indication information on [DrugCentral](http://drugcentral.org/). Currently we have manually curated indications for 150 anti-cancer and cardiovascular drugs using the [Hypothes.is](https://web.hypothes.is/) webpage annotation tool to highlight indications in digital drug labels on the [DailyMed](https://dailymed.nlm.nih.gov) website. We then compare these FDA-approved indications to the ones specified by DrugCentral to determine if DrugCentral's information is accurate and precise enough.

#### Description of the contents of this repository:

1. `Analysis-figures/`<br>Figures in .png format demonstrating the number of overlapping indications in our analysed datasets

2. `LabeledIn-comparison/labeledin_crowd.dsv`<br>Official [LabeledIn](https://ftp.ncbi.nlm.nih.gov/pub/lu/LabeledIn/) dataset (portion which was crowdsourced)

3. `LabeledIn-comparison/labeledin_normal.dsv`<br>Official [LabeledIn](https://ftp.ncbi.nlm.nih.gov/pub/lu/LabeledIn/) dataset (portion which was curated by human experts)

4. `LabeledIn-comparison/ManualCuration+DrugCentral.csv`<br>Manually curated indications and those from DrugCentral for the 150 drugs in this study 

5. `LabeledIn-comparison/LabeledInParser.ipynb`<br>[Jupyter](http://jupyter.org/) notebook ([Python](https://www.python.org/)) generating `LabeledIn_comparison_results_table.csv` by automatically analysing `labeledin_crowd.dsv`, `labeledin_normal.dsv` and `ManualCuration+DrugCentral.csv`

6. `LabeledIn-comparison/LabeledIn_comparison_results_table.csv`<br>The results comparing an existing drug-indication database ([LabeledIn](https://ftp.ncbi.nlm.nih.gov/pub/lu/LabeledIn/)) to DrugCentral and our manually curations (file is generated by `LabeledInParser.ipynb`)

7. `MainData.xlsx`<br>Main data file with indications from DrugCentral, our manual curations, and analyses by medical experts (and computer algorithms by [Ted Pedersen](http://www.d.umn.edu/~tpederse/umls-similarity.html)) to determine semantically similar (equivalent) indications that have different names 