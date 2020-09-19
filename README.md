# Skoltech-Microbiome-Project
Microbiome cluster analyses and low-dimensional representation

folders AGP, ibd, ptb and t2d containing the pivot tables for each database. The name of the folder is the database identificator

Python notebooks are the following:  
1.Final_merge.ipynb is for merging the pivot tables from the database folders into pivot_ .csv tables, one for each O, F and G taxonomic level  
2.PCA.ipynb is for Principal Components projection, producing proj_ csv tables  
3.Intristic_dim_estimation.ipynb is for MLE algorithm of the intristic dimension estimation, providing diagrams for the apriori dimension and neighborhood estimation  
4.Manifold_learning.ipynb is for Isomap, LLE, modified LLE embeddings of the PCA projected data. Parameters are taken near values from previous diagrams  
5.Regresion_inverse_knn.ipynb is for the inverse mapping from the Isomap projected data to the PC space. Wide range of dimensions for the Isomap images are calculated  
6.Reconstruction_knn_pca.ipynb is for the comparision of the errors for the PCA inverse transform after the inverse mapping. Mean average error is the criteria  
7.Clustering.ipynb is for DBScan, K-means and Spectral clustering. Silhouette score and the DBI are the performance criteria. Isomap and PCA data compared  
8.Projections_2d_3d.ipynb is for the 2D and 3D coordinate projections of the Isomap image  
9.TSNE_color_databases.ipynb is for t-SNE visualization in 2D and 3D, different parameters compared. Each database has a different color  
10.UMAP_o.ipynb is for UMAP visualization for 2D and 3D. Each database has a different color  
11.NCVis_o.ipynb is for 2D NCVis visualization. Each database has a different color  

It is advised to compute them in the same order as mentioned above  

All the generated .csv files are stored in the current repository in the case to perform the future computational experiments without recalculating the whole pipeine  

scripts folder is containing bash scripts to perform the conversion of the .biom files to .csv tables inside all the directories,
splitting these tables into O, F and G levels tables and merging these tables for each database on every chosen taxonomic level  

The original raw data is stored in Google Drive here:  
https://drive.google.com/drive/folders/1GeDPpmVXha88o9Ny3NVjOQfZoPzuWGT6?usp=sharing
(All the databases are also stored here for the cases after the scripts runs, refer to the READ_ME.txt in the link above for more details)  

Presentation with the infographics and the report are stored as the isomap_knn_reconstruction.pdf and report_microbiome.pdf files  
