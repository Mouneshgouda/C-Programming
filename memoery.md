# IoT Sensor Aggregation

## Problem Statement

An IoT monitoring gateway receives a stream of readings from various sensors deployed across a facility.  
Each reading contains:

- a sensor **id**
- a sensor **type** (TEMP, HUMID, MOTION, STATUS)
- a **value** interpreted based on the type

To save memory, sensor values are stored using a **union**, since different types share the same memory region.

Your task is to:

1. Read **N sensor records**, storing them in an array of structures.  
   Each structure must contain:
   - an **enum** indicating the sensor type
   - a **union** holding the sensor value

2. Compute and print aggregate statistics as specified below.

---

## Requirements

### Aggregates to Compute


2. **Average temperature**  
- Print with **two decimal places**  
- If no temperature records, print `None`

3. **Maximum humidity**  
- If no humidity records, print `None`

4. **Motion event count**  
Count how many MOTION readings have value **1**

5. **Status character counts**  
- STATUS readings contain a single uppercase character (`A`–`Z`)  
- Print results in **ascending character order**, one per line:  
  ```
  <CHAR> <count>
  ```
- If no status readings, print `None`

---

## Input Format

- First line: integer **N** (0 ≤ N ≤ 100000)
- Next **N** lines formatted as:


### Valid Types and Value Formats

| Type    | Value Format        | Example | Notes |
|---------|----------------------|---------|-------|
| TEMP    | floating-point        | 23.7    | temperature in °C |
| HUMID   | integer (0–100)       | 85      | humidity % |
| MOTION  | integer (0 or 1)      | 1       | 1 = motion detected |
| STATUS  | single uppercase char | A       | status code |

---

## Output Format

Print the results in the following order:

1. Sensor type counts  
2. Average temperature (`xx.xx` or `None`)  
3. Maximum humidity (`value` or `None`)  
4. Motion event count  
5. Status character counts (or `None`)

---

## Sample Test Case 1

### Input

```
7
101 TEMP 23.5
12 HUMID 85
7 MOTION 1
5 STATUS A
102 TEMP 24.5
9 MOTION 0
6 STATUS A

```

## output
```
### Output
2 1 2 2
24.00
85
1
A 2
```
```
---

## Sample Test Case 2

### Input
3
1 MOTION 1
2 MOTION 0
3 MOTION 1

shell
Copy code

### Output
0 0 3 0
None
None
2
None
```
1. **Number of records per sensor type**  
   Output as:  
