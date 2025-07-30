# Hashcat Password Cracking Demo

This demo shows how to use Hashcat to crack password hashes using a dictionary attack. It focuses on command-line usage and understanding password security concepts rather than writing custom code on Kali Linux.

## What It Does

- Generates a SHA1 password hash (e.g., for "password123")
- Used `tape.txt` to crack the hash using a dictionary attack

## Requirements

- [Hashcat](https://hashcat.net/hashcat/)
- A dictionary file like [tape.txt](https://github.com/brannondorsey/naive-hashcat/releases/download/data/tape.txt)

## How to Use

1. Save the target hash in `hash.txt`
2. Run Hashcat:

```bash
hashcat -m 100 -a 0 hash.txt Documents/tape.txt
