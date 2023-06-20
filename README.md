# ihccBMI_PRS
Trans-ethnic Polygenic Risk Scores for Body Mass Index: An International Hundred K+ Cohorts Consortium Study

Generating individual risk scores using LDpred

Required input-
Plink binary files (.bed .bim .fam) containing the genotypes of samples to score

Input File Formats-

For the .fam files, sex cannot be left blank in column 5. A phenotype is also required in column 6
For the .bim files, rsids are required (not chr:pos) in col2 and dbgap allele encodings (A,C,T,G) in cols 5,6

Running LDpred-
	
ldpred score --gf Human610-Quadv1HRC.rsid.bmi --rf EUR-Locke-BMI-HH3.weight --out EUR-LOK-BMI-score --pf Human610-Quadv1HRC.rsid.bmi.fam  --pf-format FAM --rf-format LDPRED --summary-file predictions-eur-bmi


Additional details can be found in the file “instructionsIRS-LDpred-v4PatrickMSleiman.docx”.

The link to the published paper: https://onlinelibrary.wiley.com/doi/full/10.1002/ctm2.1291 
