# SOC Automation Lab

## Description
This lab is a comprehensive project that builds a fully functional SOC environment from scratch, integrating Wazuh for SIEM and XDR, The Hive for case management, and Shuffle for SOAR capabilities. It highlights expertise in creating a streamlined security ecosystem capable of detecting, managing, and responding to threats with automated workflows and real-time alerting.

The project focuses on:

- Setting up infrastructure in a cloud or virtual environment.
- Configuring and integrating multiple cybersecurity tools.
- Automating detection, containment, and response processes.
- Developing a scalable and functional lab environment, similar to those used in enterprise-level SOCs.

## Key Features of the Lab

**1. Complete SOC Simulation:**

  - Integration of Wazuh (SIEM), The Hive (case management), and Shuffle (SOAR) tools to mimic real-world operations.
  - End-to-end workflow from alert generation to automated response.

**2.  Hands-On Automation:**

  - Implementation of automation for incident detection, containment, and notification processes.
  - Demonstrates problem-solving skills and the ability to streamline SOC operations.

**3. Cloud-Based or Local Deployment:** 

  - Flexibility to deploy in cloud environments or local virtual machines, depending on available resources.
  - Highlights adaptability and knowledge of different infrastructure setups.

 **4. Telemetry Simulation:** 

  - Generation of realistic threat scenarios (e.g., Mimikatz activity) to test alerting and response capabilities.
  - Ensures tools are tested under practical conditions.

**5. Scalability and Customization:**

  - The lab can be scaled and enhanced with additional automation scripts and features, showcasing innovation beyond the basics.

**6. Enterprise-Grade Practices:**

- Simulates professional SOC workflows, including alert tracking, case assignment, and cross-team communication.
- Sends automated email notifications to analysts for incident updates.

**7. Documentation and Portfolio:**
- Includes logical diagrams, setup instructions, troubleshooting notes, and key observations, making it an ideal project to feature in a professional portfolio.

## Lab Topology 

![adf](https://i.imgur.com/v1cyhs3.png)

**Explanation:**

**1. Send Events:** 
 
  - The Wazuh Agent (Windows 10 Client) will send events to the internet (the cloud).

**2. Receive Events:**
  
  - Wazuh receives the events that the Windows 10 Client sent.

**3. Send Alerts:**
  
  - Wazuh sends an alert to Shuffle for enrichment and orchestration purposes.

**4. Enrich Events:**
  
  - Shuffle enriches the events.

**5. Send Alerts:**
  
  - Shuffle sends an alert to TheHive to facilitate case management and incident tracking.

**6. Send Email:**
  
  - Shuffle also sends an email alert to the SOC Analyst.

**7. Send & Receive Email:**
  
  - The SOC Analyst receives and reads the contents of the email.

**8. Send Response Action:** '
  
  - The SOC Analyst sends the response action to the internet (the cloud). Next, the cloud routes the response action to Shuffle. After, Shuffle sends the response action to Wazuh. Finally, Wazuh delivers the response action to the Windows 10 Client who originally sent the events. 

