# Task-5-Elevate-Labs


---

### ✅ **Task**

Capture live network packets using Wireshark and identify at least three basic network protocols and traffic types.

---

### 🎯 **Objective**

To observe real-time network traffic, filter packets by protocol, and identify how different protocols operate at various layers of the network using Wireshark.

---

### 🧰 **Tools Used**

* **Wireshark** (for live packet capture and analysis)
* **Web Browser** (to generate HTTP traffic)
* **Command Prompt / Terminal** (to generate ICMP traffic using `ping`)

---

### 🧾 **Steps Followed**

1. **Selected Network Interface**

   * Opened Wireshark and selected the **active network interface** for live capture.
     *(Screenshot: `SelectInterface.png`)*

2. **Generated Traffic**

   * Visited websites using a browser to generate **HTTP and DNS traffic**.
   * Used `ping 8.8.8.8` to create **ICMP traffic**.
     *(Screenshot: `PingAndTrafficGeneration.png`)*

3. **Captured Packets**

   * Captured packets for about **1 minute** and then stopped the capture.
    

4. **Filtered by Protocols**

   * Used Wireshark filters to isolate protocol-specific traffic:

     * `http` for web requests *(Screenshot: `HTTPCapture.png`)*
     * `dns` for domain name queries *(Screenshot: `FilterByDNS.png`)*
     * `icmp` for ping packets *(Screenshot: `PacketsFilterByICMP(usingPing).png`)*
     * `tcp` for general TCP sessions *(Screenshot: `filterByTCP.png`)*

5. **Saved the Capture**

   * Exported the capture file in `.pcap` format.
     (Saved in kali by the name FIleSaved.png (the Screenshot shows the pcap file saved ))

---

### 🔍 **Protocols Identified**

| Protocol | Description                                                              | Example                                         |
| -------- | ------------------------------------------------------------------------ | ----------------------------------------------- |
| **HTTP** | Hypertext Transfer Protocol used to load websites.                       | GET request to `example.com`                    |
| **DNS**  | Domain Name System, used to resolve domain names into IPs.               | DNS Query for `google.com`                      |
| **ICMP** | Internet Control Message Protocol used for diagnostic tools like `ping`. | Echo Request/Reply with `8.8.8.8`               |
| **TCP**  | Transmission Control Protocol ensures reliable communication.            | Observed in almost all sessions, including HTTP |

---

### 📁 **Files Submitted**

* `FileSaved.png`
* `SelectInterface.png`
* `PingAndTrafficGeneration.png`
* `HTTPCapture.png`
* `FilterByDNS.png`
* `PacketsFilterByICMP(usingPing).png`
* `filterByTCP.png`
* `README.md`
  


