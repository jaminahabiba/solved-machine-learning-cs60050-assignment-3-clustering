Download Link: https://assignmentchef.com/product/solved-machine-learning-cs60050-assignment-3-clustering
<br>
<strong>AAAI needs your help !!! </strong>

<strong> </strong>

The Association for the Advancement of Artificial Intelligence (AAAI) organizes a conference of Artificial Intelligence, which is one of the most prestigious conferences relevant to the field of AI. Every year many researchers across the world submit to the conference and after a rigorous process of review and evaluation, only a selected set of papers get accepted. 150 such papers got accepted in AAAI this year. The submissions were found to span over several different domains of computer science such as: Machine Learning, Optimization, Knowledge-Based systems, Robotics, Natural Language Processing, etc..




You can find a dataset containing all the accepted submissions <u>​</u><a href="https://drive.google.com/file/d/1cz-6cVfF-A7Tp6of7L8NhczmGUBhFP1w/view?usp=sharing"><strong>here</strong></a>​. In this dataset you will find the following relevant attributes of each paper.

<ul>

 <li><strong>Title:</strong>​ Free Text; Title of the paper</li>

 <li><strong>Keywords:</strong>​ Free Text: author-generated keywords</li>

 <li><strong>Topics:</strong>​ Categorical; author-selected, low-level keywords from conference-provided list</li>

 <li><strong>High-level Domains:</strong>​ Categorical; author-selected, high-level keywords from conference-provided list. There are 9 distinct high-level domains in the dataset. ● <strong>Abstract:</strong>​ Free Text: abstract of the paper</li>

</ul>




AAAI wants an automated unsupervised script to group these documents into different clusters, so that all papers having similar high-level domains will be grouped together. For example: Let’s assume there is a paper by Harish on a novel Clustering Algorithms, and there is another paper by Surya on a novel Classification Algorithm. <u>​Topics</u>​ of the two papers might be different such as: {Clustering, Unsupervised, Machine Learning} and {Classification, Supervised, Machine Learning}, however both come under the same ​<u>high-level domain</u><u>​</u>, i.e., Machine Learning.




To complete this task there has to be a notion of similarity among different papers. For this assignment, the simple ​<strong>jaccard coefficient of two sets of topics</strong>​ is considered as the notion of similarity between the two papers. For example, if the set of topics for a paper is H = {Clustering, Unsupervised, Machine Learning} and if the set of topics for another paper is S = {Classification, Supervised, Machine Learning}, then the Jaccard Coefficient between the two papers is<em>JC<sub>HS </sub></em>= <em>JC<sub>SH </sub></em>.




<ol>

 <li>Implement a <strong>bottom-up hierarchical clustering algorithm</strong>​ considering the​              aforementioned notion of similarity, to find <strong>9</strong>​ ​ <strong>(</strong>​ <strong>nine)</strong> clusters using both the (i) ​        <strong>complete</strong>​           <strong> linkage</strong>​ and (ii) ​<strong>single linkage </strong>​ State the clusters identified in your report.</li>

</ol>




<ol start="2">

 <li>With the same notion of similarity, design a graph where each node is a research paper, and an edge is to be drawn between two nodes if their topics are very similar (you can decide some threshold for this purpose, based on the quality of the clusters – see later). Now apply the ​<strong>Girvan-Newman clustering algorithm</strong>​ on this graph to find ​<strong>9 (nine)</strong> State the clusters identified in your report. ​<strong>For this part, you can use any graph library (e.g., the Networkx package in Python, or igraph library in C) for creating / updating the graph, and evaluating the centralities. However, direct use of any implementation of Girvan-Newman clustering algorithm will be penalised.</strong></li>

</ol>




<ol start="3">

 <li>Consider the ‘gold standard’ clustering to be based on the high-level domains associated with the papers, i.e., all papers of a particular high-level domain (according to the dataset) constitute one cluster.</li>

</ol>

Now you have three sets of clusters (having 9 clusters each) of the given set of research papers, one identified by the hierarchical clustering method with complete linkage, the second identified by the hierarchical clustering method with single linkage, and the third identified by the graph-based method.

The final step is to evaluate the quality of these three clusterings. To this end, implement the ​<strong>Normalized Mutual Information (NMI)</strong>​ metric mentioned in this <u>​</u><a href="https://nlp.stanford.edu/IR-book/html/htmledition/evaluation-of-clustering-1.html">document</a>​ to evaluate the quality of the clusters that you have got. Report the NMI values of the three clusterings.

Submission instructions




For each part, you should submit the source code and all result files. Write a separate source code file for each part. <strong>You</strong>​<strong> should include a README file describing how to execute each of your codes</strong>​, so that the evaluators can test your code.




<strong>You can use C / C++ / Java / Python for writing the codes; no other programming language is allowed. </strong>​<strong>You cannot use any library/module meant for clustering or Machine Learning</strong>​<strong>. You can use libraries for other purposes, such as generation and formatting of data, and a graph library for Part 2 (as specified above), but </strong><strong>NOT</strong>​<strong> for the ML part.</strong>​<strong> Also you should not use any code available on the Web. </strong>​<strong>Submissions found to be plagiarised or having used ML libraries will be awarded zero marks for all the students concerned. </strong>




Along with the source codes and the results, you should submit a report (pdf) including the following:

<ul>

 <li>For each of the three clustering methods — final learned clusters and the number of entities in each of them.</li>

 <li>NMI values of the three clusterings you obtained</li>

 <li>What are the thresholds that you are considering while doing the assignments have to be clearly mentioned. Note that you can decide upon what sort of thresholding you want to do based on the goodness of your clusters.</li>

</ul>

All source codes, data and result files, and the final report ​<strong>must be uploaded via the course Moodle page, as a single compressed file (.tar.gz or .zip)</strong>​.​ The compressed file should be named as: ​<strong>{ROLL_NUMBER}_ML_A3.zip or {ROLL_NUMBER}_ML_A3.tar.gz </strong>

Example: If your roll number is 16CS60R00, then your submission file should be named as 16CS60R00_ML_A3.tar.gz or 16CS60R00_ML_A3.zip




<strong>***Note that the evaluators can deduct marks if the deliverables are not found in the way that has been asked for the assignment. </strong>

<strong> </strong>

<strong>Submission deadline: March 31, 2019, 23:59 IST </strong>​<strong>[hard deadline] </strong>




For any questions about the assignment, contact the following TAs:

<ol>

 <li>Abhisek Dash (assignmentad @ gmail . com)</li>

 <li>Paheli Bhattacharya (paheli.cse.iitkgp @ gmail . com)</li>

</ol>