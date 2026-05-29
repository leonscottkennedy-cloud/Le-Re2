⚡ SmartDNS — Boost Your Game, Block the Noise
<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android-green?style=for-the-badge&logo=android"/>
  <img src="https://img.shields.io/badge/Language-Java-orange?style=for-the-badge&logo=java"/>
  <img src="https://img.shields.io/badge/Min%20SDK-21-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/License-MIT-purple?style=for-the-badge"/>
</p>
<p align="center">
  A smart DNS changer for Android that <b>reduces ping in online games</b> like Call of Duty Mobile,<br/>
  while staying dead simple for casual users and fully featured for power users.
</p>

🎯 Why SmartDNS?
Most DNS apps are either too simple (just change DNS, done) or too complex (overwhelming for regular users). SmartDNS is different:

🟢 One tap to find & apply the fastest DNS for your network
📊 Real ping stats — see before/after results
🔒 DNS over HTTPS (DoH) support for privacy
🛡️ Ad & tracker blocking built-in
🧪 Benchmark mode — test multiple DNS servers simultaneously
📋 Query log — see exactly what your apps are resolving


📱 Screenshots

Coming soon


🚀 Features
For Regular Users
FeatureDescription🎮 Game ModeOne-tap optimization for low-latency gaming⚡ Auto Best DNSBenchmarks and picks the fastest server automatically📶 Ping DisplayLive before/after ping comparison
For Power Users
FeatureDescription🔧 Custom DNSAdd any DNS server manually🔐 DoH / DoTEncrypted DNS support📋 Query LogFull DNS request logging🚫 BlocklistsImport custom blocklists🌐 Per-App DNSSet different DNS per app

🏗️ Architecture
app/
├── ui/
│   ├── MainActivity.java          # Main dashboard
│   ├── BenchmarkActivity.java     # DNS speed test
│   └── SettingsActivity.java      # Advanced settings
├── service/
│   ├── DnsVpnService.java         # Core VPN service
│   └── DnsResolver.java           # DNS resolution engine
├── model/
│   ├── DnsServer.java             # DNS server model
│   └── PingResult.java            # Benchmark result model
└── utils/
    ├── DnsBenchmark.java          # Multi-server benchmarking
    └── NetworkUtils.java          # Network helpers

🛠️ Built With

Java — Android development
VpnService API — Local VPN tunnel for DNS interception
OkHttp — DNS over HTTPS requests
Room — Local database for query logs
Material Design 3 — Modern UI components


⚙️ How It Works
SmartDNS creates a local VPN tunnel on your device (no data leaves your phone to any VPN server). All DNS queries are intercepted and forwarded to the fastest DNS server found during benchmarking.
App Request → SmartDNS VPN Tunnel → Fast DNS Server → Response
                     ↑
              (all local, on-device)

📦 Installation
From Release

Download the latest .apk from Releases
Enable "Install from unknown sources"
Install and enjoy

Build from Source
bashgit clone https://github.com/YOUR_USERNAME/SmartDNS.git
cd SmartDNS
./gradlew assembleDebug

🗺️ Roadmap

 Project setup
 Core VPN service
 DNS benchmarking engine
 Basic UI (one-tap mode)
 DoH support
 Ad blocking
 Per-app DNS rules
 Widget support
 Play Store release


🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first.

📄 License
MIT — free to use, modify, and distribute.

<p align="center">Made with ❤️ for gamers</p>
