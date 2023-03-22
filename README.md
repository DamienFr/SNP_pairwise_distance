# DESCRIPTION
Produces a tab delimited file with pairwise distances between pairs of sequences.
Optionaly, computation of specific pairs only can be specified with the -r option.
For each pair, the script's behavior is to search for sequence1 in input file 1 and sequenc e2 in input file 2. if all your sequences are in the same fasta file, you can specify it twice.

# USAGE

Usage: perl Pairwise_SNP_distance_from_fasta -i in.fasta -i2 in.fasta [-r comparisons_to_make.tsv] [-o output_file] [-o2 output_file]

[] means argument is optional

available arguments:

	-i or -input:	fasta file	(REQUIRED)
	-i2 or -input2:	fasta file	(REQUIRED)
	-r or -restrict:	To compute only certain pairwise comparisons, provide a tab delimited file with comparisons to make as rows	(OPTIONAL)
	-o or -out:	Output File	(DEFAULT: [input_name].pairwise_SNP_number.csv)
	-o2 or -out2:	Summarized Output File	(DEFAULT: no summarized output)
	-m or -min:	Min size of each sequence of each pair in order to consider the pair (DEFAULT: no min size of sequence applied)

	-h or -help:	This Documentation

# OUTPUT

- pairwise distance tab file
- summary pairwise distance tab file containing the mean value of all COMPUTED distances

# AUTHOR

Damien Richard, 2023
