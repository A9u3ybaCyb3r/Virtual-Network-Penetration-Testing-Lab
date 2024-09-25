# Virtual-Network-Penetration-Testing-Lab

## Objective

The lab focuses on providing a safe and controlled space to practice various security skills, including network security, penetration testing, and defensive strategies. By building virtual machines and configuring a network with a firewall, you can simulate real-world scenarios and gain hands-on experience with security tools and techniques.

### Skills Learned

- Virtualization: Installing and configuring VirtualBox software, creating and managing virtual machines (VMs), allocating resources to VMs, and installing guest operating systems.
- Network Security: Understanding network concepts (VLANs, subnets, IP addressing), configuring virtual networks with pfSense firewall, setting up network segmentation, and implementing network security controls.
- Penetration Testing: Importing pre-configured vulnerable machines (VulnHub) and Kali Linux for practicing penetration testing techniques.
- Active Directory: Building a simulated Active Directory environment to understand directory services and practice potential attack vectors.
- Security Analysis: Utilizing tools like pfSense firewall for network traffic control.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used


- VirtualBox: A virtualization software platform used to create and manage virtual machines.
- pfSense: An open-source firewall software used to create a secure network gateway for the virtual lab environment.
- Kali Linux: A Linux distribution pre-loaded with various security and penetration testing tools.
- VulnHub: A repository of pre-configured vulnerable virtual machines for practicing penetration testing techniques.
- Windows Server:
- Windows 10: 

## Steps

### Planning Phase
1. First we will build a network diagram to represent our lab visually.
   
![image](https://github.com/user-attachments/assets/8805a3cd-25cb-4cd1-a185-f5291bd3dc3c)
 
 *Ref 1: Network Diagram*

### Building a pfSense VM

1. First we download the file that we need. 
 - Go to this link: https://www.google.com/search?q=site%3A*.netgate.com+download+-site%3Aforum.netgate.com+-site%3Adocs.netgate.com+-inurl%3Ablog+-site%3Awww.netgate.com+-site%3Ashop.netgate.com+-site%3Aforums.netgate.com+-site%3Ainfo.netgate.com&ref=benheater.com

Choose this one. 

![image](https://github.com/user-attachments/assets/b1c3be2d-a7dd-437d-af8d-3af6658d3056)


Then we choose the latest version.

![image](https://github.com/user-attachments/assets/4510c75a-d8b6-4821-ae6d-df8d84c0bf3a)


2. Extract the file, in this case I will be using 7-zip.

![image](https://github.com/user-attachments/assets/b395d9a3-6e1c-4d7d-a32f-352084f731eb)

3. Create a New Machine

![image](https://github.com/user-attachments/assets/a1bed139-45f7-4864-9d89-74ef542fc0cc)

Name your vm, choose the folder that you want to save the machine, choose the iso image that you want to use, select the type and version of the VM.

![image](https://github.com/user-attachments/assets/fa7194ac-cf8c-44f5-882e-62213f7dc89d)

![image](https://github.com/user-attachments/assets/56b00275-2a31-4da9-8535-45e44f417f51)

![image](https://github.com/user-attachments/assets/bf359848-201f-438d-992a-66db8d18b070)

![image](https://github.com/user-attachments/assets/e73ca9a0-ee82-4aff-83a5-d966640e2c60)

!!Do not start the VM yet!!

4. Go to the settings of the machine

![image](https://github.com/user-attachments/assets/783117c5-c6c4-42d2-81c3-d70b5ce5d8fb)

Change the boot order and match it as in the image shown below. Also, uncheck the Floppy Disk 
This will ensure that the operating system boots upon installation from the disc.

![image](https://github.com/user-attachments/assets/f69d55aa-465c-4616-a2cb-ceac898494ef)

Go to the audio settings and disable the audio

![image](https://github.com/user-attachments/assets/0677dd7d-2d4d-4383-8697-01d8fe5b8c04)

Go to the USB settings and disable it.

![image](https://github.com/user-attachments/assets/96c4257b-b5aa-416e-a86a-2f23360f1d0c)

5. Configure the Network Interface

Still on the machine settings go to the Network settings.

![image](https://github.com/user-attachments/assets/f21163f3-85dc-4176-a402-9eb705f61631)

Adapter 1 WAN:

![image](https://github.com/user-attachments/assets/7ba13507-0c08-4ce8-a7a5-48591123ad08)

Adapter 2 LAN:

![image](https://github.com/user-attachments/assets/924e9715-78d5-45ba-8176-7dcb7d878862)

Adapter 3 ISOLATED:

![image](https://github.com/user-attachments/assets/7f6f4678-f46f-4344-8b99-9b39a45d55cf)

Adapter 4 AD-LAB:

![image](https://github.com/user-attachments/assets/7fe81f34-1f06-443e-bbaf-251de2fc6024)

After doing all of this we can start the machine.


### Importing Kali 

1. Go to https://kali.org/get-kali/
   - Click on the image that says Virtual Machines and download the 64-bit version of Virtualbox

      ![image](https://github.com/user-attachments/assets/ae2d558e-57a4-4d1a-8576-5ad25de659ec)
     
     ![image](https://github.com/user-attachments/assets/6430026d-9ca1-46db-9dd6-98e6d758617c)



### Configuring the pfSense firewall

### Importing Vulnhub VMs to the lab

### Building an Active Directory

### Building a Pivoting Lab
