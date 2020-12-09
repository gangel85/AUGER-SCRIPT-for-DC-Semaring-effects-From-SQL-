Files utilized for the creation of different smearing values for Drift Chambers, so to compare Monte Carlo simulations to the Data.

How to : 
1)Define a local copy of the sqlite calibtations files (test.sqlite) .

2) Dump the table of the doca_smearing for drift chamber into a txt file 

3) Replace the column containing the smearing values.

2) Replace the smearing values located in  database : /calibration/dc/signal_geneeration/doca_smearing 

3) cdb -c sqlite:///test.sqlite vers /calibration/dc/signal_generation/doca_smearing

4) setenv CCDB_CONNECTIONsqlite:///PATH/test.sqlite

Once the env variable is set to the proper sqlite file,  submit the Auger Script to the JLAB cluster machine.


jsub Smearing.clasdis 

The path of the simulated Monte Carlo files can be changed in the Smearing.clasdis script.


The Simulation version used in the auger script is 4.4.1 [ End of 2020]  
