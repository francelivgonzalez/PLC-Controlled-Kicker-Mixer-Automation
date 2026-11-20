# PLC-Controlled-Kicker-Mixer-Automation
> Translating industrial mixer protection and timed-cycle logic from PLC ladder logic into Python—built after a ~$100k production loss

A Python representation of an automated kicker mixer control and protection system originally developed in PLC ladder logic to replace manual oversight with timed cycles, temperature monitoring, fault shutdowns, and cooldown logic.

## What This Project Does

Before automation, kicker mixer operation relied heavily on manual operator monitoring—leaving the process vulnerable to delayed reactions, inconsistent runs, and costly equipment or batch loss. After a production failure tied to nearly **$100,000 in losses** and a **$30,000 prevention effort**, the control solution was implemented using roughly **$1,800** by repurposing existing and available hardware.

This project translates the core PLC control and protection logic into readable Python for documentation, simulation, and future expansion:
1. **Timed Mixer Cycles:** Automates mixer operation on defined time intervals rather than manual guesswork.
2. **Temperature & Fault Monitoring:** Continuously checks operating conditions and detects overheating or fault states.
3. **Protective Shutdown & Cooldown:** Triggers automated shutdown and cooldown sequences when unsafe conditions occur.

## What I'm Focusing On

- **Equipment & Batch Protection:** Preventing overheating and repeat failures on a high-consequence mixer process.
- **Cost-Effective Engineering:** Delivering reliable protection for **~$1,800** using repurposed components against a **$30,000** prevention allocation.
- **Reducing Manual Dependency:** Replacing inconsistent manual checks with repeatable timers, interlocks, and fault handling.
- **PLC-to-Python Portability:** Documenting ladder logic control sequences in a clean Python structure for review and simulation.

## How the Control Logic Is Set Up

- **Cycle & Timer Control:** Manages timed mixer run/dwell states and startup preconditions.
- **Condition & Thermal Checks:** Evaluates temperature and fault signals against safe operating limits.
- **Shutdown & Cooldown State Machine:** Transitions into safe stop and cooldown routines upon detecting faults or overheating.
- **Simulation & Scenario Testing:** Exercises normal timed runs, over-temperature trips, and fault/cooldown transitions in Python.

## Planned Folder Layout

```text
PLC-Controlled-Kicker-Mixer-Automation/
├── README.md
├── src/
│   ├── mixer_controller.py   # Timed cycle sequencing, interlocks, and shutdown/cooldown logic
│   ├── thermal_monitor.py    # Temperature threshold checks and fault detection
│   └── hardware_sim.py       # Simulated mixer, timer, and analog/sensor inputs
├── configs/
│   └── mixer_limits.yaml     # Cycle durations, temperature limits, and cooldown parameters
├── tests/
│   └── test_protection.py    # Normal cycle, overheat fault, and cooldown recovery tests
└── main.py                   # Entry point for running simulated mixer scenarios
