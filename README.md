# Merkle Tree Implementation in C (Using Hash Table + BST)

This project implements a simplified version of a **Merkle Tree** using a **Hash Table** where each bucket is a **Binary Search Tree (BST)**. It allows insertion, deletion, search, and display operations while keeping track of the structure's size.

## What is a Merkle Tree?

A Merkle Tree is a hash-based data structure used in blockchain, databases, and file systems for efficient and secure verification of content. This simplified version uses a hybrid approach combining hashing with binary search trees.

## Features

- Each key-value pair is stored in a BST at a hashed index.
- Operations include:
  - Insert
  - Delete
  - Find
  - Display contents
  - Check tree size
- Uses **hashcode(key % max)** to determine index in the hash table.

## How It Works

- The `struct bst` represents each hash table slot containing a `head` pointer to a BST.
- The `hashcode()` function computes the index for a given key.
- Nodes in the BST are inserted or searched based on binary search logic.
- A menu-based interface allows users to interactively test the structure.

## Compilation & Execution

### Compile the code:
  gcc -o merkle_tree merkle_tree.c
### Run the Executable
  ./merkle_tree

