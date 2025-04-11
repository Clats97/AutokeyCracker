# AutokeyCracker
This Python script decrypts ciphertext encrypted with the Vigenere Autokey cipher. The script automates the decryption process by testing candidate keywords from a file until a decrypted message is detected as a valid English sentence.

# Vigenère Autokey Cracker

## Key Features

- **ASCII Art Header:**  
  Displays an ASCII art header with the tool's name, version, and author's signature.

- **Autokey Decryption:**  
  Implements the `autokey_decrypt` function that:
  - Starts with an initial keyword.
  - Extends the decryption key by appending each successfully decrypted letter.
  - Decrypts letters by performing modulo arithmetic on their positions in the alphabet.

- **English Sentence Verification:**  
  Uses NLTK’s English words corpus to verify if the decrypted output is a valid English sentence. The function `is_english_sentence` checks the ratio of recognized words, ensuring only likely valid decryptions are flagged.

- **Brute-Force Keyword Testing:**  
  The script reads candidate keywords from a user-specified file (default: `passkeys.txt`) and attempts decryption with each keyword. Once a decryption produces an output that meets the English language threshold, it displays the successful candidate keyword along with the decrypted plaintext.

- **Interactive User Interface:**  
  Runs in a loop, prompting the user for ciphertext and passkeys file path, providing an easy-to-follow command-line interface.

## Prerequisites

- **Python 3.x**
- **NLTK (Natural Language Toolkit):**  
  Install via pip:
  pip install nltk

  **Author**
Joshua M Clatney (Clats97)
Ethical Pentesting Enthusiast

Copyright 2025 Joshua M Clatney (Clats97)
