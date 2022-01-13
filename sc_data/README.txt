README for sc_data folder

howick_tryps_sce.rds is the RDS file with SC3 analysis run on 388 single-cell transcriptomes collected from tsetse fly. It includes cell meta data (also found in coldata_howick_tryps_sce.csv) with the following columns

sample_id - sample name and column name in expression matrix
npgnum - associated with cram files along with run_num (run number)
tag, library - tag and library index from nexteraXT prep
top_map, second_map, top_mapreads, second_mapreads - output from automated blast analysis done by Sanger core pipelines.
run_number - the run number  and lane associated with sequencing run.
ShortenedLifeStage - Tissue of isolation
attachment - free (allowed to swim out) vs attached (from disassociated SG tissue)
Strain - 1738 or J10
date_sorted - cell sort and cDNA manufacture date
plate_name - sort plate identification
time - day post infection parasites were isolated
COI - complexity of infection single vs cross (coinfection of J10 and 1738)
fixation - live or reagent used
sum - total mapped counts in that cell
detected - number of genes detected in that cell
percent_top_* - QC stats from scater on the precent of reads falling the top * expressed genes
sizeFactor - size factor used for normalisation
sc3* - cluster assignments and outlier scores from SC3 analysis, 6 clusters were used (sc3_6), which are renamed as cluster_name
xfilename and rsemname - used for VSG mapping analysis
assignment status spr_strain - output from Souporcell
cluster_name - cluster assignment name associated with Fig 1
fig1_UMAP* - UMAP coordinates for data in fig 1
logsumg1VSG, detected_g1_VSG - total VSG expression for that cell from fig 2
Pseudotime- pseudotime value from Slingshot
pt_sc3_4_clusters - cluster assignment used for pseudotime analysis
pt_UMAP* - pseudotime UMAP coordinates

rowdata_howick_tryps_sce.csv contains the per gene QC and SC3 output

counts_howick_tryps_sce.csv contains the raw count data 