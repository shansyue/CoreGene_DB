## Main Direction :

genomes -> BLASTp on Linux ->  many BLASTp reports ( includes similarity, e-value, % overlapping ... to define "similar" )

->

get .txt from BLASTp -> store in MySQL -> new score ( based on BLAST report ) to summary in DB ( MCL paper ) -> 
-> get similar gene ( core gene candidate, use DEG to validate ) -> get core gene -> GUI webpage oriented to find core gene 

## Webpage Spec :

### input :

e-value, scores, % overlapping ...

DNA seq needed to be compared with 

### output :

core gene



