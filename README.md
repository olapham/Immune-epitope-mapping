# Immune-epitope-mapping

The script produces a polypeptide sequence for testing. You have to input a peptide file and a csv file containing immunogenic peptides from IEBD.

The way to execute the script is to:

1. Get all of the files attached to this email into the same directory (folder) on your computer. It can be any folder.

2. Open your Mac terminal app

3. In the terminal, navigate to the directory containing the files using the cd command. Eg, if the files were on my desktop I’d type
cd /Users/johncounsell/Desktop

4. Now you can instruct the system to run the script on the input files and create an output sequence, by entering the command
python Immune_epitope_map.py -i1 bole1a.fa -i2 epitope_table_export_1675018680.csv -n1 50 -n2 1000 -o1 bole1a_hits_1w.csv -o2 bole1a_Tcell_polypeptide.fa
 
This will create a file containing a polypeptide consisting of the regions with greatest density of immunogenic peptides. You can choose how many windows you split your query sequence into. In the example above I split it into 50 (the number after -n1). You can also choose how long you want it to be. In the example above I chose 1000 amino acids length (the number after -n2)
