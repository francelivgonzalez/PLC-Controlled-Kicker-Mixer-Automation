# PLC-Controlled-Kicker-Mixer-Automation
This project recreates in Python a PLC-based automation and protection system for an industrial mixer after a production issue caused nearly $100,000 in losses. The control logic automated mixer operation through timed cycles, temperature monitoring, and fault-based shutdown/cooldown behavior.


# Kicker Mixer Automation and Protection System

## Overview

This project focused on improving a mixer process that had **not previously been automated** and relied heavily on manual monitoring. After a production issue caused nearly **$100,000 in losses**, the system was backed by **$30,000** to help prevent the failure from happening again. By repurposing existing parts and available hardware, I was able to implement the solution using only **about $1,800**.

The project involved transferring industrial control logic from **PLC ladder logic to Python** while developing an automation and protection system for the mixer. The final solution automated timed mixer operation, monitored temperature conditions, and triggered shutdown or cooldown behavior when unsafe conditions were detected. The goal was to reduce operator dependency, improve consistency, protect equipment, and create a more scalable control system.


## Problem

Before this project, the mixer process depended largely on manual oversight. That meant operators had to actively monitor the system and respond to issues themselves, which increased the risk of delayed reactions, inconsistent operation, and equipment or product loss. After a major failure led to nearly $100,000 in losses, there was a clear need for a more dependable and automated control approach.


## Solution

To address the issue, I developed a control system that automated key parts of the mixer process and added built-in protection logic. The system was first designed in **PLC ladder logic** and later transferred into **Python** to support documentation, logic portability, and future system integration.

The solution included:
- Timed mixer operation
- Temperature monitoring
- Fault detection
- Automated shutdown behavior
- Cooldown response logic
- A structure that supports future sensor-based expansion

This turned a previously manual process into a more reliable and scalable system.


## Key Features

- **Automated timed cycles** for mixer operation
- **Temperature-based protection** to detect overheating conditions
- **Fault-responsive shutdown and cooldown logic**
- **Repurposed hardware approach** to reduce implementation cost
- **Logic transfer from ladder logic to Python** for scalability and documentation
- **Foundation for future analog sensor integration** such as contamination or process-quality monitoring


## Impact

- Addressed a process tied to nearly **$100,000 in losses**
- Supported by a **$30,000 prevention effort**
- Implemented using only **~$1,800** through repurposed parts
- Reduced reliance on manual intervention
- Improved process reliability and protection
- Created a more cost-conscious automation solution without requiring a full rebuild


## Technologies Used

- **PLC ladder logic**
- **Python**
- Industrial controls and automation concepts
- Temperature monitoring logic
- Timers, interlocks, and fault handling
- Repurposed control hardware and components
- Analog 


## System Logic Summary

The control logic was designed to:
1. Start and manage mixer operation through timed cycles
2. Continuously monitor operating conditions
3. Detect overheating or fault conditions
4. Trigger protective shutdown or cooldown behavior when needed
5. Improve repeatability and reduce the chance of operator error


## Why This Project Matters
This project came from a real production need, not just a classroom exercise. It reflects how automation can directly improve reliability, lower risk, and reduce losses in an industrial environment. It also shows how thoughtful engineering and repurposing existing hardware can create a strong solution without using the full allocated budget.

## Future Improvements
- Expand analog sensor integration for contamination detection and process-quality monitoring
- Add fault logging and event history
- Integrate HMI or dashboard monitoring
- Add data tracking for maintenance and process analysis
- Further refine Python-based logic simulation and validation
