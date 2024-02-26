# Building Resilient Web Infrastructure: A Multi-Server, Load-Balanced Architecture

This project tackles the challenge of establishing a robust and scalable web infrastructure, capable of serving across multiple servers and platforms. Imagine a scenario where your website experiences a surge in traffic, threatening its stability and performance. This project equips you with the tools to navigate such situations with confidence.

The Heroes of the Story:

* Nginx Web Servers (Heroes A, B, C): These valiant servers act as the workhorses, tirelessly serving web pages to users. Each hero boasts its own unique hostname, IP address, and port, ready to handle incoming requests.
* HAProxy (The Wise Leader): This strategic leader orchestrates the web-serving operation. It functions as a load balancer, intelligently distributing incoming traffic amongst the Nginx servers, ensuring optimal performance and preventing any one server from being overwhelmed.
* Bastion Host (The Gatekeeper): This vigilant guardian serves as the sole entry point for Secure Shell (SSH) access to the internal network. It acts as the first line of defense, protecting the core servers from unauthorized access.

The Intricate Plot:

* Deployment: Five hosts play crucial roles in this narrative: HAProxy, Heroes A, B, and C, and the Bastion. HAProxy stands tall as the entry point, while the Bastion serves as the gateway to the internal network.
* SSH Key Generation: To ensure secure communication between the servers, an SSH key pair is generated. The public key is distributed to the servers, granting authorized access.
* SSH Configuration: The SSH configuration file on each server is meticulously crafted, specifying the IP addresses of its peers and the path to the private SSH key. This configuration enables secure
  communication and collaboration between the servers.
  
## The Impact:

This project empowered me to:

* Enhance Scalability: Effortlessly handle increased traffic by distributing the load across multiple servers.
* Boost Resilience: Mitigate the impact of server failures, as HAProxy seamlessly redirects traffic to available servers.
* Strengthen Security: Implement secure access to the internal network through the Bastion host and SSH key authentication.
  
By implementing this multi-server, load-balanced architecture, you lay the foundation for a robust and secure web infrastructure, capable of weathering any storm and delivering exceptional performance under pressure.
