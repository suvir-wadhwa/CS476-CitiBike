
# Citi Bike Ridership Analysis

Overview

This project analyzes the Citi Bike ridership data for the years 2019 and 2023. The analysis aims to understand the changes in ridership patterns, popular stations, membership distributions, and trip durations, before and after COVID-19.
Directory Structure:

project_root/
│
├── src/
│   └── CitiBikeAnalysis.scala  # Main Scala script for analysis
│
└── data/
    ├── 201809-citibike-tripdata.csv  # Data for 2019
    └── JC-202309-citibike-tripdata.csv  # Data for 2023

Prerequisites:
	  Apache Spark installed and configured.
	  Access to HDFS (Hadoop Distributed File System).
	  Input data files placed in the specified HDFS directory.

How to Build:

The Scala script can be compiled using SBT or directly run in the Spark shell. Ensure that Spark is properly set up in your environment.

How to Run:
		Start the Spark Shell: spark-shell   
		Load the Scala script in the Spark shell:  load CitiBikeAnalysis.scala   
		The script will automatically execute the analysis once loaded.
  
Input Data:
	  The 2019 dataset is located at hdfs:///user/sw4854_nyu_edu/201809-citibike-tripdata.csv.
	  The 2023 dataset is located at hdfs:///user/sw4854_nyu_edu/JC-202309-citibike-tripdata.csv.
 
Running the Code:
The main script CitiBikeAnalysis.scala performs the following analyses:
		Data loading and cleaning.
		Basic data profiling.
		Count of rides per year.
		Analysis of most popular stations.
		Membership type distribution.
		Analysis of trip durations.
		Time-based analysis (distribution of rides across different hours).

  
Run each section of the script step-by-step in the Spark shell.

 
Results:

The results of the analysis are displayed in the Spark shell console. They include statistical summaries, counts, and other relevant information derived from the data.

Access to HDFS Files:
	  Use permissions to access the HDFS paths provided.
	  Use Hadoop commands to access or inspect the data files, for example:
	  hdfs dfs -ls /user/sw4854_nyu_edu/   
