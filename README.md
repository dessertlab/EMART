# EMART

In this repository, all results obtained in EMART experimentation are collected.
Each folder is coupled with the correspondent Research Question (RQ) as described in the paper.
In the RQ1 and RQ2 folders results in terms of MSE and Variance are organized considering:
-	the true operational profile: profile1, profile2, profile3 and variable profile
-	the error attached to relative estimated profiles: 10%, 90%

In pictures both EMART results and Operational Testing (OT) results are reported.
The RQ3 contains all results of the cost-benefit analysis considering both MSE and Variance.
All considerations on results representation are consistent with what specified in the paper.

In the folder "code", the source code of the EMART engine is available.
To run EMART is necessary to follow some steps:
1. Import the source code in an IDE (like Eclipse).
2. Populate the data structure Test Frame.
3. Define a Weight Matrix to build connections among Test Frames.
4. Set the values of n (number of samples to be selected), and d (a parameter proper of the selection strategy, defined as "r" in the paper)

In addiction, to repeat the experiments is necessary to:
1. Download and run the application defined in the paper as experimental subjects.
2. Generate requests according to a desired profile (defined in the test frame data structure) to the interface of the components.
3. Run a monitoring infrastructure (like Metro Funnel https://github.com/dessertlab/MetroFunnel.git) to collect the methods invocation and update the information in input to the EMART engine.