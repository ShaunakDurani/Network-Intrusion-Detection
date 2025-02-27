# Network-Intrusion-Detection
📌 Project Overview
This project focuses on detecting and mitigating DDoS attacks in a Software-Defined Networking (SDN) environment using Mininet and the Ryu controller. It involves generating a custom dataset, training a machine learning model, and implementing real-time traffic monitoring with firewall-based mitigation.

⚙️ Technologies Used
Mininet – For creating a virtual network topology.
Ryu Controller – For managing and controlling network traffic.
Python – For dataset processing, model training, and live traffic monitoring.
Machine Learning – To classify network traffic as benign or malicious.
Firewall Mechanisms – Blacklist and whitelist firewalls for mitigation.
📊 Dataset Generation
Why Custom Dataset?
Publicly available datasets often contain anomalies that can lead to 100% accuracy, making models ineffective for real-world scenarios. To overcome this, we generated our own dataset.

How It Works:
Topology Creation: A network topology is set up in Mininet.
Traffic Control: Using Ryu controller commands, traffic flows between nodes are managed.
DDoS Attack Simulation: Malicious traffic is introduced to generate realistic attack patterns.
Benign Traffic Generation: Normal traffic is also recorded for model training.
Dataset Preparation: The collected traffic data is preprocessed and labeled.
🧠 Machine Learning Model
The dataset is split into DDoS attack traffic and benign traffic.
A machine learning model is trained on this dataset, achieving 99% accuracy in classification.
The trained model is integrated into the live network monitoring system.
🔥 Attack Detection & Mitigation
Live Traffic Monitoring: The model continuously analyzes network packets.
Attack Detection: If DDoS traffic is detected, mitigation strategies are triggered.
Firewall-Based Mitigation:
Blacklist Firewall: Blocks detected malicious IPs.
Whitelist Firewall: Ensures trusted IPs remain unaffected.
IP List Management: Maintains an updated list of blacklisted and whitelisted IPs for faster processing.
🚀 How to Run the Project
