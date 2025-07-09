# Biocondensate-Heterogeneity
The goal of this project is to group and cluster groups of similar bio condensates together. 

As part of the Saurabh Lab at NYU, I was working closely with PhD and PhD candidates to explore heterogeneity in PopZ proteins in Caulobacter cells. The starting input for this was images and then after using RegionProps, the lab was able to break these images down into CSVs that contained the lifetime of each cell at a particular point in the condensate. Then through more RegionProps feature extraction, I was able to create a tabular dataset containing unique characteristics for each condensate based off of the CSV-image form. After this, these images were then reduced using PCA (Principle Component Analysis) and then clustered using hierarchical clustering. The clustering technique used involved cosine similarity which basically worked by finding the angle (via dot product) between the vectors that were established from the RegionProps feature extraction. This allowed me to group around 65-70 images into different classes.  

Below is a workflow diagram
![Diagram](diagram)


Below is the final product. These are the clusters that the model created.
![cluster_ex](cluster_ex.pdf)
