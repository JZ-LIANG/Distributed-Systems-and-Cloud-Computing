# Distributed Systems and Cloud Computing [CLOUDS]
This repository contains my project notebooks for the Distributed Systems and Cloud Computing course at EURECOM.

### Course abstract
The goal of this course is to provide a comprehensive view on recent topics and trends in distributed systems and cloud computing. We will discuss the software techniques employed to construct and program reliable, highly-scalable systems. We will also cover architecture design of modern datacenters that constitute a central topic of the cloud computing paradigm. The course is complemented by a number of lab sessions to the design of scalable algorithms and get hands-on experience with Apache Spark.

***
## Notebooks
### [Lab1 Introduction](https://github.com/JZ-LIANG/Distributed-Systems-and-Cloud-Computing/blob/master/notebooks/Lab1%20-%20Introduction.ipynb)
<img align="right" src="images%20/intro_img.png" width="250">

In this introductory laboratory:
 * Acquire Pandas, Matplotlib, Numpy
 * Gain familiarity with the PySpark and how to interact with the HDFS
 * Gain hands-on experience with two Distributed codes: 
   * Word Count 
   * Analysis of night flights


### [Lab2 Distributed Gradient Descent](https://github.com/JZ-LIANG/Distributed-Systems-and-Cloud-Computing/blob/master/notebooks/Lab2%20-%20Distributed%20Gradient%20Descent.ipynb)
<p align="center">
<img src="images%20/gradient_img.png" width="600">
</p>

This notebook contains multiple implementations of the gradient descent algorithm. 
 * Generate synthetic data for a regression problem, and use Scipy lib to obtaine a baseline regression result.
 * A Numpy implementation of Batch Gradient Descent.
 * A Numpy implementation of Stochastic Gradient Descent and Mini-Batch Stocastic Gradient Descent.
 * A Distributed version of Mini-Batch Gradient Descent implemented using PySpark.

Beside i also compare those 4 implementations with the baseline from Scipy. A deep analysis is performed regarding how each algorithm's results change with parameters such as the learning rate and the number of iterations.  Finally an analysis of the performance of all the algorithms in terms of dataset size.


### [Lab3 Distributed k-Means](https://github.com/JZ-LIANG/Distributed-Systems-and-Cloud-Computing/blob/master/notebooks/Lab3%20Distributed%20k-Means.ipynb)
<img align="right" src="images%20/k-means_img.png" width="300">

This notebook is mainly about implementation and analysis the k-means algorithm on a 2D dataset:
 * A Numpy implementation of Vanilla k-means.
 * Analysis of algorithm convergence by Heterogeneity (total within Sum of Squares), and implementation the k -means++ technique for smart centroid initialization and allows to improve the quality of the local optima.
 * Implement the Elbow Method to help find the optimal value of the number of clusters.
 * A Distributed version of k-means is implemented with PySpark, the distributed version is analyzed and compared with the serial implementation.


### [Lab4 Flights Data Analysis](https://github.com/JZ-LIANG/Distributed-Systems-and-Cloud-Computing/blob/master/notebooks/Lab4%20-%20SparkSQL%20Flights%20Data%20Analysis.ipynb)
<img align="left" src="images%20/Sparkql_img.png" width="300">

This notebook is mainly about study the DataFrames API in Spark that allow developers to impose a structure on a distributed collection of data, allowing higher-level abstraction. We learn how to use DataFrame API and its advantages to manipulate distributed, structured data.

A hand-on experience is the analysis of flights data using SparkSQL. Data exploration is divided in three main sections: basic queries, flight volume statistics and additional queries. Data visualization is performed using the seaborn module.




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
