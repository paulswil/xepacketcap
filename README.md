# xepacketcap

Automate & secure packet captures on IOS XE devices using WT bots and Python APIs


## Business/Technical Challenge


Our goal is to enable Easy activation and storage of packet captures on Cisco IOS-XE routers and switches across the enterprise LAN.

Large Federal and Enterprise networks can support thousands of employees, contractors and partners, and mission-critical collateral worth billions of dollars. Delivery of network services for troubleshooting and ease of management are critical to managing a network of this size and breadth. The IOS-XE packet capture app can provide a flexible and scalable implementation for packet captures on any device platforms that host a GuestShell or other linux environments. The ability to capture and view the data from any of their devices quickly and accurately will provide a tremendous enhancement to  troubleshooting efforts. As customers refresh their entire network with newer technologies automation tools like this can position Cisco to the front of the line. Many customers do not have a virtual environment or applications making it very difficult for them to do automation or data collection without using external applications. This type of orchestration can help provide those tools to the customer within their own network. Executing a Wireshark capture on a specific device (router or switch) from a bot or web interface to a IOS-XE Guest shell and directing that data to a remote storage location can significantly simplify network troubleshooting or help the security team capture any interesting traffic. 


## Proposed Solution

The IOS-XE GuestShell provides a Linux environment from which router administration functions can be automated. One of the key troubleshooting tools available for network engineer is the packet capture, which provides a critical view into what data is actually traversing the network. When a network-based application is not working properly, the packet capture is a critical tool available in the effort to determine where things are going wrong. In the old times, network engineers had to SPAN a port that was connected to a physical capture host, such as a laptop running wireshark. But what if that laptop was moved to a new location? No capture for you. 

Fortunately, two innovations have made this problem moot. First, IOS-XE ships with Wireshark on-box. This allows network operators to run captures from the command line, and save them locally or remotely. Second, modern IOS-XE platforms ship with GuestShell installed. GuestShell is a general-purpose CentOS 7 container which provides a Linux shell that can be used to automate tasks on the device. Using python, the GuestShell can run commands on the IOS-XE host, including packet captures. 

The XE Packet Capture App is will accept capture parameters that are associated with the access-list (e.g. protocol, src/dst, duration) from a remote user interface, run the capture, and upload the resulting PCAP file to an AWS S3 host.

We will demonstrate packet capture. However, the possibilities for automating tasks through the GuestShell are endless. Repetitive tasks such as adding lines to ACLs, configuring IP SLA jobs, editing routing protocols, etc. can easily be automated.




### Cisco Products Technologies/ Services


Our solution will levegerage the following Cisco technologies

* Cisco IOS XE GuestShell (https://www.cisco.com/c/en/us/td/docs/ios-xml/ios/prog/configuration/167/b_167_programmability_cg/guest_shell.html)
* Webex Teams Bots

## Team Members


* Paul Wilson <paulswil@cisco.com> - Federal Civilian
* Luis Garcia <luigarc2@cisco.com> - Federal Civilian
* Chris Mader <chmader@cisco.com> - Enterprise


## Solution Components


<!-- This does not need to be completed during the initial submission phase  

Provide a brief overview of the components involved with this project. e.g Python /  -->


## Usage

<!-- This does not need to be completed during the initial submission phase  

Provide a brief overview of how to use the solution  -->



## Installation

How to install or setup the project for use.


## Documentation

Pointer to reference documentation for this project.


## License

Provided under Cisco Sample Code License, for details see [LICENSE](./LICENSE.md)

## Code of Conduct

Our code of conduct is available [here](./CODE_OF_CONDUCT.md)

## Contributing

See our contributing guidelines [here](./CONTRIBUTING.md)
