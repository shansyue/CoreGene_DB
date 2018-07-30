## MCODE - Cluster Finding Algorithm

## STEP 1. Node Scoring

- Assigns higher scores to nodes whose immediate neighbors are most interconnected.

- For each node :

  (1) Get the immediate neighbors of a node to score.

  (2) Find the highest K-Core network.

  (3) Calculate the Core Density. ( = edges / possible edges aka (# nodes)^2 )

  (4) Score the node. ( = K * Core Density )


## STEP 2. Cluster Finding

- Find a complex with the highest-scored node and recursively move outward from it as seed, 
including nodes whose scores are above a given threshold.

- Threshold = ( 1.0 - Node Score Cutoff ) * ( Score of Seed Node )
  // Bigger node score cutoff -> Bigger clusters

  (1) Find the max score as a seed.
  
  (2) Find a cluster.

- This step are repeated and then the clusters are filtered out that don't contain at least K-core networks.

- K-Core Filtering : 

removes clusters that do not contain at least K-Core network.


## STEP 3. Post-Processing

- Process haircut and fluff.

- Haircut : 

removes all singly-connected nodes from each cluster.

- Fluff :

expands cluster cores by one neighbor shell outwards according to a Density Cutoff.


## STEP 4. Cluster Scoring

- Cluster Score = nodes * density = nodes * ( edges / possible edges )

