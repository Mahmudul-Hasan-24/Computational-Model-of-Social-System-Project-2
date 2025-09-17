
## "Sharp transition towards shared vocabularies in multi-agent systems"
## 📌 Project Overview
This project implements an **agent-based model** to study opinion spreading and consensus formation on different network structures.  
The aim is to explore how **network topology** and **interaction rules** affect the **time to consensus** and overall opinion dynamics.

---

## 🗂 Repository Structure
```
├── notebooks/
│   └── OpinionDynamics.ipynb   # Main notebook implementing the model
├── docs/
│   └── consensus_plot.png      # Example visualization
└── requirements.txt            # Python dependencies
```

---

## 🧠 Model Description

### Agents
- Each agent represents an individual with a **binary opinion** (0 or 1).

### Network Topologies
- **Erdős–Rényi (Random network)**
- **Watts–Strogatz (Small-world network)**
- **Barabási–Albert (Scale-free network)**

### Interaction Rule
At each time step:
1. Select a random agent.
2. Select one of its neighbors at random.
3. The agent adopts the neighbor's opinion.

This process repeats until consensus is reached (all agents share the same opinion).

---

## 📊 Key Results
| Network Type       | Finding |
|-------------------|--------|
| Random Network    | Reaches consensus quickly but with high variability. |
| Small-World       | Moderate consensus time; clustering slows convergence slightly. |
| Scale-Free        | Slowest consensus due to influence bottlenecks at hubs. |

---



## 🛠 How to Run Locally

### 1. Clone this repository
```bash
git clone https://github.com/Mahmudul-Hasan-24/Computational-Model-of-Social-System-Project-2.git
cd Computational-Model-of-Social-System-Project-2
```

### 2. Create and activate a virtual environment
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook
```bash
jupyter notebook notebooks/OpinionDynamics.ipynb
```

---

## 📦 Dependencies
- networkx – Network generation & analysis  
- numpy – Numerical operations  
- matplotlib – Visualization  
- jupyter – Notebook interface  

---

## 🚀 Possible Extensions
- Introduce **stubborn agents** (zealots) and measure their effect on consensus time.
- Simulate **multi-opinion models** (e.g., more than two opinions).
- Measure **polarization metrics** instead of only consensus time.

---

## 📜 License
This project is licensed under the MIT License – see [LICENSE](LICENSE) for details.

---

## 👤 Author
**Mahmudul Hasan**  
Master’s of Computational Social System (Business Analytics) at Technical University of Graz & University of Graz 
