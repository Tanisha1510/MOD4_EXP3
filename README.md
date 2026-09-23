# AUTOMATED-TEST-CASES-FOR-16-DOOR-COMBINATIONS

## AIM: Develop and Execute Automated Test Cases for All 16 Combinations of Four Vehicle Door Statuses

---

## Apparatus Required

| S. No. | Apparatus / Software | Specification |
|:---:|---|---|
| 1 | PC / Laptop | For TSMaster configuration |
| 2 | Software | **TSMaster** |
| 3 | CAN Interface | **CAN Interface / CAN Simulator** |
| 4 | CAN Database | **DBC File** |
| 5 | Programming Environment | **TSMaster C Mini Program** |
| 6 | Test Environment | **TSMaster Test System / Test Module** |
| 7 | Input Signals | **Four Door-Status Signals** |
| 8 | Output Signal | **Interior-Light Signal** |

---

## Procedure

1. Open the **TSMaster** project containing the interior-light control program.
2. Identify the four door input signals:
   - **Front Left Door**
   - **Front Right Door**
   - **Rear Left Door**
   - **Rear Right Door**
3. Create a **Test Group** in the TSMaster test environment.
4. Create test cases covering all **16 possible combinations** of the four door inputs.
5. Assign the corresponding door-status inputs to each test case.
6. Define the expected result:
   - **All doors closed → Interior Light OFF**
   - **One or more doors open → Interior Light ON**
7. Configure automatic comparison between the **actual** and **expected** interior-light status.
8. Configure the test system to generate **PASS** when the actual and expected results match.
9. Configure the test system to generate **FAIL** when the actual and expected results do not match.
10. Execute the complete **Test Group**.
11. Record and verify the **PASS/FAIL verdicts** for all 16 test cases.

---

## Test Case Configuration

| Parameter | Configuration |
|---|---|
| Number of Door Inputs | **4** |
| Total Combinations | **16** |
| Test Type | **Automated** |
| Expected Output – All Doors Closed | **OFF** |
| Expected Output – Any Door Open | **ON** |
| Verdict | **PASS / FAIL** |
| Test Environment | **TSMaster Test System** |

---

## 16 Door Combinations

| Test Case | FL | FR | RL | RR | Expected Interior Light |
|:---:|:---:|:---:|:---:|:---:|:---:|
| TC01 | 0 | 0 | 0 | 0 | **OFF** |
| TC02 | 0 | 0 | 0 | 1 | **ON** |
| TC03 | 0 | 0 | 1 | 0 | **ON** |
| TC04 | 0 | 0 | 1 | 1 | **ON** |
| TC05 | 0 | 1 | 0 | 0 | **ON** |
| TC06 | 0 | 1 | 0 | 1 | **ON** |
| TC07 | 0 | 1 | 1 | 0 | **ON** |
| TC08 | 0 | 1 | 1 | 1 | **ON** |
| TC09 | 1 | 0 | 0 | 0 | **ON** |
| TC10 | 1 | 0 | 0 | 1 | **ON** |
| TC11 | 1 | 0 | 1 | 0 | **ON** |
| TC12 | 1 | 0 | 1 | 1 | **ON** |
| TC13 | 1 | 1 | 0 | 0 | **ON** |
| TC14 | 1 | 1 | 0 | 1 | **ON** |
| TC15 | 1 | 1 | 1 | 0 | **ON** |
| TC16 | 1 | 1 | 1 | 1 | **ON** |

**FL = Front Left, FR = Front Right, RL = Rear Left, RR = Rear Right**

---

## OUTPUT

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/9e3c3a88-12c8-42ad-bc43-8dfe4bd3f1ca" />

---

## Result

Automated test cases were successfully created and executed for all **16 possible combinations** of the four vehicle door statuses. The actual interior-light output was automatically compared with the expected result, and **PASS/FAIL verdicts** were generated for each test case.
