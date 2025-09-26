# VMWare and Hyper-V Overview Guide

**Description/Overview:** VMWare (unless otherwise mentioned, this article is specifically in reference to *vSphere* and *ESXi*, a foundational technology upon which *vSphere* is built) and Microsoft's *Hyper-V* are bare-metal hypervisors that create virtual machines (VMs). Both VMWare technologies and Hyper-V are common solutions for professional deployments, but they have more than a few key differences (such as their operating environments, costs, and integrations with guest OSes). While most VMWare solutions are intended for mid-to-large scale organizations (which may be more capable of paying expensive licensing fees) with a diversity of operating system needs and compatibilities (e.g., Windows, MacOS, various Linux distributions), Hyper-V is a common free solution for Windows-specific OS environments.

#### Table of Contents

1. [Hyper-V Overview](#hyperv)
2. [VMWare Overview](#vmware)
3. [Contrasting Three VMWare Components](#threevm)
4. [VMWare vs. Hyper-V: A Comparison](#comparison)
5. [Choosing a Bare-Metal Hypervisor](#choosing)
6. [Supplemental Resources](#supplemental)

<hr />

## 1. <a name="hyperv">Hyper-V Overview</a>

*Hyper-V* is Microsoft's virtualization platform solution (allowing for the creation and oversight of virtual machines on Windows systems), and an integrated, low-cost (and often bundled) component of Windows Server OSes. It features a practical and beginner-ready user interface (UI), fluent integration with other Microsoft software and hardware, and other technical conveniences: migrations without interruptions or downtime ('live migrations'), virtual networking capabilities, and dynamic memory allocation, for example.

While Hyper-V is utilized by many different kinds of enterprises, it is not natively non-Windows OS/platform friendly (although basic Linux VMs, for example, can be configured and executed). Sometimes, such as when advanced features are required for VMs, Hyper-V is not even compatible with non-Windows OSes.

<hr />

## 2. <a name="vmware">VMWare Overview</a>

(TODO)

<hr />

## 3. <a name="threevm">Contrasting Three VMWare Components</a>

| *Consideration* | *VMWare ESXi* | *VMWare vCenter* | *VMWare vSphere* |
| :---: | :---: | :----: | :----: |
| What is It? | A bare-metal hypervisor/platform for virtualization.	| Utility for centralized server infrastructure oversight.	| Product family containing virtualization management tools and assistive software. |
| What's the Goal? | Virtual machine configuration, deployment and execution on independent host devices. | Oversee ESXi servers and server clusters in a centralized manager that allows for pooling hosts. | Integrate the hypervisor and server management tools while providing additional functionality.  |
| Who Might Use It? | Popular for software testing, academic and research labs, and when hardware and native OS resources are limited. | Enterprise environments that oversee multiple servers. | Enterprises with scalability needs for their virtualized servers. |
| Does It Involve Payment? | Can be free, or paid with a vSphere license. | Paid with a vSphere license. | Licensing is set at various levels/tiers (e.g., Standard, Enterprise Plus). |
| To What Extent Does Payment Matter? | Free version lacks advanced functionalities and does not natively integrate with vCenter.	| Extent of scalability determined by particular license purchased. | Extent of various functionalities dependent upon license level/tier. |

<hr />

## 4. <a name="comparison">VMWare vs. Hyper-V: A Comparison</a>

| *Consideration* | *VMWare* | *Hyper-V* |
| :---: | :---: | :----: |
| Environment | vSphere provides comprehensive environments, based on complex licenses. Abundance of Cloud integrations and third-party utilities. | Firmly integrated with Microsoft utilities and Windows Server (which it is built upon). |
| Management and Architecture | Managed by Windows admins via VMWare vCenter Server, with a proprietary Unix-based kernel. | Managed via Hyper-V Manager, PowerShell, and similar utilities. |
| OS Integrations | Compatible with many OSes (traditional UNIX-based, traditional Linux-based, Cloud platforms, etc.). | Intended for Windows guest OSes, with limited compatibility for non-Windows OSes. |
| Performance and Scalability | High performance and scalability, intended for mid-to-large scale enterprises. | Potentially similar performance and scalability, but dedicated to Windows systems. |
| Pricing | Licensing plans/fees can be costly and complicated. | Either free or bundled into Windows Server licenses. |
 
<hr />

## 5. <a name="choosing">Choosing a Bare-Metal Hypervisor</a>

* *VMWare* may be a better choice if a bare-metal hypervisor is needed for a massive, enterprise-level organization that can sustain larger costs. Furthermore, if there are comprehensive support needs for diverse operating systems and a desire to host various third-party utilities in an interconnected environment, VMWare may be the more sensible choice.
* *HyperV* may be a better choice for organizations that run on Windows and would prefer to rely on Windows management utilities, and if cost consciousness is high.

<hr />

## 6. <a name="supplemental">Supplemental Resources</a>

* *[Intro to Data Center Virtualization Overview Guide](https://github.com/chaseofthejungle/intro-to-data-center-virtualization/)*
* *[Ubiquiti and Cisco Meraki Overview Guide](https://github.com/chaseofthejungle/unifi-vs-cisco-meraki)*
* *[Intro to IP Telephony Overview Guide](https://github.com/chaseofthejungle/intro-to-ip-telephony)*
