# iGEM-modelling

Check out UBC iGEM's website for the work I've done!
https://2025.igem.wiki/ubc-vancouver/biocementing-bacteria/modelling/

Requirements: 
- install nextflow: 
https://www.nextflow.io/docs/latest/install.html
- install docker / singularity / apptainer 
(depends on which one you use, modify the line -profile accordingly)
- install pymol
- To run alphafold part of the script, need 12 GB RAM 

Workflow:
all fasta files -> a csv file -> alphafold -> pdb files of individal fasta file -> pymol structural alignment -> .txt files 
- alphafold results and .txt files are saved to output directory

Running the script: 
- put all the fasta files in the parent folder, make sure the naming doesn't contain special character, underscore is allowed
- add name + path of the fasta files to the line that creates the csv file
- Run: nextflow run af_pymol.nf

