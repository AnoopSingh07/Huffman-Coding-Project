
# Huffman Compression & Decompression Utility

**Project Duration:** August 2024 - September 2024

## Objective
The primary objective of this project is to develop an efficient algorithm for lossless data compression using Huffman coding techniques.

## Description
This project implements a Huffman encoding and decoding algorithm in C++. The utility is capable of compressing text files by up to 50%, while ensuring data integrity is preserved. The compression and decompression processes are achieved through the generation of optimal prefix codes using binary trees and priority queues.

### Key Features:
- **Huffman Encoding:** Compresses input files by creating a binary tree and generating optimal prefix codes.
- **Huffman Decoding:** Accurately reconstructs the original file from its compressed format using the generated Huffman tree.
- **Core Functionalities:** 
  - Construction of the Huffman tree.
  - Management of priority queues.
  - File input/output operations.
- **Metadata Handling:** Efficient encoding and decoding with proper management of binary-to-decimal conversions and Huffman tree reconstruction.
- **Extensive Testing:** The utility has been tested across diverse text datasets to ensure both efficiency and correctness.

## Usage

### Compilation
To compile the encoding and decoding programs, use the following commands:

```bash
g++ -o encode encode.cpp huffman.cpp
g++ -o decode decode.cpp huffman.cpp
```

### Running the Program
To compress a file:

```bash
./encode inputFile.txt outputFile.huf
```

To decompress the file:

```bash
./decode outputFile.huf decodedFile.txt
```

## Files in the Repository

- **encode.cpp**: The main file for encoding (compression).
- **decode.cpp**: The main file for decoding (decompression).
- **huffman.cpp**: Implementation of the Huffman algorithm and associated functions.
- **huffman.hpp**: Header file containing declarations for the Huffman algorithm.
- **inputFile.txt**: Sample input file for testing compression.
- **outputFile.huf**: Output file after compression.
- **decodedFile.txt**: File generated after decompression, should match the original input file.
- **.vscode/settings.json**: Configuration file for the Visual Studio Code environment.
