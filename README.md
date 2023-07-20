# AirAnchor: UAV Tracking

## Overview

AirAnchor is a project that explores the implementation of a blockchain-based solution for tracking and storing data related to Unmanned Aerial Vehicles (UAVs). The primary goal is to create a global, decentralized, and secure database that enables transparent auditing of all UAV-related activities without the need for intermediaries.

## Motivation

The exponential increase in the use of UAVs by both companies and individuals has led to the necessity of establishing a regulatory and traffic management entity to avoid collisions and ensure safe UAV operations. The Unmanned Aircraft System Traffic Management (UTM) serves as the central controller, responsible for supervising UAV traffic and providing route instructions to prevent collisions.

However, merely relying on regulations and a supervisory body is insufficient to handle the vast amount of data and scenarios that can arise in this environment. Thus, the need arises for a comprehensive tracking and data storage system that records all drone actions, commands, and locations. Similar to the black box in aircraft, this approach enables tracking the last UAV records in case of accidents, analyzing data to identify risks, implementing preventive measures, or enforcing regulatory compliance.

## Objectives

The main objective of this study is to investigate the viability of using blockchain technology for data storage, satisfying the tracking and registration needs mentioned earlier. To achieve this goal, the project aims to:

* Deploy a blockchain infrastructure that ensures immutable and distributed data registration, considering the resource constraints and real-time requirements of the UAV use case.
* Adapt the blockchain infrastructure to a Kubernetes environment, leveraging its features.
* Design and implement a scalable solution for both storing and querying the data saved in the blockchain.
* Evaluate the solution's performance and scalability in terms of transactions per second, latency, and storage capacity, considering different usage scenarios and workloads.
* Contribute valuable insights to the UAV management field and blockchain technology.
  
## Project Modules

* Gateway: The Gateway module serves as the interface for handling UAV data and interactions with the blockchain. It receives data from UAVs, processes it, and forwards it to the relevant components for storage and validation. It also manages the communication between the UAVs and the blockchain network.
* DronApi: DronApi is a critical component that provides the necessary APIs and endpoints for the UAVs to interact with the system. It enables UAVs to send data and receive instructions from the blockchain network. The DronApi module acts as the primary communication channel for the UAVs.
* CA (Certificate Authority): The Certificate Authority module is responsible for managing security certificates for the UAVs and other network entities. It ensures secure communication and authentication between the UAVs and the blockchain network, enhancing the overall security of the system.
* Keeper: The Keeper module is responsible for listening for events of validated transactions in the ledger and sending notifications to the gateway.
* TP (Transaction Processor): The Transaction Processor module handles the processing of incoming transactions from UAVs. It executes smart contracts and applies the necessary business logic to validate and record UAV-related transactions in the blockchain.
* Kubernetes Files: This module contains the necessary configuration files and scripts for deploying the blockchain infrastructure in a Kubernetes environment. It ensures seamless integration with Kubernetes, enabling easy scalability and management of the system.


Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue in this repository.

License

This project is licensed under the MIT License.

Thank you for your interest in UAV Tracking using Blockchain. We hope this solution contributes to establishing a secure and efficient environment for UAV operations and inspires further innovations in the field of blockchain technology.
