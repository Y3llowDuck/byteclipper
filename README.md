# ByteClipper

A minimalist Bash script to generate a clean, single-line C# reverse https shell payload using `msfvenom`, and copy it directly to your clipboard.  
Ideal for red teamers, CTF players, and security researchers who need fast and formatted payloads without manual cleanup.

Once executed, the script extracts only the byte array from the generated payload, removes newlines, and stores it to your clipboard — perfect for pasting into .NET loaders or other tools.

---

## ✨ Features

- **Generates C# Reverse HTTPS Shell Payload**  
  Uses `msfvenom` to create a `windows/x64/meterpreter/reverse_https` payload.

- **Cleans the Output**  
  Extracts just the byte array from the C# payload and formats it into a one-liner.

- **Clipboard Support**  
  Automatically copies the final result to your clipboard via `xclip`.

- **Lightweight & Fast**  
  A single Bash script that does the job in seconds.

---

## ⚙️ Prerequisites

- [`msfvenom`](https://www.metasploit.com/) – from the Metasploit Framework  
- [`xclip`](https://linux.die.net/man/1/xclip) – clipboard tool for X11 (Linux)  
- Bash shell environment

Install dependencies on Debian/Ubuntu systems:

```bash
sudo apt install metasploit-framework xclip

