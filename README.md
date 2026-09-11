<img width="1419" height="736" alt="Gemini_Generated_Image_rwqrxjrwqrxjrwqr" src="https://github.com/user-attachments/assets/58c98f92-36a0-442a-b707-478b40602949" /># NETWORKWALKS-SHAHABASUSMANAK-B083-WK1-PM1-CYBERSECURITY-LAB-SETUP
# Cybersecurity Hands-On Lab Setup

> Building a secure, isolated sandbox environment for ethical hacking and defensive security training.

---

## 📌 Project Overview

This project walks through the process of building a private, virtual cybersecurity laboratory from scratch. By using VirtualBox alongside Kali Linux, this setup provides a safe, contained space to practice vital security skills. 

Inside this isolated network, you can safely perform core cybersecurity tasks like:
* Network Scanning to find active devices.
* Reconnaissance to gather vital system data.
* Vulnerability Assessments to scan for weak spots.
* Security Testing to practice ethical hacking methods over and over without risking real-world systems.

The entire environment runs on a customized, private network layout. This makes it incredibly easy to attach more target machines or vulnerable systems later on as your testing needs grow.

---

## 🎯 Core Objectives

The primary goals accomplished in this project are:
* Deploy and Configure VirtualBox as the main virtualization manager.
* Import and Initialize Kali Linux to serve as the primary security operating system.
* Establish a Custom NAT Network to guarantee secure, isolated communication between lab machines.
* * Set up network access for the Kali Linux machine.
* Give a permanent IP address to your Kali Linux virtual machine (VM).
* Test the internet connection and check that DNS (website names) works correctly.
* Save a clean system backup (snapshot) so you can easily reset the lab if anything breaks.
* Write clear notes on how the whole environment was built.
* Get the system ready to handle more advanced security labs in the future.

---

## 🛡️ Why We Build This Lab

This lab gives you a secure, locked-down digital workspace. It is a completely safe zone built for hands-on learning and approved security testing. 

You can use this lab setup to practice things like:
* Information Gathering: Finding out what systems are running on a network.
* Port Discovery: Checking which digital doors or entry points are open.
* Weakness Hunting: Finding software gaps that need to be patched or fixed.
* Traffic Inspection: Looking closely at data moving across a network.
* Web Security Testing: Checking website code for flaws.
* Ethical Exploitation: Learning how hackers break into systems so you can defend against them.
* Tool Testing: Trying out different cybersecurity software programs to see how they work.

---

## ⚠️ Crucial Safety Warning

Important Note: This laboratory setup must only be used to interact with machines that you legally own or have written permission to test. Never use these tools or methods to scan or attack computers that do not belong to you!
---

## 🏗️ Lab Architecture

Below is the network topology map designed for this virtual environment. It outlines the master host system, the hypervisor engine, and the isolated target subnet layout.

<!-- Replace the text below with your actual image path or URL -->
http://1-screenshot-title-image.png/

### 💻 Base Host Specifications
* Operating System: Windows 10/11 (Main Host)
* IP Configuration: Dynamic / Assigned by local router
* Hardware Profile: 8GB RAM minimum, 256GB SSD storage, Core i3 processor (or equivalent modern CPU)

### 🌐 Network & Virtual Machine Mapping
All guest machines communicate within an isolated, customized NAT Network configured on a designated private IP pool.

* Lab Subnet Range: 10.0.0.2 to 10.0.0.254

#### 🎯 Configured Machines:
1. Kali Linux VM (Attacker Machine):
   * IP Assignment: 10.0.0.2 (Static / Manual)
   * Network Mode: Custom NAT Network

2. Target Node Scalability:
   * Additional systems (such as Windows 10, Windows 11, Server platforms, or legacy endpoints) can easily be provisioned into the 10.0.0.X scope.
   * Provides flexible architecture to scale out attack scenarios for future cybersecurity training modules.

---

## ⚙️ Lab Configuration
