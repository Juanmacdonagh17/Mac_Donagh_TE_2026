# Transposable elements as evolutionary substrates of protein disorder in the human proteome

**Juan Mac Donagh, Nicolas Vergesio, Andrea Aguilar, Rodrigo Nores, Antonio Lagares, Maria Silvina Fornasari, Gustavo Parisi**

Universidad Nacional de Quilmes · CONICET · Universidad Nacional de Córdoba · Universidad Nacional de La Plata

---

## Abstract

Intrinsically disordered regions (IDRs) are central contributors to protein function, evolution and human disease, yet the evolutionary routes that seed new disordered segments within pre-existing proteins are still poorly understood. Here, we systematically mapped TE-derived segments across human proteins and isoforms, and found that these insertions are strongly enriched in intrinsic disorder. Recent, Primate-specific insertions preferentially generate disordered segments, whereas older insertions more frequently occupy ordered structural contexts, revealing an age-dependent transition in the conformational state of TE-derived sequences. These findings identify TEs as a major evolutionary mechanism linking genome mobility to the emergence of new disordered conformational ensembles in the human proteome.

---

## Repository structure

```
Mac_Donagh_TE_2026/
├── main/
│   ├── figures/
│   │   ├── figure1.pdf
│   │   ├── figure2.pdf
│   │   ├── figure3.pdf
│   │   ├── figure4.pdf
│   │   └── figure5.pdf
│   └── extended_data/
│       ├── extended_data_fig1.pdf
│       ├── extended_data_fig2.pdf
│       ├── extended_data_fig3.pdf
│       ├── extended_data_fig4.pdf
│       ├── extended_data_fig5.pdf
│       ├── extended_data_fig6.pdf
│       └── extended_data_fig7.pdf
├── scripts/
│   └── (R scripts for all analyses and figure generation)
├── data/
│   ├── supplementary_table_1.csv
│   ├── supplementary_table_2.csv
│   ├── supplementary_table_3.csv
│   ├── supplementary_table_4.csv
│   └── supplementary_table_5.csv
└── README.md
```

Supplementary Tables 6–20 and all processed datasets are archived on Zenodo (see below).

---

## Data availability

All supplementary tables and processed datasets are deposited on Zenodo:

**DOI: [10.5281/zenodo.20648235](https://doi.org/10.5281/zenodo.20648235)**

To download all files from the Zenodo record at once:

```bash
RECORD_ID=20648235
curl https://zenodo.org/api/records/${RECORD_ID} \
  | python3 -c "import sys,json; [print(f['links']['self']) for f in json.load(sys.stdin)['files']]" \
  | wget -i -
```

Or to download a specific file directly:

```bash
wget https://zenodo.org/records/20648235/files/supplementary_table_6.csv
```

---

## Figures

### Main figures

| Figure | Description |
|--------|-------------|
| Figure 1 | Transposable element insertions in the human proteome |
| Figure 2 | TE insertions in coding sequences are enriched in intrinsic disorder |
| Figure 3 | GC content and compositional properties drive disorder in TE-derived sequences |
| Figure 4 | Evolutionary age of TE insertions correlates with disorder content |
| Figure 5 | Expression and splicing properties of TE-containing isoforms |

### Extended Data figures

| Figure | Description |
|--------|-------------|
| Extended Data Figure 1 | E-value distributions and strand insertion preference |
| Extended Data Figure 2 | Disorder enrichment is robust across multiple predictors |
| Extended Data Figure 3 | Primate TE insertions show distinct disorder profiles across repeat classes |
| Extended Data Figure 4 | CpG-adjusted Kimura divergence distributions of Alu subfamilies |
| Extended Data Figure 5 | Z-score-based age stratification of Alu subfamily insertions |
| Extended Data Figure 6 | TE insertions contribute to disordered and functionally relevant protein regions |
| Extended Data Figure 7 | Splicing properties of TE-containing isoforms |

---

## Reproducibility

All analyses were performed in R 4.5.3. Scripts for data processing, statistical analyses and figure generation are in the `scripts/` folder. Full computational environment details are described in the Methods section of the manuscript.

Computational resources: [CCAD – Universidad Nacional de Córdoba](https://supercomputo.unc.edu.ar), SNCAD, República Argentina.

---

## Citation

> Mac Donagh J, Vergesio N, Aguilar A, Nores R, Lagares A, Fornasari MS, Parisi G.
> **Transposable elements as evolutionary substrates of protein disorder in the human proteome.**
> *bioRxiv* (2026). DOI: [10.5281/zenodo.20648235](https://doi.org/10.5281/zenodo.20648235)

---

## License

Code: [MIT License](LICENSE)
Data: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

---

## Contact

Gustavo Parisi · gusparisi@gmail.com · Universidad Nacional de Quilmes
