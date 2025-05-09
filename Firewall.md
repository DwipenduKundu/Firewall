# Firewall

## Introduction

A **firewall** is either a software application or a dedicated hardware device that acts as a barrier between a trusted internal network and an untrusted external network, such as the internet. Its primary role is to screen out unauthorized access attempts, including those from hackers, viruses, and worms.

Firewalls regulate the flow of data between networks of varying trust levels—such as your highly trusted home network and the untrusted internet—to ensure that only legitimate traffic is allowed.

## Software vs Hardware Firewalls

### Software Firewall

* Installed directly on a personal computer or device.
* Monitors and filters traffic specific to that device.
* Available by default in most modern Windows operating systems (XP SP2, Vista, 7, 8, 10, and 11).
* Important for protecting individual devices, especially if one system in a network becomes infected.

### Hardware Firewall

* A physical device that connects between your local network and the internet.
* Provides centralized protection for all devices in the network.
* Essential when multiple devices are connected to the same network.

> 🔒 **Best Practice:** Use both software and hardware firewalls together. This layered security approach ensures device-level and network-level protection.

## Core Functionality of Firewalls

* All incoming and outgoing traffic is evaluated by the firewall.
* Each message must meet predefined security rules.
* Compliant messages are allowed through; others are blocked.

Disabling the firewall removes this protection and leaves your system vulnerable. A common reminder:

> "Today you might be a billionaire, but without protection, tomorrow you could be a beggar. Never turn your firewall off."

## How Firewalls Work: Real-World Example

Imagine you're using a browser like Google Chrome and type in `www.example.com`:

* Your request goes to the internet.
* The server hosting the website (say, Bob's computer) responds with the content.
* Meanwhile, a hacker’s computer (let's call it Sam) tries to intercept and send malicious data.

If Sam’s IP is on the firewall’s block list (access control list), the firewall prevents any data from reaching your system. This filtering process is known as **packet filtering**.

### Session Awareness

Firewalls also track active sessions. If you’re watching a video on YouTube, the firewall logs the legitimate communication. Should a hacker attempt to inject data mid-stream, the firewall blocks it—because the intrusion isn’t part of the original, verified session. This is how firewalls ensure consistent, safe browsing.

## Understanding Data Packets

All data transferred over a network is broken into **packets**—small chunks of information containing:

* Actual data (called the payload)
* Source and destination IP addresses

Breaking down data improves reliability and speed, making firewalls' role in inspecting each packet essential for robust security.

## Types of Firewalls

### 1. Packet-Filtering Firewall

* The simplest and most foundational firewall type.
* Evaluates packets individually based on:

  * Source and destination IP
  * Port numbers
  * Protocols (TCP, UDP, etc.)
* Operates at the **network layer (Layer 3)** of the OSI model.

**How it works:**

* Allows packets that match approved criteria.
* Blocks those that don’t.

### 2. Proxy Firewall (Application-Level Gateway)

* Works at the **application layer**.
* Acts as an intermediary between your device and the internet.

**How it works:**

* Intercepts user requests.
* Filters traffic according to rules.
* Forwards valid requests and responses securely.

### 3. Hybrid Firewall

* Combines features of:

  * Packet-filtering
  * Stateful inspection
  * Proxy firewalls
* Delivers broad, layered security.

**How it works:**

* Filters based on IP and port (like packet-filtering).
* Tracks active sessions (stateful inspection).
* Examines data at the application level (like a proxy).
* May also include IDS/IPS and VPN capabilities.

## Limitations of Firewalls

### Software Firewalls

* May impact system performance.
* Only protect the host device.
* Can be disabled by malware or user error.
* Require technical knowledge to configure properly.
* Less suitable for large networks.

### Hardware Firewalls

* More costly to purchase and maintain.
* Setup can be complex.
* Do not protect against threats from within the network.
* If the firewall fails, the whole network becomes vulnerable.
* Require periodic firmware updates.

## Conclusion

Choosing the right type of firewall depends on your specific needs:

* **Hardware firewalls** are ideal for centralized protection across multiple devices.
* **Software firewalls** provide critical security for individual endpoints.

For the strongest protection, a combination of both is recommended, ensuring a **layered defense** against cyber threats in both personal and professional settings.

