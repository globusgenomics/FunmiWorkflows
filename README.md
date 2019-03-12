# FunmiWorkflows
Swift based workflows for Convarcal analysis


ConVarCal workflows on Globus Genomics

1. Alignment 
    PRODUCTION-Color_BWA-MEM+BQSR_Globus-transfer-and-alignment-only

2. SNV and indel calling
    PRODUCTION_Atlas-SNP2_Swift_BEDFilterTrim_MasterSiteList
    PRODUCTION_Atlas-Indel2_Swift_BEDdefault_MasterSiteList
    PRODUCTION_FreeBayes_Swift_by_BEDWindowSize
    PRODUCTION_GATKv3.8_HaplotypeCaller_Swift_BEDdefault_VQSR
    PRODUCTION_Platypus_v0.8.1
    PRODUCTION_SAMtools_mpileup_Swift_by_BEDWindowSize

3. SNV and indel merging and intersection; outputs from Step2 above are MANUALLY put together in a history before executing Consensus Genotyper
    PRODUCTION_5Sets_Consensus_Genotyper

4. SV calling; multiple SV callers, a consensus intersection tool, and IGV screenshot, are organized in a single workflow
    PRODUCTION_ConVarCal_SV_BEDfilter_PostProcessing
