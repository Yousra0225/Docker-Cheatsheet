# 📦 Containers Cheatsheet

## What is a Container?

- A **lightweight, isolated** environment to run applications.
- **Shares the host OS kernel**, unlike virtual machines.
- Starts fast, uses fewer resources.

## Kernel

A kernel is a computer program at the core of computer's OS, that has complete control over everything in the system, including managing aplications and hardware ressources.

##  Kernel & Containers

| Concept                       | Description                                                                                         |
| ----------------------------- | --------------------------------------------------------------------------------------------------- |
| **Host Kernel**               | The core part of the host OS. Containers **share** this kernel.                                     |
| **No kernel in container**    | Containers **do not include** their own kernel.                                                     |
| **Same kernel type required** | A container must be compatible with the host's kernel type.                                         |
| **Linux host**                | Can only run **Linux containers** (directly).                                                       |
| **Windows host**              | Can run: <br> → **Windows containers** (natively) <br> → **Linux containers** (via Hyper-V) |
| **Isolation level**           | Containers are **process-level isolated**, not hardware-level like VMs.                             |

---

