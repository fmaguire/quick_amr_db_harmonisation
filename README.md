# Crude AMR database harmonisation

We need a quick way to compare results between different AMR databases
While there are better ideas of dealing with this problem more robustly 
(...speak to me about genomically-informed nomenclature normalisation),
for mapping NCBI and ResFinder to CARD's ARO:

- Download NCBI and ResFinder databases

- Run them through RGI

- Using hits, create a mapping of NCBI and ResFinder genes to the ARO

- Highlight any situation of no hits/disconnect for manual curation
