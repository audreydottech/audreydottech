## Hi there 👋

My name is Audrey, and I am a data engineer and ontologist with Python, React.JS, Spark and SQL experience. I made the transition from a career in metadata management because I am an impatient person by nature and would look for ways at work to automate tasks. I tend to get very excited about the process of gathering requirements and designing data pipelines, with the goal of empowering users with analytics.  


## Projects (ordered by recency)

**Building an eCommerce App in React** [repo](https://github.com/audreydottech/ecommerce-react-js-app)

A simple e-commerce app that displays products, a navigation bar and cart for a fictitious brand. Part of a Girls Develop It project.

*Stack:* [React](https://create-react-app.dev/) | [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS) | [Redux](https://redux.js.org/)


**The ESG Stock Performance Dashboard** [repo](https://github.com/audreydottech/esg-data-pipeline)

A data pipeline that extracts data from various finance APIs daily and automatically updates the database tables after checking for duplicate data. Originally coded in Python and Scala to stream data using Kafka and sink it into Delta Lake tables stored in Azure with Databricks as the analytical engine. [Original repo](https://github.com/audreyle/Real-Time-Stock-Updates) I rewrote the notebook to make it more readily available to the public, using my AWS credits to save on storage and Github Actions to run the data pipeline on schedule. This data pipeline is part of a six-month project to build a dashboard to understand the relationship between ESG ratings and a stock's performance based on the sector, region and investor confidence in company news. 

*Stack:* [Github Actions](https://github.com/features/actions) | [Databricks](https://www.databricks.com/product/data-intelligence-platform) | [AWS](https://aws.amazon.com/free/) | [Azure](https://azure.microsoft.com/en-us/products/storage/blobs)


**Access Map** [repo](https://github.com/audreydottech/AccessMap)

A web application that allows users to view a location's accessibility rating prior to their visit. Ratings are given on a 5-point scale (where 0 is least accessible and 5 is most accessible). There are multiple categories such as: sensory rating, mobility rating, service dog relief, wheelchair accessibility rating, common allergen rating. This app was built in a team of women developers and designers, with a technical lead representing the very demographics to whom the app would be marketed. The app is currently under construction. The backend extracts the crowdsourced ratings from a Google form and ingests it into a Postgres database. I wrote the stored procedures as Python functions with embedded SQL queries to update the database and display the ratings onto a custom Google Maps. 

*Stack:* [Google Cloud](https://cloud.google.com/gcp) | [Google Maps](https://developers.google.com/maps/documentation/javascript/overview) | [Flask](https://flask.palletsprojects.com/en/stable/)


**IMDB Vector Database** [repo](https://github.com/audreyle/IMDB-Vector-Search-DB)

This is a Jupyter notebook that showcases my ability to read nested json data. The movie titles were transformed into vectors and stored in a Pinecone vector database to run the k-nearest neighbor algorithm and generate movie recommendations based on a user's keyword search. 

*Stack:* [Vector database](https://www.pinecone.io/lp/get-vector-database/) | [Similarity search](https://scikit-learn.org/stable/modules/neighbors.html)


**The Wikipedia Property Graph** [repo](https://github.com/audreyle/Wikipedia-Property-Graph)

A notebook that includes all the tools needed for a taxonomist to query a knowledge graph via metadata or property without the need to pay for taxonomy software to slice and dice it. I built a parser to transform RDF triples into separate vertex and edge Spark RDDs, whereby the edge RDDs store the ids to the vertices directly with the relationship data. Storing the indices so to speak allows Spark workers to retrieve the distributed data faster because it is partitioned by relationship and the integer IDs point to an address in memory, therefore allowing the running time of graph algorithms that retrieve a node's neighbors to be closer to O(V+E). For taxonomists, it's also a clear win because it allows them to explore connections in a graph (and to determine areas of a taxonomy that are bloated and those that are missing metadata) without the assistance of a data scientist. 

*Stack:* [Spark RDDs](https://www.databricks.com/glossary/what-is-rdd) | [Spark GraphX](https://spark.apache.org/graphx/)


**Predicting ICU Deaths** [repo](https://github.com/audreyle/Predicting-ICU-Deaths)

A machine learning pipeline to predict the strongest factor in ICU deaths across hospitals around the world. Made with a team of medical experts, a data scientist, a data engineer and a software engineer. We experimented with various ensemble learning methods such as AdaBoost and XGBoost to build our predictive model out of multiple decision tree algorithms (to improve the model's predictive performance from a basic logistic regression), using GridSearchCV to fine-tune the hyperparameters (i.e. learning rate) and SMOTE to balance our dataset (to avoid overfitting). Then, we compared the ROC/AUC scores of each model and concluded that XGBoost with stratified random sampling would yield the most accurate predictions. 

*Stack:* [Ensemble Learning](https://machinelearningmastery.com/tour-of-ensemble-learning-algorithms/) | [AdaBoost](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.AdaBoostClassifier.html) | [XGBoost](https://www.nvidia.com/en-us/glossary/xgboost/) | [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html)


**Neural Art Style Transfer** [repo](https://github.com/audreydottech/neural-art-style-transfer)

Neural style transfer takes two images and uses convolutional neural networks (CNNs) to transfer the style of one image to the other. 

*Stack:* [Tensorflow](https://www.tensorflow.org/) | [Convolutional Neural Networks](https://www.datacamp.com/tutorial/introduction-to-convolutional-neural-networks-cnns)



## More About Me

- 🔭 I’m currently working on an auto-classifier for a federal government agency.
- 🌱 I’m currently learning React, MongoDB and Snowflake.
- 👯 I’m looking to collaborate on data analytics and data governance. 
- 💬 Ask me about how taxonomy can help your organization ensure the highest level of integrity and acesss for your data.
- 📫 How to reach me: DM me on LinkedIn, I have an avatar.
- 😄 Pronouns: she/her/hers
- ⚡ Fun fact: I'm a Pilates fan and wine connoisseur.

<!--
**audreydottech/audreydottech** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
-->
