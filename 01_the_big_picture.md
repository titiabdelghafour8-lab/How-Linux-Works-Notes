# The big  picture

## I - Introduction
while the internals of the linux operating system, or operating systems overall appear to be so complexe, users interact with such powerful systems through layers that simplify this interaction, called : abstraction, based on one's needs a user can go as deep as needed when interacting with components of an operating system without needing to know the intricacies and under the hood of other tools making it a lot more manageable.

# II - Layers of abstraction in a linux system  

```mermaid     
block-beta
  columns 1
  %% Layer 1: User Processes
  block:Layer1:1
    space title1(("User Processes")) space
    columns 3
    GUI["Graphical User Interface"] Servers Shell
    
  end
  %% Layer 2: Linux Kernel
  block:Layer2:1
    columns 3
    space title2(("Linux Kernel")) space
    SysCalls["System Calls"] ProcessMgmt["Process Management"] MemoryMgmt["Memory Management"]
    space
    DeviceDrivers["Device Drivers"] space space
  end
  %% Layer 3: Hardware
  block:Layer3:1
    columns 3
    space title3(("Hardware")) space
    CPU["Processor (CPU)"] RAM["Main Memory (RAM)"] Disks NetPorts["Network Ports"]
  end
```
*   Figure 1-1: General Linux system organization

