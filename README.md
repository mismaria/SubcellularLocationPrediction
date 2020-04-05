# PREDICTION OF PROTEIN SUBCELLULAR LOCALIZATION

## Overview
An exploration of different models, concluding to an NuSVC (Nu-Support Vector Classification) model with optimised parameter nu=0.18, and then fitting it to an OneVsRestClassifier. 
The model was trained on a dataset which counts 9222 proteins. 

## Author
Maria Miscouridou, UCL

## Protein data

Training and cross-validation is performed on 4 files:
    1) 'cyto.fasta.txt'
    2) 'mito.fasta.txt'
    3) 'nucleus.fasta.txt'
    4) 'secreted.fasta.txt'
    
The final testing is performed on:
    1) 'blind.fasta.txt'

Each file includes proteins sequences in fasta format.


## Further testing

If you want to test the model on further sequences:
    1) make sure the sequences are in fasta format
    (https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=BlastHelp)
    2) include the file in the same subfolder as the code
    3) change only the filename at the point when the code reads the file 

## Dependencies
The following modules need to be installed (with the 'pip install' command:
    1) biopython
    2) pandas
