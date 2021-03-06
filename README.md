# Evolution and rapid spread of a reassortant A(H3N2) virus that predominated the 2017-2018 influenza season

#### Barney I. Potter<sup>1</sup>, Rebecca Garten<sup>2</sup>, James Hadfield<sup>1</sup>, John Huddleston<sup>1,3</sup>, John Barnes<sup>2</sup>, Thomas Rowe<sup>2</sup>, Lizheng Guo<sup>2</sup>, Xiyan Xu<sup>2</sup>, Richard A. Neher.<sup>4,5</sup>, Trevor Bedford<sup>1</sup>, and David E. Wentworth<sup>2</sup>

<sup>1</sup>Vaccine and Infectious Disease Division, Fred Hutchinson Cancer Research Center, Seattle, WA, USA, <sup>2</sup>Virology Surveillance and Diagnosis Branch, Influenza Division, National Center for Immunization and Respiratory Diseases (NCIRD), Centers for Disease Control and Prevention (CDC), Atlanta, Georgia, USA, <sup>3</sup>Molecular and Cellular Biology program, University of Washington, Seattle, WA, USA, <sup>4</sup>Biozentrum, University of Basel, Switzerland, <sup>5</sup>SIB Swiss Institute of Bioinformatics, Basel, Switzerland

## Abstract
The 2017-2018 North American influenza season caused more hospitalizations and deaths than any year since the 2009 H1N1 pandemic.
The majority of recorded influenza infections were caused by A(H3N2) viruses, with most of the virus's North American diversity falling into the A2 clade.
Within A2, we observe a subclade which we call A2/re that rose to comprise almost 70\% of A(H3N2) viruses circulating in North America by early 2018.
Unlike most fast-growing clades, however, A2/re contains no amino acid substitutions in the hemagglutinin (HA) segment.
Moreover, HI assays did not suggest substantial antigenic differences between A2/re viruses and viruses sampled during the 2016-2017 season.
Rather, we observe that the A2/re clade was the result of a reassortment event that occurred in late 2016 or early 2017 and involved the combination of the HA and PB1 segments of an A2 virus with neuraminidase (NA) and other segments a virus from the clade A1b.
The success of this clade shows the need for antigenic analysis that targets NA in addition to HA.
Our results illustrate the potential for non-HA drivers of viral success and necessitate the need for more thorough tracking of full viral genomes to better understand the dynamics of influenza epidemics.

## Analyses
For this analysis, we manage software requirements using [conda](https://conda.readthedocs.io/en/latest/), a package manager that supports independent environments.
For the bulk of this analysis, we use tools from the [Nextstrain](nextstrain.org) platform.

### Install requirements
1. Install Conda and ensure that the installation was successful.
2. Download this repo:
```
git clone https://github.com/blab/h3n2-reassortment.git
cd h3n2-reassortment
conda create -f h3n2_reassortment.yaml
conda activate h3n2_reassortment
```
3. Clone nextstrain componenets:
```
git clone https://github.com/nextstrain/fauna.git
git clone https://github.com/nextstrain/augur.git
git clone https://github.com/auspice.git
```
4. Download sequence data from [GISAID Epiflu](https://www.gisaid.org/) database according to instructions [here](https://github.com/nextstrain/fauna/blob/master/builds/FLU.md#upload-documents-to-vdb).
Sequences were prepared for processing using the [fauna](https://github.com/nextstrain/fauna/blob/master/builds/FLU.md#upload-documents-to-vdb) pipeline.
A full list of accessions used in this analysis after being processed by fauna can be found [here](data/analysis_references.tsv)

## Citation

[Potter BI, Garten R, Hadfield J, Huddleston J, Barnes J, Rowe T, Guo L, Xu X, Neher RA, Bedford T, Wentworth D 2019. Evolution and rapid spread of a reassortant A(H3N2) virus that predominated the 2017-2018 influenza season. bioRxiv: 543322..](https://doi.org/10.1101/543322)
