# Creating BioApp using Machine learning to make Prediction for the Targeted Protein of our Interest
Pre-process biological activity data from the ChEMBL database that you can use to perform Computational Drug Discovery.
The dataset is comprised of compounds (molecules) that have been biologically tested for their activity towards target organism/protein of interest.

Then use the SMILES notation (representing the unique chemical structure of compounds) to compute molecular descriptors.
The descriptors that we will be computing are the Lipinski's descriptors (molecular weight, LogP, number of hydrogen bond donors and number of hydrogen bond acceptors).
Finally we will then perform exploratory data analysis by making simple box plots and scatter plots to discern differences of the active and inactive sets of compounds.

In the next step, I have made some changes to the target protein to be Acetylcholinesterase as it provides a larger dataset to work with.
We have already computed the molecular descriptors using the PADEL-Descriptor software and prepare the dataset (X and Y dataframes) that will be used in this video for Model Building.
in further process, build a regression model for predicting the pIC50 values (the Y variable).

After review the structures, build and compare several regression models (quantitative structure-activity relationship or QSAR) of the Acetylcholinesterase inhibitors using the lazypredict library in Python.

Finally in last process, deploy the machine learning model as a web app. Essentially, this web app will serve as a Bioinformatics tool that will allow users the ability to predict whether a compound of interest has favorable biological activity against the target protein or not.
