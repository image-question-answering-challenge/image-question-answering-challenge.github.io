
## 1. Introduction
This challenge focuses on the use of Web data to support semantic Visual Question Answering: given a large image collection, find a set of images matching natural language queries. The task will support advancing the state-of-the-art in Visual Question Answering by focusing on semantic representation and reasoning mechanisms. In order to address natural language queries, participating systems will need to integrate graph descriptors extracted from images to  use structured and unstructured Web data sources. 

## 2. Motivation 
As of 2017, it is estimated that images and videos account for up 73% of all all consumer Internet traffic according to Cisco Visual Networking Index [1]. However, due to its non-symbolic nature, most of the content present in visual form depends on the use of associated textual content or annotations to become accessible and searchable to end users. These associated textual information provide a limited slice to the full information content (such as entities and relations) expressed in the images. With recent advances in machine learning techniques [2,3], in particular, in the field of computer vision, the detection and classification of objects embedded in images became a very active research area [4,5,6]. More recently, the detection of relations between objects in an image scene [7,8,9,10], defined the use of lexico-semantic graphs as a lightweight representation device for images. The emergence of richer symbolic-level representation models opened the doors to more sophisticated semantic interpretation models and applications such as Visual Question Answering (VQA).

However, addressing the problem of Question Answering over visual data requires semantic representation models. These models support semantic approximation and reasoning operations necessary to bridge the gap between queries and the immediate description of an image. Moreover, it requires the integration of the intermediate graph extracted from the image to large commonsense knowledge bases.

This challenge aims at advancing the discussions on the state-of-the-art in these areas, and is creating a test collection which explores the semantic aspects of VQA.


## 3. Challenge Timeline

	* Training data ready and challenges CFP sent : 01 December 2017
	* Challenge papers submission deadline : 12 January 2018
	* Challenge papers acceptance notification : 14 February 2018
	* Challenge test data published : 14 February 2018


## 4. Dataset Description
![alt text](./graph_sample.png)


## 5. Evaluation Criteria

The test collection consists of 1000 natural language queries divided into training (600 queries) and test (400 queries) sets. All natural language queries will require the integration of one or more knowledge graphs from multiple modalities and will explore different types of representation and reasoning on the top of the scene description (See Section 5). Three data sources will be used: (i) Visual Genome scene graphs (1.7 million of object instances and 2.3 million of relationships) [11], (ii) ConceptNet 5.5 (around 28 million of statements and around 4 million of concepts) [13] and (ii) DBpedia 2016-04 (around 18 million of instances and around 80 million of statements) [14]. Participating VQA systems will be evaluated with regard to mean average precision, recall, F1-score, mean reciprocal rank and normalized discounted cumulative gain (NDCG). The challenge will provide Gerbil QA [12] as a supporting evaluation platform. Participating systems will be able to run their webservice against the evaluation platform to test their system against the provided training data and get the correct measures above back. This system ensures long term reproducibility and comparability of evaluation results. GERBIL QA layed the foundation for the H2020 project HOBBIT (https://project-hobbit.eu/) which aims at benchmarking Big Linked Data in a FAIR way. However, to not impose a technical hurdle on the participants, the submissions to the challenges can also happen as file submission in a later announced format.




