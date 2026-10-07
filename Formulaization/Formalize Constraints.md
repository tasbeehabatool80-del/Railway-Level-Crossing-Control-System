### Task 2: Formalize Constraints

**Symbols used**

| Symbol | Meaning |
| ------ | ------- |
| TA | Train_Approaching |
| TP | Train_Present (in crossing) |
| TC | Train_Cleared |
| BO | Barrier_Open |
| BC | Barrier_Closed |
| OC | Open_Command (system tries to open the barrier) |
| WN | Warning_On (lights and alarm) |
| RR | Road_Signal_Red |
| SF | Sensor_Failure |
| CL | Communication_Lost |
| BF | Barrier_Failure |
| CA | Control_Center_Alerted |
| TG | Train_Signal_Green |

| ID | Formal expression |
| --- | ----------------- |
| C1 | TP → ¬BO |
| C2 | TA → WN |
| C3 | TP → BC |
| C4 | OC → (TC ∧ ¬TP) |
| C5 | BC → WN |
| C6 | (TA ∨ TP) → RR |
| C7 | SF → (BC ∧ WN) |
| C8 | CL → (BC ∧ WN) |
| C9 | BF → (CA ∧ ¬TG) |
| C10 | TG → BC |
