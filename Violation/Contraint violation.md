### Task 3: Constraint Violations

**C1: TP → ¬BO**  
Violation scenario: TP = TRUE, BO = TRUE  
The barrier stays open while a train is on the crossing. Since TP is TRUE, BO should be FALSE. Therefore, TRUE → FALSE is false, so C1 is violated.

**C2: TA → WN**  
Violation scenario: TA = TRUE, WN = FALSE  
A train is approaching, but the warning lights and alarm are off. Since TA is TRUE and WN is FALSE, the implication fails, so C2 is violated.

**C3: TP → BC**  
Violation scenario: TP = TRUE, BC = FALSE  
A train is present in the crossing, but the barrier is not closed. Since TP is TRUE, BC should be TRUE. Therefore, C3 is violated.

**C4: OC → (TC ∧ ¬TP)**  
Violation scenario: OC = TRUE, TC = FALSE, TP = TRUE  
The system sends an open command while the train has not cleared the crossing and is still present. The condition (TC ∧ ¬TP) is FALSE, so C4 is violated.

**C5: BC → WN**  
Violation scenario: BC = TRUE, WN = FALSE  
The barrier is closed, but the warning lights and alarm are off. Since BC is TRUE, WN should also be TRUE. Therefore, C5 is violated.

**C6: (TA ∨ TP) → RR**  
Violation scenario: TA = TRUE, TP = FALSE, RR = FALSE  
A train is approaching, but the road signal is not red. Since TA ∨ TP is TRUE while RR is FALSE, the implication fails, so C6 is violated.

**C7: SF → (BC ∧ WN)**  
Violation scenario: SF = TRUE, BC = FALSE, WN = TRUE  
A sensor failure occurs, but the barrier remains open. The rule requires both BC and WN to be TRUE. Since BC ∧ WN is FALSE, C7 is violated.

**C8: CL → (BC ∧ WN)**  
Violation scenario: CL = TRUE, BC = TRUE, WN = FALSE  
Communication with the control center is lost. Although the barrier closes, the warning system is off. Since BC ∧ WN is FALSE, C8 is violated.

**C9: BF → (CA ∧ ¬TG)**  
Violation scenario: BF = TRUE, CA = FALSE, TG = TRUE  
The barrier has failed, but the control center is not alerted and the train signal is green. Since CA is FALSE and TG is TRUE, the required condition is false. Therefore, C9 is violated.

**C10: TG → BC**  
Violation scenario: TG = TRUE, BC = FALSE  
The train signal is green while the barrier is open. Since TG is TRUE, the barrier should be closed. Therefore, TRUE → FALSE is false, so C10 is violated.
