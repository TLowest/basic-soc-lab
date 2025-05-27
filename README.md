# Basic SOC Lab: SIEM and Log Analysis

---

## Project Overview

This project provides a structured, multi-node lab environment that emulates a lightweight Security Operations Center (SOC) using open-source technologies. It guides users through the deployment of a distributed SIEM architecture leveraging the ELK Stack (Elasticsearch, Logstash, Kibana) with Filebeat for log forwarding. Additional features include GeoIP enrichement, email alerting, centeralized log collection from multiple Ubuntu-based nodes, and automated deployments using Ansible and Docker. 

The lab is intended for cybersecurity students, entry-level SOC analysts, and DevSecOps professionals who wish to develop practical skills in log management, threat detection, event correlation, and SOC automation in a scalable and modular environment. 

--- 

### Virtual Machine Architecture

| **Purpose** | **Tools / Services** |
| :---: | :---: |
| VM #1 : Ansible Control Node | Ansible, Docker, SSH Keys to other VMs |
| VM #2 : ELK Stack Node 1 | Elasticsearch (in Docker) |
| VM #3 : ELK Stack Node 2 | Logstash, Kibana (in Docker) | 
| VM #4 : Log Shipper / Collector Node | Filebeat, rsyslog, Docker (optional, for testing input) | 
| VM #5 : Firewall / Router Log Generator | pfSense, iptables, and simulated logs | 

---

