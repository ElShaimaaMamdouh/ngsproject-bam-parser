# ngsproject-bam-parser
The aim is to detect and report loci of supplementary reads found in a bam file
Drosophila meanogaster is the organism used

References:
https://www.ncbi.nlm.nih.gov/pubmed/29619822
  J Agric Food Chem. 2018 Apr 18;66(15):3737-3753. doi: 10.1021/acs.jafc.7b05900. Epub 2018 Apr 5.
  Drosophila melanogaster as a Versatile Model Organism in Food and Nutrition Research.
  Staats S1, Lüersen K1, Wagner AE2, Rimbach G1.
  
https://www.frontiersin.org/articles/10.3389/fgene.2019.00051/full
   Front. Genet., 01 March 2019 | https://doi.org/10.3389/fgene.2019.00051
   Drosophila melanogaster: A Model Organism to Study Cancer
   Zhasmine Mirzoyan1, Manuela Sollazzo2, Mariateresa Allocca1, Alice Maria Valenza3, Daniela Grifoni2 and Paola Bellosta1,2,3,4*
  
https://www.ncbi.nlm.nih.gov/genome?term=vih&cmd=DetailsSearch
(all genomic files for download)
  
https://science.sciencemag.org/content/287/5461/2185
  The Genome Sequence of Drosophila melanogaster
  Mark D. Adams1,*,et al.
  Science  24 Mar 2000:Vol. 287, Issue 5461, pp. 2185-2195
  DOI: 10.1126/science.287.5461.2185 
  
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3032934/  
  Genome Res. 2011 Feb; 21(2): 315–324.
  doi: 10.1101/gr.107854.110
  PMCID: PMC3032934
  PMID: 21177959
  The Drosophila melanogaster transcriptome by paired-end RNA sequencing
  Bryce Daines,Hui Wang,Liguo Wang,Yumei Li,Yi Han,David Emmert,William Gelbart, Xia Wang, Wei Li,ichard Gibbs, and Rui Chen


###########################################################################
#screen output from fastqc
##FastQC	0.11.8
#Basic Statistics	pass
#Measure	Value
#Filename	SRR8878057.fastq
#File type	Conventional base calls
#Encoding	Sanger / Illumina 1.9
#Total Sequences	18257083
#Sequences flagged as poor quality	0
#Sequence length	49
#%GC	47
#############################################################################################################################
#screen output from indexing
index [bwa_index] Pack FASTA... 1.67 sec
[bwa_index] Construct BWT for the packed sequence...
[BWTIncCreate] textLength=204385202, availableWord=26381084
[BWTIncConstructFromPacked] 10 iterations done. 43516610 characters processed.
[BWTIncConstructFromPacked] 20 iterations done. 80392946 characters processed.
[BWTIncConstructFromPacked] 30 iterations done. 113164658 characters processed.
[BWTIncConstructFromPacked] 40 iterations done. 142288210 characters processed.
[BWTIncConstructFromPacked] 50 iterations done. 168169266 characters processed.
[BWTIncConstructFromPacked] 60 iterations done. 191168370 characters processed.
[bwt_gen] Finished constructing BWT in 67 iterations.
[bwa_index] 97.94 seconds elapse.
[bwa_index] Update BWT... 1.60 sec
[bwa_index] Pack forward-only FASTA... 1.13 sec
[bwa_index] Construct SA from BWT and Occ... 43.84 sec
[main] Version: 0.7.17-r1188
[main] CMD: bwa index -a bwtsw dmel-all-gene-r6.27.fasta
[main] Real time: 149.253 sec; CPU: 146.179 sec
#############################################################################################################################
#screen outout from alignment
[main] Real time: 2803.426 sec; CPU: 2846.461 sec
	Command being timed: "bwa mem bwa_index/dmel-all-gene-r6.27.fasta /home/elshaimaa/NGS_Proj/SRR8878057.fastq"
	User time (seconds): 2828.51
	System time (seconds): 17.96
	Percent of CPU this job got: 101%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 46:43.44
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 501460
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 751606
	Voluntary context switches: 436659
	Involuntary context switches: 269098
	Swaps: 0
	File system inputs: 7907984
	File system outputs: 6647344
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
Exit status: 0
