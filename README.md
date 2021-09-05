# Calc-Trancripts-Relative-Gaps
Computational Biology Final Project - Python Script to Calculate Transcripts
This script calculates transcripts using the output of genomecov.
Usage: python3 calcTranscriptsRelativeGaps.py [genomecov results] [output file] [min coverage # per tanscript] [max gap length]
The script parses each line, and checks the coverage for each base in the genome.
The current peak is saved for each transcript, and the gap is calculated to be 5% of the current peak (or keeps the minimun coverage, the greater of the two).
After passing the allowed number of gaps, the transcript is cut and appended to the results.
Output: an output file with bed format: Chr, Start, End.
