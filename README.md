# SECURED - EPITECH (Elementary Programming in C)

## Custom hash function and C library for managing a secure hashing table

## 🔐 Project Overview

Secured is a project focused on implementing hash tables in C,

serving as an introduction to data structures and hashing techniques.

The goal is to create a secure storage system for important data by

developing a custom hash function and handling collisions effectively.

## 📌 Features

Custom hash function implementation
Creation and management of hash tables
Support for insertion, deletion, and searching of key-value pairs
Collision handling using separate chaining
Implementation of a library (libsecured.a)

## ⚙️ Installation & Usage
##### Prerequisites

Ensure you have the necessary tools installed:

    sudo apt-get install gcc make

##### Building the Project

To compile the project, use the provided Makefile:

    make

To clean up object files:

    make clean

To remove compiled binaries and object files:

    make fclean

##### Running the Secured System

To execute the program:

    ./secured

## 📂 Project Structure

    ├── src/                     #    Source code for hash table functions
    │   ├── delete_hashtable.c       #    Freeing hash table memory
    │   ├── hash.c                   #    Custom hash function
    │   ├── ht_delete.c              #    Deletion logic
    │   ├── ht_dump.c                #    Dumping hash table contents
    │   ├── ht_insert.c              #    Insertion logic
    │   ├── ht_search.c              #    Searching in hash table
    │   ├── main.c                   #    Entry point
    │   ├── new_hashtable.c          #    Creating a new hash table
    │
    ├── include/                 #    Header files
    │   ├── hashtable.h              #    Hash table structure and functions
    │   ├── my.h                     #    Custom utility functions
    │
    ├── lib/                     #    Library files
    │   ├── my/                      #    Custom utility functions library
    │
    ├── Makefile                 #    Build script
    ├── README.md                #    Project documentation

## 🚀 Example Usage

##### Creating a Hash Table

    hashtable_t *ht = new_hashtable(&hash, 10);

##### Inserting Data

    ht_insert(ht, "Key1", "Some important data");

##### Searching for Data

    char *value = ht_search(ht, "Key1");
    printf("Value: %s\n", value);

##### Deleting Data

    ht_delete(ht, "Key1");

##### Dumping the Hash Table

    ht_dump(ht);

## 📌 Compilation Rules

The project is compiled using make
Only write, malloc, and free are authorized functions
The executable should return 84 on errors.

## 👨‍💻 Author

Arthur VIGNES – Developed for EPITECH 2024.

## 🏛️ License

This project is for educational purposes as part of the Elementary Programming in C module at EPITECH.
