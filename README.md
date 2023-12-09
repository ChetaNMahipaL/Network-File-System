# Network File System (NFS) Implementation Project

## Overview

This project demonstrates the development of a Network File System (NFS) comprising clients, a Naming Server (NM), and multiple Storage Servers (SS). The NFS allows seamless file operations within a networked environment.

## Key Features

- **Client Operations:** Initiate file-related tasks such as reading, writing, deletion, and file/folder creation.
- **Naming Server (NM):** Manages directory structure and facilitates client interactions with SS.
- **Storage Servers (SS):** Handle storage, file operations, and client communication.

## Highlights

- **Dynamic Functionality:** Allows addition of new Storage Servers during runtime.
- **Error-Resilient:** Equipped with error handling and distinct error codes for troubleshooting.
- **Concurrent Access:** Supports multiple client interactions without blocking.
- **Redundancy & Replication:** Implements data redundancy and replication for fault tolerance.

## Usage

1. **Initialization:**
   - Start the NM followed by initializing SS_1 to SS_n.

2. **Client Interaction:**
   - Use provided scripts to perform file operations.
   - Follow communication protocols with NM and SS.

3. **Advanced Features:**
   - Explore concurrent access, optimized searches, and data replication.

# Setup

1. Clone this repository / Download the zip file
2. Change into the directory
3. Run `bash setup.sh` to generate test cases
4. Run `make` to compile files for naming server, storage server and client.
5. Run naming server by executing `./nm.out`, storage server by executing `./ss.out` and client by executing `./client.out`

## Makefile commands

- `make / make all` : Compiles files for naming server, storage server and client
- `make client` : Compiles only files for client
- `make naming_server / make ns / make nm` : Compiles only files for naming server
- `make storage_server / make ss` : Compiles only files for storage server
- `make clean` : Deletes compiled `.out` executables
- `make clean_test_cases` : Deletes the `test_cases` directory.
- `make clean_log` : Deletes the `log_file.txt` file.
- `make reset` : Resets the directory to initial state deleting compiled executables, generated testcases and log file.

# Tests Run

### Basic Functioning

- [x] Read files
- [x] Read large files
- [x] Write to files
- [x] Get file info
- [x] Create file
- [x] Create folder
- [x] Delete file
- [x] Delete folder
- [x] Copy File
- [x] Copy folder

# Contributors

- [@Chetan Mahipal](https://github.com/MirageF458Italia)
- [@Kushal Shah](https://github.com/Kushal-Shah-03)
- [@Prithvi Karthik](https://github.com/Prithvi-k)
