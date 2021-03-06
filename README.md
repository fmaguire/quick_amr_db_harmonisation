# Crude AMR database harmonisation

We need a quick way to compare results between different AMR databases
While there are better ideas of dealing with this problem more robustly 
(...speak to me about genomically-informed nomenclature normalisation),
for mapping NCBI and ResFinder to CARD's ARO:

- Download NCBI and ResFinder databases

- Run them through RGI

- Using hits, create a mapping of NCBI and ResFinder genes to the ARO

- Highlight any situation of no hits/disconnect for manual curation

## Running

    conda env create -f env.yml
    conda activate crude_harmonisation
    bash crude_db_harmonisation.sh

Output mapping can be found at `resfinder_ncbi_ARO_mapping.tsv`

- 93.1% of ResFinder entries with trivial mapping to ARO using homology models (218 entries missing).
- 80.7% of NCBI entries with trivial mapping to ARO using homology models (1260 entries missing).

