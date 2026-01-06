# Marlowe Smart Contract – Conditional Deposit & Payment

##  Overview
This repository contains a **Marlowe smart contract** developed as part of my learning journey through the **EBU program**.  
The contract demonstrates a **conditional deposit and payment flow** between two parties using ADA on the Cardano blockchain.

The goal is to showcase how Marlowe enables **clear, secure, and time-bound financial agreements**.

---

##  Contract Logic (High-Level)
The contract involves two roles:
- **Olivier**
- **Mwatsimulamo**

### Flow:
1. Olivier deposits **2000 ADA** into the contract before a defined deadline.
2. After that, Mwatsimulamo deposits **1500 ADA** before a second deadline.
3. If both deposits are completed successfully:
   - **2000 ADA are automatically paid to Mwatsimulamo**
   - The contract closes.
4. If any deposit is not made within its deadline:
   - The contract closes safely without unintended execution.

---

## Time Constraints
The contract uses **POSIX timestamps** to enforce deadlines:
- First deadline: Olivier’s deposit
- Second deadline: Mwatsimulamo’s deposit

These time constraints ensure predictability and reduce counterparty risk.

---

## Technology
- **Blockchain:** Cardano
- **Smart Contract Language:** Marlowe DSL
- **Development Tool:** Marlowe Playground
- **Token Used:** ADA

---
