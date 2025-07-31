# HydraStrike 🌊

![HydraStrike Banner](https://raw.githubusercontent.com/RedHydra/HydraStrike/main/assets/banner.png) 
<!-- You can create a banner and upload it to your repo to use here -->

**A sophisticated and dynamic attack execution platform that automatically analyzes targets, configures, and optimizes multi-vector attacks in real-time.**

---

### ⚠️ Disclaimer

This tool is intended for **educational and authorized security testing purposes only**. The author is not responsible for any illegal or malicious use of this tool. Using HydraStrike against targets without prior mutual consent is illegal. **Always respect the law and ethical guidelines.**

---

## ✨ Features

* **🎯 Intelligent Target Analysis:** Automatically scans the target to identify open ports, services, and optimal attack vectors.
* **🚀 Multi-Vector Attacks:** Employs a combination of attack methods (Layer 4 and Layer 7) for maximum impact.
    * HTTP Flood
    * HTTPS Flood
    * Slowloris
    * TCP Flood
    * UDP Flood
* **📊 Live Attack Interface:** Provides a real-time terminal UI displaying crucial statistics:
    * Attack Duration
    * Total Requests & Data Sent
    * Requests per Second & Live Bandwidth
    * Success Rate
    * Active Attack Methods
* **⚙️ Dynamic Configuration:** Adjusts attack parameters like thread count based on target analysis.
* **🎨 Colorful & Clean UI:** Uses color-coded output for better readability and a professional feel.
* **🐍 Cross-Platform:** Written in Python, making it compatible with most operating systems.

---

## 🚀 Getting Started

### Prerequisites

* [Python 3.x](https://www.python.org/downloads/)
* `pip` (Python package installer)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/HydraStrike.git](https://github.com/YOUR_USERNAME/HydraStrike.git)
    cd HydraStrike
    ```

2.  **Install the required Python libraries:**
    ```bash
    pip install -r requirements.txt
    ```
    *(You will need to create a `requirements.txt` file containing `requests`)*

---

## Usage

The script is straightforward to use. The primary argument is the target, which can be a domain name or an IP address.

### Basic Syntax

```bash
python3 HydraStrike.py <target> [options]
```

### Arguments

| Argument     | Description                                         | Default |
|--------------|-----------------------------------------------------|---------|
| `target`     | **Required.** The target domain or IP address.      | N/A     |
| `--duration` | The duration of the attack in seconds.              | 60      |
| `--threads`  | The number of threads to use per attack method.     | Dynamic |

### Examples

1.  **Launch a default attack on a domain:**
    * This will run a 60-second attack with dynamically configured methods and threads.
    ```bash
    python3 HydraStrike.py example.com
    ```

2.  **Launch an attack on an IP address for 3 minutes (180 seconds):**
    ```bash
    python3 HydraStrike.py 192.168.1.100 --duration 180
    ```

3.  **Launch an attack with a specific number of threads per method:**
    * This overrides the dynamic thread configuration.
    ```bash
    python3 HydraStrike.py secure-target.net --threads 250
    ```

---

## ⚔️ Attack Methods

HydraStrike combines several attack methods to stress-test network infrastructure and web servers.

| Method       | Type      | Description                                                                                             |
|--------------|-----------|---------------------------------------------------------------------------------------------------------|
| **HTTP/HTTPS Flood**| Layer 7   | Sends a high volume of legitimate-looking GET requests to overwhelm a web server's resources.       |
| **Slowloris** | Layer 7   | Establishes many connections to the target server and holds them open by sending partial requests, exhausting the server's connection pool. |
| **TCP Flood** | Layer 4   | Inundates the target with SYN packets, attempting to consume all available connection resources.        |
| **UDP Flood** | Layer 4   | Floods random ports on the target host with UDP packets, causing the server to check for applications listening and respond with ICMP "Destination Unreachable" packets. |

---

## 🖼️ Screenshots

*(Here you can add screenshots of the tool in action)*

**Live Attack Interface:**
![Live Interface Screenshot](https://raw.githubusercontent.com/RedHydra/HydraStrike/main/assets/interface.png)
<!-- Add a screenshot of the terminal UI -->

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Crafted with ❤️ by RedHydra**
