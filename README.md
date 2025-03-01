# Network Traffic Classification with Machine Learning  

This project focuses on **network traffic classification** using multiple **Machine Learning (ML) models**.  
The dataset used is **UNSW-NB15**, which contains both normal and attack traffic of various types (Fuzzers, DoS, Shellcode, etc.).  
The goal is to implement different ML approaches to accurately classify network traffic and analyze model performance.

## Dataset
The **UNSW-NB15** is a comprehensive data set for network intrusion detection systems, created by dr. Nour Moustafa and dr. Jill Slay.  
A detailed explanation of the dataset can be found on their [original paper](https://ieeexplore.ieee.org/abstract/document/7348942) and on the [UNSW-NB15](https://research.unsw.edu.au/projects/unsw-nb15-dataset) page.  
The dataset is comprised of labeled network traffic data including both normal and attack network traffic.  
The dataset consists of **49 features** including both **numerical** and **categorical** attributes.

### Attack Categories  
The attack-labeled network traffic data contains **nine different attack categories**:

- **Fuzzers** – Attempts to cause a program or network suspended by inputting large amounts of random data.
- **Analysis** – Attacks involving reconnaissance and vulnerability scanning.  
- **Backdoors** – Unauthorized access mechanisms that allow attackers to bypass authentication and gain remote control over a system.
- **DoS (Denial of Service)** – Attacks that flood a network or system with excessive requests, making it unavailable to users.
- **Exploits** – Attacks that take advantage of known system vulnerabilities.  
- **Generic** – Attacks that target cryptographic weaknesses in encryption algorithms.  
- **Reconnaissance** – Network scanning for gathering information.  
- **Shellcode** – Code injection attacks exploiting buffer overflows.  
- **Worms** – Self-replicating malware that spreads across networks.    

## Technologies Used  
- **Python** (pandas, numpy, matplotlib, seaborn, sklearn)  

## Support Vector Machine (Polynomial Kernel)

### Binary Classification
 ```python
 model = SVC(kernel='poly', cache_size=500, probability=True)
 ```

#### Performance Metrics:
- Accuracy: 0.8729291162609921
- Precision: 0.8679978048883448
- Recall: 0.9071737404041296
- f1 score: 0.8871534893754719
- ROC AUC: 0.9408879134362458

## License  
This project is open-source and available under the [MIT License](LICENCE).  