# SCore-rust
Single Cell Pathway Scoring powered by Rust

Speed can be workflow altering. By reimplementing pathway (KEGG/Reactome) scoring algorithms for single cell sequencing, higher anaylsis throughput, richer insights, and better interactivity can be achieved.

Wrappers to call the faster implementations directly in R are designed as in-place replacements for SingleCellExperiment and Seurat workflows.

```
# current working example
pass_features(c("ZFP36", "UPF1"))
pass_mat(as.matrix(SeuratObject::pbmc_small@assays$RNA@data))
calc_modulescore()
```
