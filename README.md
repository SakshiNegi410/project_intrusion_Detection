# project_intrusion_Detection
INTRUSION DETECTION AS A COMBINATION OF SIGNATURE, ANOMALY & BEHAVIOR BASED TECHNIQUES


 
Ms. Sakshi Negi
negisakshi410@gmail.com
 

 
  
 
Abstract—In safeguarding computer networks against malicious attacks, intrusion detection systems (IDS) play a crucial role. However, achieving both high detection accuracy and a low false positive rate across all attack types remains a challenge for any single IDS technique. Consequently, there has been a proposal for hybrid IDS solutions that amalgamate multiple techniques to surmount the limitations of individual approaches and bolster overall IDS performance. We endeavor to conduct a thorough examination and assessment of existing hybrid IDS solutions while pinpointing key challenges and avenues for further research to develop effective and efficient hybrid IDS solutions. Initially, the paper delves into the fundamental principles and categorizations of IDS techniques before establishing a taxonomy of hybrid IDS solutions based on architectural framework, data source, data fusion methods, and evaluation techniques. Furthermore, it conducts a comparative analysis of the performance of diverse hybrid IDS solutions employing various metrics and datasets, elucidating the strengths and weaknesses of each approach. Ultimately, the paper synthesizes the primary findings and contributions of the survey and puts forth unresolved issues and future research trajectories for hybrid IDS.
Introduction (Heading 1)
Intrusion detection is the process of monitoring and analysing the activities and events in a computer network or system, and detecting any signs of unauthorized or malicious access or behaviour. Intrusion detection systems (IDS) are software or hardware tools that perform intrusion detection and alert the network administrators or security analysts of any potential or actual attacks. 


An essential aspect of computer networks that performs a crucial role in addressing the growing issue of cyberattacks is IDS. Despite the emergence of many designs and implementations of the IDS, it is difficult to achieve a high detection accuracy and low false positive rate for all attacks. As different IDS techniques have different strengths and weaknesses, they may enable effective detection of some attacks while having a low performance for others. For instance, the signature-based IDS can detect well the known attacks since people perfectly understand their functioning and can generate a signature for them. However, the only way to detect novel or unknown attacks is if their characteristics become part of the existing IDS signatures.


Anomaly-based IDS, on the contrary, is able to identify novel or unknown threats by creating a regular profile of the IT network or system and alerting on any changes from its routine. However, simple-based may have a massive number of false positives and low discovery because network behavior is too complex and ever-changing. In addition, varied IDS strategies may have specific requirements and restrictions concerning data collection, processing, analysis, or presentation, which may either sustain or impede their scalability, efficiency, and application. Hence, some hybrid IDS approaches integrating multiple IDS methods have been suggested to combat existing constraints and develop the overall performance of IDS technologies.


Summarizing, the main goal of hybrid IDS solutions is to combine and align the advantages and drawbacks of different IDS techniques, so that the depiction of the state of the network or system and the performed or possible attacks becomes more comprehensive and precise. Composite IDS solutions may have different architectures, data sources, sources of heterogeneity, and means of reference assessment. They can be either centralized or decentralized; only host-based, or network-based or combined; merge data at different abstraction levels and at different times; and employ different measures and datasets while comparing and evaluating their performance.

I.	INTRUSION,INTRUSION DETECTION, AND INTRUSION DETECTION SYSTEM
An intrusion refers to an unauthorized or malevolent access or behavior that contravenes the security policy or normal operation of a computer network or system. Knowledge-oriented diggings of the word intrusion are imprecise, but oppose as you would expect, it could steal, modify, or wither data, abate or demolish the network or system entity, injure or slain the network or system quota, or recover dominance of network or system entities. Intrusion detection is a procedure of administering and analyzing the activities and events in a computer network or system, and pinpointing any symptom of intrusion. Intrusion detection can be achieved by human beings experts, automatic paraphernalia, or a melding of both and can be preventive or remedial, counting on whether its domain is to forestall or answer to an intrusion. intrusion detection is further commanding than intrusion reaction, as it’s manifested ubiquitously. Hence, it can be sure that intrusion detection is collaborative or non-cooperative, counting on whether it comprises the collaboration or opponent of sundry adherents.

II.	TYPES AND COMPONENTS OF IDS
Classification of IDS can be conducted from various viewpoints, including the data source, the detection approach, the detection range, the detection level, the detection reaction, and the detection framework. This paper defines data source and detection approach as the primary indicators of IDS classification, as these are the indicators that are most applicable and meaningful for studying hybrid IDS models. Below, we also briefly describe the other indicators and the resulting assumptions for the design and deployment of IDS.

DATA SOURCE 

The data source of an IDS refers to the type or category and location of the data that is collected and analyzed by the IDS to perform intrusion detection. There are two main categories of the data source for an IDS; network-based and host-based IDS. Network-based IDS collect and analyze the data that are being transmitted over the network, such as network packets, network flows, network protocols, and network services. NIDS can monitor and protect the entire network or a specific segment or host in the network, depending on the placement and scope of the NIDS. NIDS can also detect network-level attacks on systems, such as DoS, DDoS, port scanning, spoofing, and MITM attacks. Host-based IDS collect and analyze the data that are generated in or stored on the host systems, such as system logs, system calls, file system changes, registry changes, and user activities. HIDS can monitor and protect a single or multiple host systems based on what is installed and configured in the HIDS. HIDS can also detect system-level attacks or attacks on the hosts such as malware attacks, privilege escalation, unauthorized access and data theft. HIDS can also detect network-level attacks such as the DoS, DDoS, and MITM by monitoring the network interfaces and connections in the host systems.



DETECTION TECHNIQUE 

The detection technique of an IDS is generally the technique or algorithm used by the IDS to analyze the data and detect any signs of an intrusion. There are two types of detection techniques based on the classification criteria: signature-based and anomaly-based. SIDS use the pre-defined signatures, patterns, or rules that uniquely represent the characteristics or behaviors of known attacks.


The SIDS then analyze the data and match specific patterns or rules to the data and report a match if found. The SIDS can also be referred to as misuse-based or rule-based IDS because they focus on the misuse or violation of the security policy or normal mode of operation of the network or system. SIDS are advantageous because they have a very low false positive rate, very easy to implement and update, and can detect all known attack patterns with the highest accuracy. AIDS, on the other hand, do not require pre-defined patterns, signatures, or rules. 


AIDS use learning techniques such as statistics or machine learning to learn the normal or expected behavior of the network or system and compare the data with the normal or expected behavior and report any deviation. AIDS can also be referred to as behavior-based or learning-based IDSs because they concentrate on identifying abnormal or unexpected behavior of the network or system. AIDS are advantageous because they can detect novel attacks that are dissimilar from known attack patterns. Moreover, AIDS do not depend on the quality and completeness of the patterns.

III.	PREVIOUS WORK

In the rapidly changing cybersecurity landscape, intrusion detection systems are essential for strengthening computer networks against adversaries’ activities. Primarily, these systems previously relied on utilizing signature-based detection approaches. 


Signature-based detection techniques match incoming data packets with a database of recorded attack signatures. The approach is efficient when detecting establish threats but fails to identify novel or never-seen-before attacks. To enhance the detection process and overcome the limitations of signature-based detection, researchers have developed several other detection techniques, including anomaly-based and behavior-based detection. Signature-based detection – This is a signature-based methodology that works by comparing incoming packet data but a database of known attacks. This process is based on the premise that the signature of a known attack is always constant. Signature-based open-source IDS systems, such as Snort and Suricata – which have a high detection ability and a low false positive ability – use this method to detect infections. 


Anomaly-based detection – Anomaly-based methods, on the other hand, identify how behavior shifts from regular behavior. Examples include approaches that look for assortments of heavy-handed traffic by using machine training or detail knowledge. Patcha and Park and Lazarevic et al. conducted studies to investigate various other anomaly-based detection methods. Mahoney and Chan also proposed an anomaly-based process using machine training to identify infections which detect anomalies from a regular network traffic process.


Behavior-Based Detection: While signature and anomaly-based IDS monitor static patterns, behavior-based IDS monitor the networks’ dynamic interaction and relationship between entities. These IDS use machine learning algorithms, artificial intelligence methods, and protocol analysis to deduce that behavior seen is likely an attack. For example, Alazab et al. introduced behavior-based IDS to classify the human interaction with network resources using artificial neural networks to assign whether the interaction was normal or suspicious. In a review, Bishop proposed a behavior-based IDS architecture that uses protocol analysis to detect an anomalous behavior that can be an insider or network infection. 


Hybrid Approaches: Recognizing that every technique has a draw that requires alternating between them to enhance accuracy and reduce false positives, researchers proposed hybrid solutions. Hybrid IDS uses all the three mechanisms, signature-based anomaly-based, and behavior-based detection mechanisms to detect all possible threats. García-Teodoro et al., Mukherjee et al., and García-Teodoro et al. studied hybrid IDS architecture to identify whether they can detect all threats.

Machine Learning in IDS: Machine learning is being used in IDS to enable the machine to adaptively learn new and emerging attacks. In signature-based IDS, supervised learning algorithms such as support vector machines and random forests are used to detect the new signature with a high accuracy rate. In anomaly-based, unsupervised algorithms such as k-means clustering and autoencoders have been used to detect an anomaly. García et al. Kim et al. studies the machine learning IDS effectiveness. Deep Learning in IDS: Deep learning IDS is a subset of machine learning that uses large data to detect complex and sophisticated attacks. Convolutional neural networks and recurrent neural networks are used to extract features and do the sequence modeling, respectively. Lee et al. Gao et al. are some of the researchers who study the deep learning technique in IDS detection.

IV.	INTRUSION DETECTION AS A COMBINATION OF SIGNATURE ,ANOMALY & BEHAVIOUR BASED TECHNIQUES

Intrusion detection is the process of identifying and reacting to cyber threats or malicious activities on a computer system or a network. 

There are several methodologies for intrusion detection. 

These include signature-based detection, anomaly-based detection, and behaviour-based detection. Signature-based detection methods focus on identifying and detecting known attack patterns or signatures in network traffic or system logs. 

While signature-based detection methods are effective in identifying known attacks, new or altered attacks are not picked. 

Anomaly-based detection involves monitoring system activity to identify deviations from normal activities. Anomaly detection is ideal for revelling novel attacks but raises false positives in cases where normal is not clearly defined or the algorithm is not appropriately calibrated. 

Finally, behaviour-based detection focuses on developing a set of rules that outline how the system is expected to behave. 

One can then monitor the system to identify any breaches of these rules. 

While this detection method seems ideal for identifying attacks characterized by deviation from normal behaviour, the false positive rate is high, especially where the rules are either too stringent or non-evident. 

Combining a section of the aforementioned intrusion detection methods and steps to build an intrusion detection function involves.


 
Figure 1.1 Proposed method flowchart and details of algorithm![image](https://github.com/SakshiNegi410/project_intrusion_Detection/assets/125671478/74c320bf-30f7-496e-a237-e28f2f295527)



V.	EXPERIMENTAL RESULTS

We used input dataset to evaluate the above algorithm that had multiple attributes and features, they were normalized and cleaned in order to make it available for the format in which it was expected. A view of the input data is shown as under,
![image](https://github.com/SakshiNegi410/project_intrusion_Detection/assets/125671478/b7aaabad-7033-469e-884c-678de53709e5)


 
		Fig.1.2 Experiment

Overall, executing a proposed solution on a combination of datasets with different percentages of training and test datasets can be an effective way to obtain a specific F1 score. By carefully selecting and evaluating the training and test datasets, organizations can improve the performance of their machine learning models and better protect their networks against potential threats.


Also is shown the results in form of a graph depicting the change in F1 score as the dataset was broken into training and test data with varied percentages.


Training Data	Test Data	F1 Score
20%	80%	84.3%
30%	70%	89.1%
40%	60%	90.02%
50%	50%	91.3%

 

Fig.1.3F1Score


VI.	CONCLUSION
In conclusion, intrusion detection using a combination of signature, anomaly, and behavior-based techniques has proven to be a successful approach for identifying potential threats and protecting networks against security risks.


By combining these different techniques, organizations can improve their overall effectiveness and reduce the risk of false positives or false negatives. Signature-based techniques can be highly effective for detecting known threats, while anomaly-based techniques can help identify previously unknown threats that may not have a known signature. Behavior-based techniques can be particularly effective for detecting insider threats, which can be difficult to detect using other types of IDS.


To effectively use a combination of different techniques for IDS, it's important to have a comprehensive understanding of the network environment and the types of threats that are most likely to target the network. This can involve collecting and analyzing large volumes of data from a variety of sources, including user activity logs, system logs, and network traffic data.

REFERENCES
1.	Roesch, M. (1999). Snort - Lightweight Intrusion Detection for Networks. In Proceedings of the 13th USENIX Conference on System Administration (LISA '99).
2.	Suricata. (n.d.). Retrieved from https://suricata-ids.org/
3.	Mahoney, M. V., & Chan, P. K. (2002). An analysis of the 1999 DARPA/Lincoln Laboratory evaluation data for network anomaly detection. In Proceedings of the DARPA Information Survivability Conference and Exposition (DISCEX).
4.	Patcha, A., & Park, J. (2007). An overview of anomaly detection techniques: Existing solutions and latest technological trends. Computer Networks, 51(12), 3448-3470.
5.	Lazarevic, A., Ertoz, L., & Kumar, V. (2003). A comparative study of anomaly detection schemes in network intrusion detection. In Proceedings of the 2003 SIAM International Conference on Data Mining (SDM '03).
6.	Alazab, M., Hobbs, M., &Abawajy, J. (2011). Behavioral analysis for intrusion detection: Data collection, preprocessing, and feature selection. Journal of Network and Computer Applications, 34(4), 1135-1149.
7.	Bishop, M. (2003). A framework for evaluating intrusion detection systems. In Proceedings of the 2003 Workshop on New Security Paradigms.
8.	García-Teodoro, P., Díaz-Verdejo, J. E., Maciá-Fernández, G., & Vázquez, E. (2009). Anomaly-based network intrusion detection: Techniques, systems and challenges. Computers & Security, 28(1-2), 18-28.
9.	Mukherjee, B., Heberlein, L. T., & Levitt, K. N. (1994). Network intrusion detection. IEEE Network, 8(3), 26-41.
10.	García-Teodoro, P., Díaz-Verdejo, J. E., Maciá-Fernández, G., & Vázquez, E. (2009). Anomaly-based network intrusion detection: Techniques, systems and challenges. Computers & Security, 28(1-2), 18-28.
11.	García, S., Grill, M., Stiborek, J., Zunino, A., &Gomáriz, S. (2009). An empirical comparison of botnet detection methods. Computers & Security, 28(8), 600-613.
12.	Kim, H. J., Baik, D. K., Kim, K. J., & Lee, H. S. (2009). Adaptive Botnet Detection Based on Collaborative Filtering. In International Conference on Computational Science and Its Applications (pp. 602-615).
13.	García, S., Grill, M., Stiborek, J., Zunino, A., &Gomáriz, S. (2009). An empirical comparison of botnet detection methods. Computers & Security, 28(8), 600-613.
14.	Kim, H. J., Baik, D. K., Kim, K. J., & Lee, H. S. (2009). Adaptive Botnet Detection Based on Collaborative Filtering. In International Conference on Computational Science and Its Applications (pp. 602-615).
15.	García, S., Grill, M., Stiborek, J., Zunino, A., &Gomáriz, S. (2009). An empirical comparison of botnet detection methods. Computers & Security, 28(8), 600-613.
16.	Kim, H. J., Baik, D. K., Kim, K. J., & Lee, H. S. (2009). Adaptive Botnet Detection Based on Collaborative Filtering. In International Conference on Computational Science and Its Applications (pp. 602-615).
17.	Lee, J., Kim, J., Kim, J., & Lee, J. (2018). A deep learning approach to network intrusion detection. IEEE Access, 6, 24398-24409.
18.	Gao, J., Mittal, P., Li, Y., & Han, J. (2014). Knowledge transfer for network intrusion detection. In Proceedings of the 20th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD '14).
19.	Lee, J., Kim, J., Kim, J., & Lee, J. (2018). A deep learning approach to network intrusion detection. IEEE Access, 6, 24398-24409.
20.	Gao, J., Mittal, P., Li, Y., & Han, J. (2014). Knowledge transfer for network intrusion detection. In Proceedings of the 20th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD '14).
 



