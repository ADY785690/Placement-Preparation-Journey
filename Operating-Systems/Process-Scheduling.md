# Process Scheduling

## What is Process Scheduling?

Process Scheduling is the method used by the Operating System to decide which process gets CPU execution time.

Goal:
- Maximum CPU Utilization
- Minimum Waiting Time
- Maximum Throughput

---

## Important Terms

### Arrival Time (AT)

Time at which process enters ready queue.

### Burst Time (BT)

CPU time required by process.

### Completion Time (CT)

Time when process finishes execution.

### Turnaround Time (TAT)

Formula:

TAT = CT - AT

---

### Waiting Time (WT)

Formula:

WT = TAT - BT

---

### Response Time (RT)

Time between process arrival and first CPU allocation.

---

# FCFS (First Come First Serve)

Processes execute in arrival order.

Example:

P1 → P2 → P3

Advantages:
- Simple
- Easy implementation

Disadvantages:
- Convoy Effect
- High waiting time

Type:
Non-Preemptive

---

# SJF (Shortest Job First)

Process with smallest burst time executes first.

Example:

BT:
P1 = 6
P2 = 2
P3 = 4

Order:

P2 → P3 → P1

Advantages:
- Minimum average waiting time

Disadvantages:
- Starvation possible

Type:
Non-Preemptive

---

# SRTF (Shortest Remaining Time First)

Preemptive version of SJF.

CPU can switch if shorter process arrives.

Type:
Preemptive

---

# Priority Scheduling

Highest priority process executes first.

Example:

Priority:
P1 = 1
P2 = 3
P3 = 2

Execution:

P1 → P3 → P2

Advantages:
- Important tasks execute first

Disadvantages:
- Starvation

---

# Round Robin

Each process gets fixed Time Quantum.

Example:

Time Quantum = 2 ms

P1 → P2 → P3 → P1 → P2

Advantages:
- Fair scheduling
- Good response time

Disadvantages:
- Context Switching Overhead

Type:
Preemptive

---

# Scheduling Comparison

| Algorithm | Preemptive | Starvation |
|------------|------------|------------|
| FCFS | No | No |
| SJF | No | Yes |
| SRTF | Yes | Yes |
| Priority | Yes/No | Yes |
| Round Robin | Yes | No |

---

# Common GATE & Placement Questions

Q1. Formula for Turnaround Time?

TAT = CT - AT

Q2. Formula for Waiting Time?

WT = TAT - BT

Q3. Which scheduling gives minimum waiting time?

Answer:
SJF

Q4. Which scheduling is best for Time Sharing Systems?

Answer:
Round Robin

Q5. Which algorithm suffers from Convoy Effect?

Answer:
FCFS

---

# Revision Notes

FCFS → Arrival Order

SJF → Smallest Burst Time

SRTF → Preemptive SJF

Priority → Highest Priority First

Round Robin → Uses Time Quantum
