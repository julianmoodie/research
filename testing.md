# Ransomware Incident Analysis & Recovery Report

## Abstract
This report documents a ransomware incident analysis conducted in a controlled environment. It focuses on execution behavior, persistence mechanisms, encryption workflow, and defensive response strategies.

---

## 1. Attack Overview

The ransomware follows a standard multi-stage attack chain:

- Initial execution (user-triggered)
- Payload unpacking
- System reconnaissance
- File encryption
- Cleanup + persistence attempts

---

## 2. Attack Chain Diagram

![Attack Flow](images/attack-flow.png)

> Figure 1: High-level ransomware execution lifecycle

---

## 3. Execution Process Tree

![Process Tree](images/process-tree.png)

### Observations:
- Dropper spawns multiple child processes
- Process masquerading observed (system-like names)
- High file-system enumeration activity

---

## 4. Execution Flow (Technical Breakdown)
