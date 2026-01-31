# 🖥️ Advanced CPU Scheduling Simulator

A comprehensive, production-grade CPU scheduling simulator with I/O operations, multi-level queues, and real-time performance analysis. Built with pure HTML/CSS/JavaScript - no frameworks needed!

[![Live Demo](https://img.shields.io/badge/Demo-Live-success)](https://Aayu2810.github.io/cpu-scheduler-simulator/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## ✨ Features

### 🎯 Core Capabilities
- **6+ Scheduling Algorithms**: FCFS, SJF, SRTF, Priority, Round Robin, MLFQ
- **I/O Operations**: Realistic process behavior with I/O bursts
- **Process States**: NEW → READY → RUNNING → WAITING → COMPLETED
- **Real-time Metrics**: Turnaround, Waiting, Response Time, Throughput
- **Visual Gantt Charts**: Color-coded timeline with hover details
- **Algorithm Comparison**: Side-by-side performance analysis

### 🔬 Advanced OS Concepts
- Context switching simulation
- Multi-level feedback queue implementation
- CPU utilization tracking
- State transition visualization
- I/O wait queue management
- Starvation prevention mechanisms

## 🚀 Live Demo

**[Try it here!](https://Aayu2810.github.io/cpu-scheduler-simulator/)**

## 📸 Screenshots

### Gantt Chart View
![Gantt Chart](Grantt Chart.png)

### Process State Timeline
![States](assets/states.png)

### Performance Comparison
![Comparison](assets/comparison.png)

## 🎓 Educational Use

Perfect for:
- Operating Systems courses
- Algorithm analysis
- Interview preparation
- Teaching demonstrations
- Research projects

## 💻 Usage

### Quick Start
1. Click "Generate Random (5)" for sample processes
2. Select an algorithm or "Compare All"
3. Click "Run Simulation"
4. Explore different tabs for insights

### Custom Processes
1. Enter process details (name, arrival, burst, priority)
2. Optionally add I/O operations
3. Click "Add Process"
4. Configure algorithm settings
5. Run simulation

### Features Breakdown

#### Process Configuration
- Custom names (e.g., "Chrome", "Compiler")
- Arrival time (ms)
- CPU burst time (ms)
- Priority levels (1-10)
- Optional I/O operations

#### Algorithms Explained

**FCFS (First Come First Serve)**
- Simplest algorithm
- No preemption
- High average waiting time
- Good for batch systems

**SJF (Shortest Job First)**
- Optimal for average waiting time
- Requires burst time knowledge
- Can cause starvation
- Non-preemptive

**SRTF (Shortest Remaining Time First)**
- Preemptive version of SJF
- Minimum average waiting time
- High context switching overhead
- Good for time-sharing

**Priority Scheduling**
- Each process has priority
- Can be preemptive/non-preemptive
- Risk of starvation (solved by aging)
- Used in real-time systems

**Round Robin**
- Time quantum based
- Fair CPU allocation
- Good response time
- Higher context switching

**MLFQ (Multi-Level Feedback Queue)**
- Multiple ready queues
- Dynamic priority adjustment
- Prevents starvation
- Used in modern OS (Unix, Windows)

## 📊 Performance Metrics

### Calculated Metrics
- **Turnaround Time**: Completion - Arrival
- **Waiting Time**: Turnaround - Burst
- **Response Time**: First Run - Arrival
- **CPU Utilization**: (Busy Time / Total Time) × 100
- **Throughput**: Processes / Second

## 🛠️ Technical Details

### Technologies
- HTML5
- CSS3 (Grid, Flexbox, Animations)
- Vanilla JavaScript (ES6+)
- No external dependencies!

### Architecture
```
├── Process Management
│   ├── Process Creation
│   ├── State Management
│   └── Queue Operations
├── Scheduling Engine
│   ├── Algorithm Implementations
│   ├── Context Switching
│   └── I/O Handling
├── Visualization Layer
│   ├── Gantt Chart Renderer
│   ├── State Timeline
│   └── Metrics Dashboard
└── Analytics
    ├── Performance Calculator
    ├── Comparison Engine
    └── Recommendations
```

### Key Algorithms

**Time Complexity:**
- FCFS: O(n log n) - sorting
- SJF: O(n²) - selection in worst case
- SRTF: O(n²) - preemptive checks
- Priority: O(n log n) - heap-based
- RR: O(n) - queue operations
- MLFQ: O(n) - multi-queue

## 🎨 Customization

### Color Scheme
Edit CSS variables in `:root`:
```css
--primary: #667eea;
--success: #51cf66;
--danger: #ff6b6b;
```

### Add New Algorithm
```javascript
function myScheduler(queue, time) {
    // Your logic here
    return selectedProcess;
}
```

## 📚 Learning Resources

- [OS Scheduling Concepts](https://www.geeksforgeeks.org/cpu-scheduling-in-operating-systems/)
- [MLFQ Explained](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-sched-mlfq.pdf)
- [Scheduling Algorithms Comparison](https://www.javatpoint.com/os-scheduling-algorithms)

## 🤝 Contributing

Contributions welcome! Ideas:
- [ ] Add more algorithms (EDF, LJF, etc.)
- [ ] Export results to PDF/CSV
- [ ] Animation of process execution
- [ ] Multi-core CPU simulation
- [ ] Memory management integration
- [ ] Deadlock detection

## 📄 License

MIT License - feel free to use for education and research!

## 🙏 Acknowledgments

- Inspired by OS textbooks (Silberschatz, Tanenbaum)
- Built for students learning operating systems
- Designed for practical understanding of scheduling

## 📧 Contact

Questions or suggestions? Open an issue!

---

⭐ **Star this repo if it helped you understand CPU scheduling!**
