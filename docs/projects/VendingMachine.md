# Hot Dog Vending Machine

**Software:** Relay Ladder Logic (RLL)  
**Role:** Sole Developer  
**Dates:** 2021  

**Problem.** Build an unattended vending machine that prepares a hot dog to order with basic customization, using a low-cost PLC while keeping the process safe and repeatable.

**Approach.**

- **Ladder-logic state machine** (Idle → Order → Prep/Heat → Dispense → Toppings → Eject → Fault/Recovery)
- **I/O map** for actuators (feed/valves) and sensors (limits/guards/temperature-ready)
- **Parameterized options** (portion times, topping enable bits) to avoid hard-coding
- **Safety interlocks**, timeout-based jam detection, and E-stop
- **Bench testing with simulated I/O** to validate sequencing and restart behavior

**Outcome.**

- Working prototype that reliably sequences prep → dispense → toppings based on user selections

