# Run-Experiments
---

## General Idea  :

Run Experiments is a Java Class used to automatically run different information retrieval Experiments Automatically based on different input variables in different XML Files. In addition , It accepts a range of values to run Ex : BRange = 1:10:2 >>> will run 5 experiments of B (1,3,5,7,9).

Read the attached pdf for details 
[here](https://github.com/ABDULAZIZALQATAN/Run-Experiments/issues/10)
 
## Input & Output

### Input Parameters :
The Main input parameters are :
* Experiment parameter files . (used to identify the values for each experiment run)
* Indexes ( It is preferable to create the index using IndexerApp from https://github.com/lucene4ir/lucene4ir/blob/master/README.md __in order to match token filters with the run experiments__
* Query Files
* Qrel Files
* Token Filters . Token Filters used for creating the index and retrieval experiment should be the same


### Output Results :

![Output Explanation](https://user-images.githubusercontent.com/47518534/56103304-0c3b7880-5f2a-11e9-8080-4f2cf65f32bd.jpg
 "Output Explanation")
 
* Bash Scripts : a generated file that includes trec_eval commands for all experiments grouped by experiment file
![Bash Scripts](https://user-images.githubusercontent.com/47518534/56102807-4e16ef80-5f27-11e9-8ae0-aa5654ea6601.jpg
 "Bash Scripts")
* Params : list of XML parameter files generated to be passed to RetrievalApp from [Lucene4Air](https://github.com/lucene4ir/lucene4ir/blob/master/README.md)
![Retrieval Parameters](https://user-images.githubusercontent.com/47518534/56102458-21fa6f00-5f25-11e9-9f22-22c262707e2b.jpg
 "Retrieval Parameters")
 
 * Performance : list of files that contain trec_eval results for each experiment 
 ![Performance](https://user-images.githubusercontent.com/47518534/56102506-4d7d5980-5f25-11e9-80be-42ab9df27853.jpg
 "Performance")
 
 * Results : result files the contain the results of running RetrievaApp for each experiment
  ![Results](https://user-images.githubusercontent.com/47518534/56102453-1444e980-5f25-11e9-87cb-fa1f41f963ea.jpg
 "Results")
 * Rertrieval Scripts : Java Scripts used to directly run RetrievalApp class using its associated retrieval parameter File
   ![Rertrieval Scripts](https://user-images.githubusercontent.com/47518534/56102493-3dfe1080-5f25-11e9-9424-2cab6e9ad6cf.jpg
 "Rertrieval Scripts")
