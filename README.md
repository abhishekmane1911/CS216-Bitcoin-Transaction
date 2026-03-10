# CS 216: Bitcoin Transaction Lab Assignment

## Team Members

* Mane Abhishek Ganesh (240001043)
* Chetan Verma (240001022)
* Dhoke Vinod Eknath (240001025)
* Sahil Hedaoo (240041032)
---

## Project Overview

This project demonstrates how Bitcoin transactions work using:

* **Legacy Transactions (P2PKH)**
* **SegWit Transactions (P2SH-P2WPKH)**

The programs interact with **Bitcoin Core (bitcoind)** using RPC to create, sign, and broadcast transactions. The results are then analyzed to compare script structures and transaction sizes.

---

## Installation

Install required Python libraries:

```
pip install -r requirements.txt
```

Ensure **Bitcoin Core** is installed and running in **regtest mode** using the provided `bitcoin.conf`.

---

## Running the Programs

### Part 1 – Legacy Transactions (P2PKH)

```
cd Part1_Legacy
python part1.py
```

This program:

* Creates legacy addresses
* Sends transactions A → B → C
* Decodes the transaction scripts

---

### Part 2 – SegWit Transactions (P2SH-P2WPKH)

```
cd Part2_SegWit
python part2.py
```

This program:

* Creates SegWit addresses
* Sends transactions A’ → B’ → C’
* Analyzes SegWit transaction scripts

---

### Part 3 – Analysis

The comparative analysis between Legacy and SegWit transactions is provided in the report:

```
Part3_Analysis/report.pdf
```

The report includes:

* Transaction workflow
* Script analysis
* Transaction size comparison (bytes, vbytes, weight)
* Explanation of SegWit efficiency

---

## Repository Structure

```
Part1_Legacy/
Part2_SegWit/
Part3_Analysis/
bitcoin.conf
requirements.txt
README.md
```

---
