<div align="center">
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Animals/Hydra.png" alt="Hydra" width="120" height="120" />
</div>

<h1 align="center">
<svg width="420" height="50" xmlns="http://www.w3.org/2000/svg">
<style>
.text {
font-family: 'Courier New', Courier, monospace;
font-size: 35px;
font-weight: bold;
fill: #E84D4D; /* Red color /
animation: typing 3.5s steps(11, end), blink-caret .75s step-end infinite;
white-space: nowrap;
overflow: hidden;
border-right: .15em solid #FFC436; / Blinking cursor */
width: 0;
}
@keyframes typing {
from { width: 0 }
to { width: 410px }
}
@keyframes blink-caret {
from, to { border-color: transparent }
50% { border-color: #FFC436; }
}
</style>
<text x="10" y="40" class="text">HydraStrike v1.0</text>
</svg>
</h1>

<p align="center">
<strong>A Dynamic Attack Execution Platform</strong>
</p>

HydraStrike is a sophisticated, Python-based attack execution platform designed to automatically configure and optimize network attacks in real-time. It intelligently analyzes the target and unleashes a multi-headed assault for maximum effectiveness.

<pre>
<code class="language-bash">
<span style="color: #00ffff;">  _    _           _            _____ _        _ _         </span>
<span style="color: #00ffff;"> | |  | |         | |          / | |      () |       </span>
<span style="color: #00ffff;"> | |__| |   _  | | __ __ | ( | | _ __ | | _____ </span>
<span style="color: #00ffff;"> |  __  | | | |/  | &#39;__/ _ |_ | | '| | |/ / _ \ </span>
<span style="color: #00ffff;"> | |  | | || | (| | | | (| |) | || |  | |   &lt;  __/ </span>
<span style="color: #00ffff;"> ||  ||_,|_,||  _,|_____/ _||  ||_|___| </span>
<span style="color: #00ffff;">          / |                                            </span>
<span style="color: #00ffff;">         |/                                            </span>
<span style="color: #ff0000;">v1.0 - Dynamic Attack Platform</span>
</code>
</pre>

Disclaimer: This tool is intended for educational and authorized security testing purposes only. Unauthorized use of this tool against any system is illegal. The author is not responsible for any misuse or damage caused by this tool.

✨ Features
🎯 Smart Target Analysis: Automatically scans the target to identify open ports and running services (HTTP, HTTPS, etc.).

⚙️ Optimal Configuration: Dynamically determines the best attack methods and parameters based on the target's profile.

💣 Multiple Attack Modules:

HTTP Flood: Overwhelms web servers with a high volume of requests.

Slowloris: Ties up server resources by sending partial HTTP requests.

TCP Flood: Saturates the target with TCP packets.

UDP Flood: Floods the target with UDP packets.

📺 Live Terminal Interface: Provides a real-time console view of attack statistics with vibrant, color-coded output.

🚀 Multi-threaded Power: Utilizes a thread pool to execute multiple attack vectors simultaneously.

💻 Simple CLI Control: Easy-to-use command-line interface to define your target, attack duration, and thread count.

🛠️ Installation
Clone the repository or download the HydraStrike.py script.

Install the necessary Python dependencies:

pip install -r requirements.txt

▶️ Usage
To launch an attack, simply provide a target domain or IP address.

Command-Line Arguments
# General Syntax
python HydraStrike.py <target> [--duration <seconds>] [--threads <count>]

target: (Required) The domain name or IP address of the target.

--duration: (Optional) The duration of the attack in seconds. Default: 60.

--threads: (Optional) The number of threads per attack method. Default: Auto-configured.

Examples
# Run a default 60-second attack on example.com
python HydraStrike.py example.com

# Run a 5-minute (300 seconds) attack on an IP address
python HydraStrike.py 192.168.1.100 --duration 300

# Force an attack with 200 threads per method
python HydraStrike.py testserver.local --threads 200

📊 Live Attack Interface
Watch the attack unfold in real-time with a colorful and detailed statistics panel.

<pre>
<code class="language-bash">
<span style="color: #ffff00;">[!] HydraStrike - Dynamic Attack Execution Platform</span>
<span style="color: #ffff00;">[!] Author: RedHydra</span>
<span style="color: #ffff00;">[!] Press Ctrl+C to stop the attack</span>

<span style="color: #0000ff;">[+] Target Information:</span>
Host: example.com
IP: 93.184.216.34
Open Ports: 80, 443
Services: HTTP, HTTPS

<span style="color: #0000ff;">[+] Attack Statistics:</span>
Duration: 35.12 seconds
Total Requests: 175600
Data Sent: 167.47 MB
Requests/sec: 4999.89
Bandwidth: 4.77 MB/s
Success Rate: 99.82%

<span style="color: #0000ff;">[+] Active Attacks:</span>
HTTPS Flood on port 443: <span style="color: #00ff00;">RUNNING</span>
HTTP Flood on port 80: <span style="color: #00ff00;">RUNNING</span>
Slowloris on port 443: <span style="color: #00ff00;">RUNNING</span>
Slowloris on port 80: <span style="color: #00ff00;">RUNNING</span>

<span style="color: #ffff00;">[+] Attack in progress...</span>
</code>
</pre>
