### MToolBox (v.1.0)

MToolBox is a highly automated bioinformatics pipeline to reconstruct and analyze human mitochondrial DNA from high throughput sequencing data. MToolBox includes an updated computational strategy to assemble mitochondrial genomes from Whole Exome and/or Genome Sequencing (PMID: 22669646) and an improved fragment-classify tool (PMID:22139932) for haplogroup assignment, functional and prioritization analysis of mitochondrial variants. MToolBox provides pathogenicity scores, profiles of genome variability and disease-associations for mitochondrial variants. MToolBox provides also a Variant Call Format file (version 4.0) featuring, for the first time, allele-specific heteroplasmy.  
  
The MToolBox pipeline includes:

- an extended version of a previously published computational strategy for mtDNA genome assembly (PMID: 22669646). The pipeline has been integrated with the detection of insertions and deletions (indels) and the assessment of the heteroplasmic fraction (HF) and related confidence interval (CI) for each mt variant. HF and CI are integrated as genotype specific meta-information in a Variant Call Format (version 4.0) file;
- the mt-classifier tool, for haplogroup prediction, mt variant functional annotation and prioritization.


The MToolBox development and manteinance relies on the work of undegraduates, PhD and Postdocs, which we would like to thank for their invaluable support:
- [Claudia Calabrese](https://github.com/clody23)
- [Domenico Simone](https://github.com/domenico-simone)
- [Mariangela Diroma](https://github.com/ma-diroma)
- [Roberto Preste](https://github.com/robertopreste)
- [Rosanna Clima](https://github.com/Ros85)
- Mariangela Santorsola
- Ornella Vitale
- Cristiano Gutta' (past)
- Francesco Rubino (past)

We would also like to thank Professor Marcella Attimonelli (University of Bari), who inspired and supervises the MToolBox project.

**As of February 2019**

A bug in the phylotree build 17 tree parsing has been fixed, causing replacement of `haplogroups.txt` and `phylotree_r17.pickle` files. The bug was causing wrong predictions mostly for X haplogroups. Please update your MToolBox installation with `git pull`.


**As of April 2018**    
Update to MToolBox v.1.1

Update of the [Sitevar nucleotide variability](http://www.hmtdb.uniba.it/siteVariability). The nucleotide variability of each variant site was estimated on the multi-alignment of 30,860 healthy genomes reported in [HmtDB](http://www.hmtdb.uniba.it/hmdb/). These genomes were derived from primary INSDC databases and individual submissions. Credits to [Rosanna Clima](https://github.com/Ros85) and Ornella Vitale. 

for more details please check the changelog file.

**As of 24 October 2017**    

MToolBox can be now also installed on Mac OS X by specifing `-o` in the `install.sh` command line. For further details please visit:
[MToolBox installation](https://github.com/mitoNGS/MToolBox/wiki/Installation). Credits to [Roberto Preste](https://github.com/robertopreste).


**As of 11 December 2016**

`GenomeAnalysisTK.jar` has been removed from the `MToolBox/ext_tools` directory.  
Users that would like to run GATK IndelRealigner are now asked to download a newer version of GATK and place it in the
`MToolBox/ext_tools` folder:

```
mv GenomeAnalysisTK.jar /path/to/MToolBox/MToolBox/ext_tools/
```

**Please keep an eye on the MToolBox updates (and do git pull from time to time) by reading the changelogs. To do so please visit [changelogs](https://github.com/mitoNGS/MToolBox/blob/master/changelog.md).**

####For the previous version of MToolBox (v.0.3.3), please go to https://github.com/mitoNGS/MToolBox/releases. (DEPRECATED)

####For further information, please visit the official [MToolBox Wiki](https://github.com/mitoNGS/MToolBox/wiki).

