# Block Cipher Cryptosystem

Welcome to the repository for the **Modern Block Cipher Cryptosystem** project developed for SWE 314 — Software Security Engineering, Fall 2019. This project represents our efforts in designing and implementing a novel cryptosystem, showcasing various cryptographic techniques in Java.

## Project Overview

This project implements a custom block cipher designed to encrypt and decrypt data blocks of size 12. Our cryptosystem utilizes a combination of polyalphabetic substitution, transposition methods, and block manipulations to ensure secure data encryption and decryption.

## Key Features

- **Encryption Methodology**:
  - Processes a 12-character input string.
  - Applies a series of operations including one-bit right circular shifts, block swapping, and rail fence cipher with a depth of three.
  - Uses additive polyalphabetic substitution to adjust character ASCII codes based on their index positions.
  - Executes a total of 3 rounds of encryption to transform the plaintext into ciphertext.

- **Decryption Methodology**:
  - Reverses the encryption process to recover the original 12-character input.
  - Performs operations including rail fence decryption, block swapping, and right circular shifts.
  - Applies a reverse additive technique to adjust character ASCII codes based on their index positions.

## Detailed Cipher Mechanics

- **Encryption**:
  1. Divides the 12-character text into 3 blocks of 4 characters each.
  2. Performs a one-bit right circular shift on the first block.
  3. Swaps the second and third blocks.
  4. Combines blocks using a rail fence cipher technique.
  5. Applies additive polyalphabetic substitution based on index positions.

- **Decryption**:
  1. Applies reverse additive substitution based on index positions.
  2. Divides the encrypted text into 3 blocks of 4 characters each.
  3. Reverses the block swapping operation.
  4. Performs a three-bit right circular shift on the blocks.
  5. Reconstructs the original text using rail fence decryption.

## Learning Outcomes

Throughout this project, we not only achieved our goal of implementing a cryptosystem but also gained valuable insights into Java programming, cryptographic principles, and efficient project management. This experience helped us appreciate the balance between creativity and practical constraints in software development.
