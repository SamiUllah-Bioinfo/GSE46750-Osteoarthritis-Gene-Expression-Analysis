# Python-Based Analysis of Osteoarthritis Gene Expression (GSE46750)

## 1. Project Overview

This project presents a beginner-friendly Python analysis of significant
differentially expressed probes identified in the GEO dataset GSE46750.

The analysis focuses on comparing inflammatory and normal/reactive regions
within osteoarthritis synovial tissue.

## 2. Dataset

- GEO accession: GSE46750
- Organism: Homo sapiens
- Platform: Illumina HumanHT-12 V4.0 expression beadchip
- Input file: GSE46750_significant_annotated_probes.csv
- Significant probes: 152

## 3. Tools and Libraries

- Python
- Pandas
- Matplotlib
- Google Colab

## 4. Analysis Performed

1. Loaded the significant probe results from the original R analysis.
2. Inspected the dataset and its columns.
3. Selected the top five significant probes.
4. Visualized log fold changes using a horizontal bar chart.
5. Exported the selected results as a CSV file.

## 5. Top Five Significant Probes

| Gene | logFC | Adjusted p-value |
|---|---:|---:|
| CD48 | 0.8083 | 0.02243 |
| MATN2 | -0.9352 | 0.02243 |
| SNTB1 | 0.3778 | 0.02243 |
| MAN1C1 | 0.6739 | 0.02416 |
| IRF8 | 0.6869 | 0.02744 |

Positive logFC values indicate higher expression in inflammatory regions,
while negative values indicate lower expression, relative to normal/reactive regions.

## 6. Output Files

- GSE46750_top5_gene_expression.png
- GSE46750_top5_gene_results.csv

## 7. Limitations

This is a short exploratory Python analysis based on significant results
previously obtained using R and the limma package. It does not repeat the
original differential expression analysis.

The top five probes are selected by their order in the input results,
which are ranked by adjusted p-value.

## 8. Conclusion

This project demonstrates the use of Python for loading, inspecting,
visualizing, and exporting gene expression results from a public
osteoarthritis transcriptomics dataset.
