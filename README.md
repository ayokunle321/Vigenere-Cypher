# Vigenere Cipher Decryption with Key Guessing

## Purpose

This Python code implements a Vigenere cipher decryption tool capable of decrypting a given ciphertext (encrypted text) using a short key. Additionally, the code includes functionality to guess the key used for encryption based on the frequencies of characters in the English language.

## Functionality

The code provides the following functions:

1. `decrypt(text, key)`: This function takes a ciphertext and a short key as input and decrypts the text using the Vigenere cipher. The Vigenere cipher is a method of encrypting alphabetic text using a simple form of polyalphabetic substitution. It iterates through each character in the text and the key, performs the decryption calculation, and returns the decrypted text.

2. `get_frequencies(text)`: This function obtains the relative frequency of each character (in uppercase) in the given text. It computes the relative frequencies of each character in the provided `ALPHABET` and returns a dictionary containing these frequencies.

3. `cross_entropy(freqs1, freqs2)`: This function compares two dictionaries of frequencies (`freqs1` and `freqs2`) and calculates their cross entropy. Cross entropy is a measure of how similar two probability distributions are. The function computes the cross entropy between the relative frequencies of the characters in the dictionaries and returns the result as a float.

4. `guess_key(encrypted)`: This function guesses the key used to encrypt the provided encrypted text based on the frequencies in the English language. It analyzes the relative frequencies of each character in the encrypted text, comparing them to the frequencies of characters in English text. The function returns a key consisting of three characters as a string.

5. `crack(encrypted_text)`: This function decrypts the given encrypted text using the guessed key obtained from `guess_key`. It decrypts the text using the Vigenere cipher with the guessed key and returns the decrypted text as a string.

## Execution

To use the Vigenere cipher decryption tool, follow these steps:

1. Ensure the `math` module is imported at the beginning of the script.

2. Run the Python script containing the provided code.

3. The program will prompt you to provide an encrypted text. Enter the ciphertext to be decrypted.

4. The program will display the decrypted text along with the guessed key used for decryption.

## Notes

- The code uses a fixed `ALPHABET` string, containing all the characters considered for encryption and decryption. The input text and key should consist of characters from this `ALPHABET`.

- The code is designed to work with the Vigenere cipher encryption, where the key is a short string and must be known to the user.

## References and Resources

For more information on the Vigenere cipher and cross entropy, you can refer to the relevant resources and research papers.

## Contact

If you have any questions or feedback regarding the Vigenere cipher decryption tool, feel free to reach out. You can find me on GitHub: [github.com/yourusername](https://github.com/ayokunle321).

