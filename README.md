# Basic_Blockcahin
Building the Block Class in Python 🐍
Now we are ready to turn this concept into Python code! To work with SHA-256 in Python, we use the built-in hashlib 📚 library.

To generate a hash for a block, we must first combine all of its details into one single text string, and then convert that string into bytes before hashing it.

Here is a quick look at how hashlib computes a SHA-256 hash:

Python
import hashlib

# Example data string
data_string = "01/01/2026Hello Blockchain"

# 1. Encode string to bytes, 2. Hash it, 3. Convert to 64-character hex string
block_hash = hashlib.sha256(data_string.encode()).hexdigest()
