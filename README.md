# 🎣 A phishing demo using Zphisher tool in a controlled lab environment
## Type: Ethical Hacking / Threat Simulation
🔍 Overview
This project focused on understanding real-world phishing techniques by simulating attacks in a controlled lab using Zphisher. I used it to replicate how attackers host phishing pages and distribute malicious URLs through different channels.
# PROJECT SUMMARY
### I carried out this project using Zphisher to demonstrate how phishing attacks are typically carried out in real-life scenarios. I explored different methods attackers use to deliver phishing links, including email, SMS (smishing), social media, QR codes, and even compromised websites. I also used tools like Ngrok and URL shorteners to simulate how these links are shared and how victims might interact with them. Everything here was done in a controlled environment strictly for learning and awareness purposes. The aim was to understand both the attack side and how defenders (like SOC teams) can detect and stop these threats.
## 📦 Tool Used
- [Zphisher](https://github.com/htr-tech/zphisher)
🧰 What I Did
#### I updated Kali to ensure it has the latest version
![image](https://github.com/user-attachments/assets/7e03ab69-ce5e-42e3-917f-49ade74febec)
#### I created a new folder on kali and named it Zphisher using:
#### Installed and configured Zphisher in a Kali Linux environment using: https://github.com/htr-tech/zphisher
#### Generated phishing pages and used services like Ngrok, Serveo, and LocalTunnel to host them.
![image](https://github.com/user-attachments/assets/05e99d6b-dd63-48b8-8e1c-b310df9a83e9)
![image](https://github.com/user-attachments/assets/ccdf5293-ff86-4981-97d4-d101de866941)
![image](https://github.com/user-attachments/assets/e20e6e1c-59c2-4102-8879-8a7a682128bc)
![image](https://github.com/user-attachments/assets/51cb1952-db8c-4daf-be31-34a1ad1a703f)

#### Once a phishing page is hosted (like with Zphisher), the attacker gets a URL (often using services like ngrok, serveo, or localtunnel), which they need to deliver to the victim. 
![image](https://github.com/user-attachments/assets/a6a08af1-2443-490b-b7e8-0b4f3bc65821)
![image](https://github.com/user-attachments/assets/d96b3e52-e7d4-43c4-b612-f4fd54333c78)
![image](https://github.com/user-attachments/assets/e8db4e20-a7c4-477f-a74f-31ed800c23b2)
![image](https://github.com/user-attachments/assets/a43e94a1-45ba-4ead-a64f-52e7cdf74edd)
![image](https://github.com/user-attachments/assets/39f8c2dd-ca6c-4edf-92d5-697ce265780b)

#### Here's how they typically do that:

Simulated phishing delivery methods:

📧 Email (with spoofed addresses and fake login prompts)
The attacker sends a socially engineered email with
  #### Fake login links (e.g., “Your account has expired, log in here”)
  #### Embedded malicious URLs masked with text or images
  #### Spoofed sender addresses (e.g., support@yourbank.com)


📱 Smishing (phishing via SMS)
Attackers send short links via SMS pretending to be:
  #### Banks 
  #### Delivery companies (e.g., FedEx, DHL, Uber, Door Dash,)
  #### Government or tax agencies

💬 Chat and social media impersonation
They might:
#### Send the link on Facebook, WhatsApp, Telegram, or Discord
#### Impersonate a known contact or tech support
________________________________________


🧾 QR code phishing
Attackers convert the malicious URL into a QR code and put it on:
####	Posters
####	Fliers
####	Email attachments
####	Fake "parking tickets" or "Wi-Fi access" signs
🌐 Redirects from compromised websites
### Instead of hosting a phishing page directly, the attacker:
#### Hacks a legitimate website and uploads the phishing site
#### open redirects (e.g., legit.com/redirect?url=malicioussite.com)
#### Embeds hidden phishing forms on forums, blogs, etc.
📢 Malvertising (fake ads leading to phishing sites)
####	Fake ads on shady websites that redirect to phishing pages
#### Often used with typosquatting domains

 🔐 How to Defend (SOC Perspective)
#### Look for unusual outbound URLs in proxy logs
#### Flag URL shorteners or ngrok/serveo domains
#### Use email filters for phishing keywords and known attacker templates
#### Use Zero Trust access and enforce MFA
🧠 Learning Outcome
#### Gained hands-on experience with phishing infrastructure setup.
#### Understood phishing vectors from both attacker and SOC (defensive) perspectives.
#### Identified detection points for phishing campaigns in proxy and email logs.
⚠️ I carried out this project ethically and in a closed test environment for learning purposes only.







