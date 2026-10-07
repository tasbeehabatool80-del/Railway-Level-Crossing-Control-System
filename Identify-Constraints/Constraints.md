## Automated Railway Level-Crossing Control System (ARLCCS)

| Constraint ID | Constraint in Simple English | Why the Constraint Is Necessary |
|---|---|---|
| **C1** | The barrier must not open while a train is present in the crossing. | Opening the barrier could allow road traffic to enter the crossing while the train is passing. |
| **C2** | The barrier must close when an approaching train is detected. | Closing the barrier prevents road traffic from entering the crossing before the train arrives. |
| **C3** | Warning lights must be activated when a train approaches the crossing. | Visual warnings alert drivers and pedestrians that a train is approaching. |
| **C4** | The audible alarm must be activated when a train approaches the crossing. | An audible warning provides an additional safety signal. |
| **C5** | The barrier must remain closed while the train is passing through the crossing. | Opening the barrier during train movement could expose road traffic to the train. |
| **C6** | The barrier may open only after the system confirms that the train has completely cleared the crossing. | The train may still be occupying the crossing even after part of it has passed. |
| **C7** | The system must not allow road traffic to pass through the crossing while a train is present. | Road traffic entering the crossing while a train is present creates a collision risk. |
| **C8** | A detected sensor failure must not result in the system treating the crossing as safe. | A failed sensor can produce incorrect information and cause unsafe operation. |
| **C9** | A barrier failure must not cause the system to indicate that the crossing is safe. | The system must not report a safe crossing when the physical barrier has failed. |
| **C10** | Communication loss with the control center must not cause the crossing to enter an unsafe state. | The crossing must remain safe even when communication is lost. |
| **C11** | Incorrect or conflicting sensor readings must not cause the system to open the barrier without valid clearance confirmation. | Conflicting information can create a false safe condition. |
| **C12** | Emergency conditions must cause the system to enter a safe state. | Emergency situations require priority safety handling. |
