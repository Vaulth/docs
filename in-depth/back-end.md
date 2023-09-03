---
description: In-depth documentation on vaulth back-end
---

# Vaulth Back-end

# Vaulth's Back-end Introduction:

Vaulth's backend is the engine that fuels the entire ecosystem, facilitating the secure and efficient exchange of data between users and the blockchain. This crucial 
component ensures the integrity of certificates and stamps, providing, through Express.js, SQL, and JavaScript, the Vaulth experience.

## Centralized Data Management

To centralize access and manage data effectively, our backend connects to both an IPFS node and the Ethereum blockchain. It actively listens to contract events and 
stores specific data accordingly. This approach optimizes API calls and enhances the overall reliability of our solution.

# Let's go deeper into how these technologies !

## Express.js
At the core of Vaulth's backend is **Express.js**, a versatile and scalable web application framework built on Node.js. Express.js is the architectural framework that 
governs the flow of data between Vaulth's front-end platforms and the blockchain. 

**Explanation:** Express.js is a popular Node.js web application framework known for its simplicity and flexibility. It's often used for building robust and scalable 
server-side applications. In the context of Vaulth, Express.js serves as the backend framework to handle incoming HTTP requests and facilitate communication between 
the client-side applications and the blockchain.

**Impact on Vaulth:** Express.js provides a robust and efficient way to handle API requests from Vaulth's front-end platforms. It allows developers to define routes 
and controllers for interacting with the Vaulth contract on the blockchain. This technology ensures that data retrieval and updates from the blockchain are 
streamlined and accessible to the user interface.

<!-- Push example of api roots and how to call it with postman -->

## SQL (Structured Query Language)
While Vaulth securely stores all data of stamps and certificates on the blockchain and IPFS, the heart of our backend infrastructure is **SQL**, the industry-standard 
language for managing relational databases. SQL serves as a vital repository for certificates, stamps, user accounts, and other critical application data. With SQL, 
Vaulth ensures data integrity, consistency, and reliability, enabling efficient data storage, retrieval, and modification. This guarantees that users' certificates 
and stamps are securely stored and readily accessible when needed.

**Explanation:** SQL is a domain-specific language used for managing and querying relational databases. It provides a standardized way to interact with databases, 
performing data retrieval, insertion, modification, and deletion operations.

**Impact on Vaulth:** Within Vaulth's backend, SQL is employed to manage and store various types of data related to certificates, stamps, users, and other application-specific information. While all stamps and certificates are originally stored on the blockchain and IPFS for security and authenticity, SQL is used to create a secondary copy of this data. This copy enhances data retrieval times, ensuring a responsive user experience. This approach is crucial for efficiently managing user accounts, certificates, and other information required for Vaulth's functionality.


## JavaScript

**JavaScript**, renowned for its adaptability and ubiquity in web development, plays a pivotal role in Vaulth's backend logic. It brings together the various backend 
components, including Express.js and the blockchain contract interaction. JavaScript powers the server-side logic, enabling validation, data formatting, and custom 
responses. Moreover, specialized JavaScript libraries and frameworks, such as web3.js for blockchain interactions, facilitate seamless communication with the Vaulth 
contract. This ensures that the data retrieved from the blockchain is presented accurately and securely to users across the Vaulth platform.

**Explanation:** JavaScript is a widely used programming language for web development. It's known for its versatility and is commonly used for both client-side and 
server-side scripting. In the context of Vaulth's backend, JavaScript is used to develop server-side logic and interact with the blockchain contract.

**Impact on Vaulth:** JavaScript is the glue that connects various components of Vaulth's backend, including Express.js and the interaction with the blockchain 
contract. It allows for the creation of custom logic to handle user requests, validate data, and format responses. Additionally, JavaScript libraries and frameworks 
specific to blockchain interactions (such as web3.js for Ethereum) are used to facilitate communication with the Vaulth contract. This ensures that data from the 
blockchain is accessible and can be presented to users through the frontend platforms.

# Interaction with the Vaulth Contract

- The backend development utilizes web3.js to interact with the Vaulth contract deployed on the blockchain (e.g., Ethereum).
- Smart contracts define the core logic of Vaulth, including certificate creation, stamping, and endorsement.
- The backend communicates with the contract to retrieve data such as certificate information, user endorsements, and stamp details, allowing the frontend platforms 
- to display up-to-date and authenticated data to users.


In summary, the backend development of Vaulth is crucial for bridging the gap between the frontend user interfaces and the blockchain contract. Technologies like 
Express.js, SQL, and JavaScript enable efficient data management, routing, and interaction with the Vaulth contract, ensuring a seamless and secure user experience 
within the Vaulth ecosystem.


## Backend Deployment and API

In terms of deployment, our application is hosted on Amazon EC2, coupled with the capabilities of Cloud 66. EC2 provides a user-friendly Virtual Private Server (VPS) 
service, offering storage and computational power. Cloud 66 complements EC2 by facilitating instance management, continuous deployment, testing, firewall configuration, permissions, and an intuitive online interface for server administration.

Together, these technologies form the backbone of Vaulth's backend, enabling secure and efficient interactions with blockchain and IPFS while ensuring the reliability 
and scalability of our art authentication platform.

