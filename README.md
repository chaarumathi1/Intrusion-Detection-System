# Intrusion-Detection-System
This project is a Python-based Intrusion Detection System (IDS) designed to monitor and analyse network traffic in real-time. It leverages both anomaly-based detection (using machine learning) and signature-based detection (using predefined rules) to identify suspicious behaviour or potential security threats on a network.
The system was built as an educational and functional demonstration of how real-world IDS systems can detect cyberattacks such as SYN flood, port scans, and anomalous traffic patterns. It’s ideal for students, cybersecurity enthusiasts, and researchers who want a hands-on understanding of IDS implementation.

# Key Features
•	Real-Time Packet Sniffing:
Utilizes the scapy library to capture live packets from the network interface.
•	Feature Extraction:
Extracts key features from captured packets such as:
o	Packet size
o	Packet rate
o	Byte rate
o	TCP flags
These features are essential for identifying patterns in normal vs. malicious traffic.
•	Signature-Based Detection:
Uses rule-based logic to detect known attack patterns like:
o	SYN Flood Attacks: High volume of SYN packets without ACK.
o	Port Scanning: Rapid requests to multiple ports with small packet sizes.
•	Anomaly-Based Detection (Machine Learning):
Implements the Isolation Forest algorithm to identify unknown or previously unseen attack patterns based on outlier detection in feature vectors.
•	Threat Classification & Alerting:
Each detected threat is categorized and logged with a confidence score. Alerts are saved in a .log file with timestamps for further analysis.
•	Modular and Easy to Extend:
The architecture is built in a modular way, making it easy to add new detection rules or enhance the machine learning model with more features or data.

 Technologies & Libraries Used
•	Python 3
•	Scapy – For packet sniffing and manipulation
•	Scikit-learn – For anomaly detection (Isolation Forest)
•	Numpy – For numerical processing
•	Logging – For saving and formatting alert logs

 Use Cases
•	Educational purpose to understand how IDS systems work
•	Baseline implementation for research projects in network security
•	Small-scale internal network monitoring for detecting unusual traffic
•	Foundation for further development of AI-driven IDS solutions

 Future Improvements
•	Add visualization of traffic and threat patterns using matplotlib or plotly
•	Expand detection rules for other known attack types
•	Deploy in a real-time environment using multi-threading or background services
•	Integrate with a dashboard or notification system

