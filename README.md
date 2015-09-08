B# Corvid phylogeny

## Paths to the data
All the relevant data for this project is stored in or linked in the /home/shyam/projects/corvids/data directory.
The following is data summary from the email that Rute sent out on the 26th of August 2015.

The capture regions are in : 
/home/joseas/data/Birds/NewBait/Corvus_brachyrhynchos_capture.fasta

The references genome:
/home/joseas/data/Birds/NewBait/GenomeBGI/Corbr/*fa

The folders for the first round of sequencing of the corvids are these:
/k/basecalls/20130626_hiseq1b/Project_Corvids/Sample*

The second round of sequencing is in:
/k/basecalls/20140820_hiseq2a/Project_Corvids

The initial assemblies done by Fernando are here:
/home/fpealoza/data/Corvids

The ortholog list for the 48 bird genome paper is stored as: 
orthologs/48birds_ortholog.list

## Additional information from Rute
From Fernando:
> data location: /home/fpealoza/data/Corvids

> The correspondence sample - specie -> Samples.xlsx
> Note: The Sample ’59’ is missing, and the ’ 3' has no specie assigned (NMN2_29451).Here are some results for the corvid assembly.
> The same pipeline used to analyze the hummingbirds data was used.

> Raw assemblies:  /home/fpealoza/data/Corvids/6_assembly_soap/*/*k63.fa
> Scaffolds >= 200 bp: /home/fpealoza/data/Corvids/6_assembly_soap/*/*k63.200.fa
> Scaffolds that aligned against the reference: (capture regions) /home/fpealoza/data/Corvids/6_assembly_soap/*/K63/Corvids.Filtered_lastz.fa
> Alignment (each dataset vs capture regions - pairwise ): /home/fpealoza/data/Corvids/7_lastz/pair_maf_k63/*
> Alignment (all samples - multi): /home/fpealoza/data/Corvids/7_lastz/all_samples.63.maf

From Jon Fjeldsa:
> For rooting, you should use Pitta as sister to the rest.

From David:
> NMN2-29451 is a Philesturnus and Cap_index_5 should be the index. 

Directly from Rute's email:
> The attached files:
> - allInfo*: this is all the information I have gathered regarding this project
> - trees done with the initial dataset
> - info on coverage per target of the initial assemblies

> The steps towards the assembly (Cai did the lastz + chainNet step):

> 1) The adapters were removed with CUTADAPT [1] and the reads were quality trimmed/filtered with PRINSEQ [2].
> 2) The overlapping read pairs were merged (FLASH ).
> 3) SOAPdenovo [3] was used to assemble the reads, k-mer = 63.
> 4) The contigs for each sample were aligned against the reference exons and the best hit for each exon was selected. For this lastz + chainNet was used. Removed exons that covered less than 50% of the reference.
> 5) Exons were grouped per gene and multiple sequence alignments (MSAs) were generated with mafft-linsi [4].

> The ortholog list for the 48 bird genome paper (all supp in up on dir, should be useful for comparison with all other birds if you want):
> ftp://climb.genomics.cn/pub/10.5524/100001_101000/101000/48birds_ortholog.list

___


