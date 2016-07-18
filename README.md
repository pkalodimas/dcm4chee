#Remote Medical Diagnosis System
#Situation
Many radiological centers needing expert medical diagnosis by specialized doctors for better and more secure medical diagnosis. Specialized and experienced doctors are few in the local area and they cost a lot to be settle in the radiological center.
#Task
Specialized and experienced doctors can be hired to make medical diagnosis remotely and be paid according to the number of the diagnosis the offer. The doctor can work from his office in the city he lives and he also can offer his services two more than one radiological centers.
Every radiological center or hospital that uses medical devices that export medical images for the procedure of diagnosis (ex. ultrasound, axial tomography) needs to store the examinations images in a central server (PACS) and not locally in the medical devices so that the doctors can view the results of the medical device task and proceed to the patient medical diagnosis.
On remote diagnosis tasks the doctor has to be connected to the PACS server through the internet. This last task needs the existence of strong internet connections with high upload bandwidth that usually are not available by the ISPs.
The PACS server has to cover some security requirement like no one else except specific doctors can view patient’s medical examinations and also keep backups and examinations history archive. All these requirements are hold by the open source dcm4chee PACS server.
#Action
A very efficient PACS system that is offered by the open source community is the dcm4chee (www.dcm4chee.org). This PACS systems had to be set up and configured (users, image compression, backups, etc) in order to communicate with the medical devices and receive their medical data (DICOM protocol). This task has to be done in the local PACS server of every radiological center of hospital.
In order to solve the problem of low bandwidth ISPs connections and make the remote diagnosis task faster and simpler, the collection of all the medical examination of all the radiological centers in one PACS server (Main Server) is needed. A main server is located in an ISP data center offering
high internet connection and allowing the doctor to reach and download fast the large medical data examinations. For that reason all the local PACS server in the radiological centers have to be configured to forward their medical data to the main PACS server.
#Result
The result of this project is three radiological centers located in Rethimno (Crete, Greece), in Heraklio (Crete, Greece) and Pafos (Cyprus) to store their medical devices examinations in their local PACS servers keeping backups and history archive to be used locally by the resident doctors and simultaneously forward specific medical examinations in the main PACS server, located in a datacenter in Germany, to be used by the remote diagnosis doctor located in Heraklio (Crete, Greece).
#Tools
- Dcm4chee PACS system (Java)
- Weasis DICOM image viewer (Java)
- Java SDK
- CentOS Server 7 (Main)
- PostgreSQL Server (Main)
- Windows Server 2008 & 2012 OS (Locals)
- MySQL Server (Locals)