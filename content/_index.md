---
title: "Maize TE Annotations"
featured_image: '/images/darkcorn.jpg'
description: "Structural transposable element (TE) annotation of multiple maize genomes"
---

# TEs along a region of the genome:
We reconstruct the history of TEs nesting into each other. 
For example, the blue TE on the left inserted first, and then was disrupted by the insertion of green and yellow TEs.

![Dooner-style depiction of 8 TE copies](/maize_TEs/images/dooner_style.png)

#### We have reconstructed this history of transposition, using methods described in [Jiao et al., 2017](https://www.nature.com/articles/nature22971) and a forthcoming manuscript. 

The linked files provide updated TIR, soloLTR, and LINE searches, which better identify matched target site duplications (TSDs) and terminal inverted repeats (where applicable).

We suggest using a version of the annotation that fits your needs, here the *full-length TE* and *disjoined TE* versions.

--------------

The *full-length TE* gff3 version is useful for counting the number of TEs in the genome, or for assessing the presence/absence of a copy based on split read and read pair approaches. Each bar here is represented as a separate gff3 line.
![8 TEs along the genome](/maize_TEs/images/allTE.png)

B73: [`B73.structuralTEv2.fulllength.gff3.gz`](https://github.com/mcstitzer/maize_TEs/blob/master/B73.structuralTEv2.fulllength.2018-09-19.gff3.gz)

W22: [`W22.structuralTEv2.fulllength.gff3.gz`](https://github.com/mcstitzer/maize_TEs/blob/master/W22.structuralTEv2.fulllength.2018-09-12.gff3.gz)

PH207: [`PH207.structuralTEv2.fulllength.gff3.gz`](https://github.com/mcstitzer/maize_TEs/blob/master/PH207.structuralTEv2.fulllength.2018-10-15.gff3.gz)

Mo17: [`Mo17.structuralTEv2.fulllength.gff3.gz`](https://github.com/mcstitzer/maize_TEs/blob/master/Mo17.structuralTEv2.fulllength.2018-12-11.gff3.gz)

--------------
The *disjoined TE* gff3 version is useful for mapping reads and assigning each to a TE. 
Each base pair in the genome is assigned to only one TE copy, that which brought the sequence into the genome. 
Fragments of individual copies can be reunited by their shared TE identifier (see below). 

![8 TEs along the genome](/maize_TEs/images/disjoined.png)

B73: [`B73.structuralTEv2.disjoined.gff3.gz`](https://github.com/mcstitzer/maize_TEs/blob/master/B73.structuralTEv2.disjoined.2018-09-19.gff3.gz)

W22: [`W22.structuralTEv2.disjoined.gff3.gz`](https://github.com/mcstitzer/maize_TEs/blob/master/W22.structuralTEv2.disjoined.2018-09-22.gff3.gz)

PH207: [`PH207.structuralTEv2.disjoined.gff3.gz`](https://github.com/mcstitzer/maize_TEs/blob/master/PH207.structuralTEv2.disjoined.2018-10-15.gff3.gz)

Mo17: [`Mo17.structuralTEv2.disjoined.gff3.gz`](https://github.com/mcstitzer/maize_TEs/blob/master/Mo17.structuralTEv2.disjoined.2018-12-11.gff3.gz)

------------------

<div style="text-align: left">
We name each TE copy with a unique identifier, that contains information about the TE superfamily, TE family, and specific TE copy.
</div>


<span style="color:blue">DTA</span><span style="color:red">00001</span><span style="color:purple">Zm00001d</span><span style="color:turquoise">00001</span>

- <span style="color:blue"> DTA </span>: Superfamily, codes from [Wicker et al., 2007](https://www.nature.com/articles/nrg2165)

- <span style="color:red">00001</span>: Family number (For TIR elements, these match numbers assigned in MTEC of v1 of the maize genome, see _Legacy Annotations_ below)

- <span style="color:blue">DTA</span><span style="color:red">00001</span>: Together, these then define the family name

- <span style="color:purple">Zm00001d</span>: Assembly version code for the reference genome, as assigned by the [Maize Genetics Nomenclature Committee](https://www.maizegdb.org/nomenclature)

- <span style="color:turquoise">00001</span>: Copy ID number, unique to this copy in the genome. For disjoined copies, each line in the gff3 file contains this ID

---------------

#### _Legacy Annotations_

Original TE annotations from the publications of B73 ([Jiao et al., 2017](https://www.nature.com/articles/nature22971)) and W22 ([Springer et al., 2018](https://www.nature.com/articles/s41588-018-0158-0)) can be found here:

B73: [`B73v4.TE.filtered.gff3.gz`](ftp://ftp.gramene.org/pub/gramene/CURRENT_RELEASE/gff3/zea_mays/repeat_annotation/B73v4.TE.filtered.gff3.gz)

W22: [`W22.allTE.withSolo_10Jan18.gff3.gz`](https://ftp.maizegdb.org/MaizeGDB/FTP/W22_v2.0/W22.allTE.withSolo_10Jan18.gff3.gz)

Consensus and exemplar TEs from the Maize TE Consortium (MTEC) as published in [Schnable et al., 2009](http://science.sciencemag.org/content/326/5956/1112.full) and [Baucom et al., 2009](https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1000732), previously available at [maizetedb.org](http://www.maizetedb.org) (link broken as of September 2018) are available here:

[`TE_12-Feb-2015_15-35.fa`](https://github.com/mcstitzer/dawe_ab10_kindr/blob/master/identify_haplotypes/te_alignments/TE_12-Feb-2015_15-35.fa)

