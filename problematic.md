# Problematic

For example, we want to use Linux (or any other system) on a Windows system. That is something possible with a virtual machine. And that works well on computers or machines with high performance, or on servers.
So in companies, they use servers, and they buy parts of the server — like running a Windows on Windows. You connect to the server, and then you access your part.
In another way, they give you a [`virtual machine`](./virtual-machine.md) inside a server.

## Disadvantages of Virtual Machines
- Eats RAM
- Eats CPU
- Eats Disk Space

## Container 

- An isolated environment forruning an application.
- They don't need a full OS.
- Share the OP of the host.
- Start quickly.
- Need less hardware ressources.

## Comparison between Bare Metal, Virtual Machine, and Container

| Term                     | Description                                  | Isolation                               | Performance                          | 
| ------------------------ | -------------------------------------------- | --------------------------------------- | ------------------------------------ | 
| **Bare Metal**           | Physical computer without virtualization     | No isolation (direct hardware)          | Best performance (direct access)     |
| **Virtual Machine (VM)** | Virtual machine with full OS on a hypervisor | Full isolation (each VM has its own OS) | Less performance (OS overhead)       | 
| **Container**            | Lightweight instance sharing the host OS     | Light isolation (shares OS kernel)      | Very good performance (low overhead) | 
