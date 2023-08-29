### Intrusion and Vulnerability Detection in Software Defined Networks
Problem stated by [ITU AI For Good Global Summit](https://challenge.aiforgood.itu.int/match/matchitem/81) and presented by [ITU & ULAK](https://www.youtube.com/watch?v=zgne_H0Ki7M)
#### Abstract:
Software Defined Networks (SDNs) have revolutionised the way modern networks are managed and orchestrated. This sophisticated infrastructure can provide numerous benefits but at the same time introduce several security challenges. A centralised controller holds the responsibility of managing the network traffic, thus making it an attractive target to attackers. Intrusion detection systems (IDS) play a crucial role in identifying and addressing security threats within the SDN. By utilising machine learning algorithms an anomaly based detection system was established to identify deviation in network behaviour. Five machine learning algorithms were employed to train the SDN-IDS, and ultimately, the most appropriate one was chosen. The SDN-IDS demonstrated an exceptional overall performance, particularly when using the XGBoost Classifier trained with a reduced feature train dataset, reaching 99.9\% accuracy as well as 99.9 F1-score. Furthermore, it exhibited near-perfect performance in identifying the most types of attacks within the traffic data.

####  Software Defined Network Intrusion Detection System (SDN-IDS) Architecture:
Our SDN-IDS firstly cleans the data by removing corrupted and duplicate instances, replaces missing values with averages and removes features that contribute zero values only. The categorical label values were replaced wth numerical ones.
#### About Machine Learning Models Used:
Three baseline models were chosen to be used among with the some more complex models. Decision Trees (DT), Random Forest (RF) and K-Nearest Neighbours (K-NN) were selected
since they have an extensive use in the topic of IDS, are easy to implement and support multi-class classification. Also a Bagging and a Boosting classifier were utilised. 

#### About Resampling Techniques:
Network traffic datasets used for IDS are usually imbalanced. Imbalanced data usually lead to a biased model towards the majority class. 
From our perspective to tackle this problem, resampling techniques such as SMOTE and Tomek’s link  were utilised in order to alleviate data imbalances between classes.

#### Results
![plot](https://github.com/sotirischatzimiltis/SDN_IDS/blob/main/Figures/test_set_performance.PNG)
![plot](https://github.com/sotirischatzimiltis/SDN_IDS/blob/main/Figures/macro_test_performance.PNG)
![plot](https://github.com/sotirischatzimiltis/SDN_IDS/blob/main/Figures/xgb_test_reduced_baseline_cf.png)
![plot](https://github.com/sotirischatzimiltis/SDN_IDS/blob/main/Figures/dt_test_reduced_cf.png)
#### Authors 
Sotiris Chatzimiltis, Mohammad Shojafar, Mahdi Boloursaz Mashhadi, and Rahim Tafazolli <br />
5GIC \& 6GIC, Institute for Communication Systems (ICS), University of Surrey, Guildford, UK <br />
sc02449@surrey.ac.uk, m.shojafar@surrey.ac.uk, m.boloursazmashhadi@surrey.ac.uk, r.tafazolli@surrey.ac.uk

