tags: #networking


# OSI model

- The OSI (open system interconnected) model is a framework that standardizes how different network protocols work together. its broken down into 7 layers , each with their own specific role.

- #### Layer 7: Application Layer
- This layer is closest to the user and interact with software applications to provide communication services.

- #### Layer 6: Presentation layer 
- This layer is responsible for translating data into a format that the application layer can understand. It deals with encryption/decryption (e.g., [[SSL]]/[[TLS]]), data compression, and character encoding (e.g.,[[ UTF-8]]).

- #### Layer 5: Session layer 
- Manages the establishment, maintenance, and termination of communication sessions. This layer is responsible for maintaining sessions during the communication process (e.g., the **[[3-way handshake]]** in TCP).

- #### Layer 4: transport layer
- Responsible for ensuring complete data transfer. It can use **[[TCP (Transmission Control Protocol]]** for reliable communication or **[[UDP (User Datagram Protocol)]]** for faster, less reliable communication (like in video streaming or VoIP). TCP guarantees delivery and order, while UDP is more about speed, sacrificing error-checking.

- **Layer 3: Network Layer**  
- Handles **IP addressing** and routing of packets. The most commonly used protocol at this layer is **IP (Internet Protocol)**, which assigns IP addresses to devices and routes packets through the network.

- **Layer 2: Data Link Layer**  
- Responsible for **data transfer** between two directly connected nodes. It ensures error-free transfer by handling media access control (MAC addressing) and data framing. It manages how devices on a network communicate over a physical medium like Ethernet.

- **Layer 1: Physical Layer**  
- This is the hardware layer, responsible for the **physical connection** between devices. It includes the medium (e.g., copper cables, fiber optics, radio waves) and how the data is encoded onto the medium (e.g., voltage levels, signal modulation).

### Mnemonic :
- Please - Physical layer 
- Do  - Data layer 
- Not - Network Layer 
- Throw - Transport Layer
- Sausage - Session Layer
- Pizza - presentation layer
- Away - Application layer 


# Revision Questions 

- 1. **What does the OSI model stand for and what is its purpose?**
    
    - The OSI model stands for **Open Systems Interconnection** model. Its purpose is to standardize the networking framework to allow different systems to communicate with each other, ensuring interoperability between different devices and protocols.
	
1. **Name all seven layers of the OSI model in order from Layer 1 to Layer 7.**
    
    - 1. Physical
    - 2. Data Link
    - 3. Network
    - 4. Transport
    - 5. Session
    - 6. Presentation
    - 7. Application
    
1. **What is the main responsibility of the Physical layer (Layer 1) in the OSI model?**
    
    - The Physical layer handles the **transmission of raw bit streams** over a physical medium (such as cables or radio waves). It defines hardware, like cables, switches, and voltage levels.
    
1. **What is the role of the Data Link layer (Layer 2)? Give an example of a protocol that operates at this layer.**
    
    - The Data Link layer is responsible for **node-to-node data transfer** and error detection and correction. It also manages MAC (Media Access Control) addressing. An example of a protocol at this layer is **Ethernet**.
    
1. **Which OSI layer is responsible for routing data and IP addressing?**
    
    - The **Network layer (Layer 3)** is responsible for **routing data** and **assigning IP addresses** to packets. The main protocol at this layer is **IP (Internet Protocol)**.
    
1. **Describe the difference between TCP and UDP. Which OSI layer do they operate at?**
    
    - **TCP** (Transmission Control Protocol) provides **reliable** data transmission with error-checking, acknowledgments, and ordered delivery. **UDP** (User Datagram Protocol) is **faster** but less reliable, with no guarantees on delivery or order. Both operate at the **Transport layer (Layer 4)**.
    
1. **Which layer in the OSI model is responsible for session management and how does it contribute to communication?**
    
    - The **Session layer (Layer 5)** manages the **establishment, maintenance, and termination** of communication sessions between devices. It ensures that the session is maintained for as long as needed, such as during file transfers or video calls.
    
1. **Explain the role of the Presentation layer (Layer 6). What is it responsible for in terms of data format?**
    
    - The Presentation layer is responsible for **data translation, encryption, and compression**. It formats data into a suitable form for the Application layer, handling things like **character encoding (UTF-8)** and encryption (e.g., **SSL/TLS**).
    
1. **What services and protocols are found in the Application layer (Layer 7)? Provide two examples.**
    
    - The Application layer provides end-user services and interacts with software applications. Examples include **HTTP/HTTPS** (for web browsing) and **SMTP** (for sending emails).
    
1. **At which layer would encryption typically occur in the OSI model?**
    
    - **Encryption** typically occurs at the **Presentation layer (Layer 6)**, although it can also happen at other layers depending on the implementation (e.g., TLS operates between Layers 4 and 7).