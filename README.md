# Distributed Systems and Cloud Computing [CLOUDS]
This repository contains my project notebooks for the Distributed Systems and Cloud Computing course at EURECOM.

### Course abstract
The goal of this course is to provide a comprehensive view on recent topics and trends in distributed systems and cloud computing. We will discuss the software techniques employed to construct and program reliable, highly-scalable systems. We will also cover architecture design of modern datacenters that constitute a central topic of the cloud computing paradigm. The course is complemented by a number of lab sessions to the design of scalable algorithms and get hands-on experience with Apache Spark.

***
## Notebooks
### [Introduction](https://)
<img align="right" src="images/intro_img.png" width="300">
* The aim of this introductory lab is to:
* Gain familiarity with Juypter Notebooks
* Acquire basic knowledge about Python: Pandas, Matplotlib, Numpy
* Gain familiarity with the PySpark and how to interact with the HDFS
* Gain hands-on experience with two distributed codes: 
   * word count 
   * analysis of night flights


The aim of this introductory lab is to get familiar with
   the Jupyter notebooks, 
   python and its modules (Pandas, Matplotlib, Numpy). 
   PySpark and how to interact with the HDFS, together with two examples of distributed code: word count and an analysis of night flights.

### [Gradient Descent](https://)
<p align="center">
<img src="images/sgd_img.png" width="640">
</p>

This notebook contains multiple implementations of the gradient descent algorithm. At first, the results obtained using the scipy library are observed, then the algorithm is compared with a numpy implementation of batch gradient descent.

Furthermore, stochastic gradient descent and mini-batch stocastic gradient descent are implemented and compared with the previous one. A deep analysis is performed regarding how each algorithm's results change with parameters such as the learning rate and the number of iterations.

Finally, a distributed version of mini-batch gradient descent is implemented using PySpark and its followed by an analysis of the performance of all the algorithms in terms of dataset size.

### [k-Means](https:)
<img align="right" src="images/kmeans_img.png" width="300">

As for the previous notebook, this one starts by analyzing the k-means algorithm and its implementation, then it is tested on a generated 2D dataset to have better visualization and it is compared with the sklearn implementation.

An analysis of convergence of datasets of different shapes underlines the important of centroids initialization and introduces the k-means++ technique for smart centroid initialization that is implemented too. Moreover, the elbow method to find the optimal value of the number of clusters is discussed and implemented.

Finally, a distributed version of k-means is implemented with PySpark, the new algorithm is analyzed and compared with the serial implementation.

### [Flights Data Analysis](https:)
<img align="left" src="images/flights_img.png" width="300">

The last notebook introduces the DataFrame API and its advantages with respèct to RDDs, then, DataFrames are built starting from a structured file and from an RDD.

This section is followed by the analysis of flights data using SparkSQL. Data exploration is divided in three main sections: basic queries, flight volume statistics and additional queries. Data visualization is performed using the seaborn module.

The notebook ends with a bonus question regarding the analysis of other datasets and their relation with the used one.

***
## Course Notes
Here follows a simplified table of contents of my notes for the CLOUDS course.

 * Scalable Algorithm Design 
   * Introduction
   * Key Principles
   * The Programming Model
   * Basic Design Patterns
 * Hadoop Internals
   * Hadoop Distributed File System
   * Hadoop MapReduce
 * Apache Spark Internals
   * Introduction and Motivations
   * Anatomy of a Spark Application
   * Spark Deployments
   * Resilient Distributed Datasets
   * Spark Word Count
 * Cluster Schedulers
   * Cluster Scheduling Principles
   * Taxonomy of Scheduling Design
   * Schedulers Architectures
   * YARN
   * MESOS
   * BORG
 * SparkSQL
   * Relational Algebra
   * DataSource and DataFrame API
   * SparkSQL Architecture
 * Distributed Storage Systems
   * The CAP Theorem
   * Amazon Dynamo
   * Apache HBase
   * Apache Cassandra
 * Coordinating Distributed Systems
   * Two-phase Commit
   * Paxos
   * Raft
   * Zoe and ZooKeeper 
