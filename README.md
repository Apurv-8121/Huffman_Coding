# Huffman_Coding
Implemented the Huffman coding which is a lossless data compression algorithm, which used data 
structures like trees and linked-list.
The provided code is an implementation of the Huffman coding algorithm in Python. Huffman coding is a compression technique used to represent characters in a string with variable-length codes, where more frequent characters are assigned shorter codes. Here's a summary of the code:

1. **User Input**:
   - The code starts by taking user input for a string.

2. **NodeTree Class**:
   - It defines a `NodeTree` class to create tree nodes for building the Huffman tree.
   - Each node can have a left child and a right child.

3. **`huffman_code_tree` Function**:
   - This function recursively builds the Huffman code tree.
   - It takes a node as input and assigns binary codes to characters based on their position in the tree.
   - The function returns a dictionary where keys are characters, and values are their corresponding Huffman codes.

4. **Frequency Calculation**:
   - The code calculates the frequency of each character in the input string and stores it in a dictionary called `freq`.

5. **Sorting Frequencies**:
   - The frequencies are sorted in descending order to prioritize characters with higher frequencies.

6. **Huffman Tree Construction**:
   - The code constructs the Huffman tree by repeatedly merging nodes.
   - It starts with the nodes representing characters and their frequencies.
   - In each iteration, it combines the two nodes with the lowest frequencies into a new node and updates the list of nodes.
   - This process continues until there is only one node left in the list, which represents the root of the Huffman tree.

7. **Huffman Code Generation**:
   - The `huffman_code_tree` function is called to generate Huffman codes for each character.
   - The Huffman codes are stored in the `huffmanCode` dictionary.

8. **Output**:
   - The code prints the characters, their frequencies, and their corresponding Huffman codes in a tabular format.

9. **Summary Output**:
   - The summary of the characters, frequencies, and Huffman codes is displayed as a table.

The code essentially takes an input string, calculates the Huffman codes for each character in the string, and displays the results, showing how the characters can be encoded efficiently. It provides a simple demonstration of the Huffman coding algorithm.
