
# 📡 FTTH Network Design using AI Clustering (K-Means)

Designing smart fiber optic internet layouts for multiple homes — using Python, AI clustering, and signal loss + cost optimization.

---

## 🎯 Project Objective

This project simulates how telecom engineers plan a Fiber-to-the-Home (FTTH) network. Given the location of homes (latitude, longitude), the system:

- Groups homes into clusters (using K-Means)
- Places Fiber Distribution Hubs (FDHs) efficiently
- Calculates fiber distances from each home to its FDH
- Estimates signal loss (dB) based on cable length and splitter loss
- Calculates total project cost (fiber, splitters, FDHs)
- Generates Excel reports and layout maps automatically

✅ Everything is automated with Python and fully reproducible!

---

## 🛠️ Tools & Technologies Used

| Technology   | Purpose                             |
|--------------|-------------------------------------|
| Python       | Main programming language            |
| pandas       | Data handling and processing         |
| scikit-learn | K-Means clustering                   |
| geopy        | Calculating geographic distances     |
| matplotlib   | Drawing layout maps                  |
| xlsxwriter   | Excel report generation              |

---

## 📂 Folder Structure

```
FTTH-Network-Design/
│
├── main.py                      ← Main script to run everything
├── requirements.txt             ← Python libraries
├── README.md                    ← This file
│
├── data/
│   └── homes_coordinates.csv    ← Input: Home locations
│
├── src/
│   ├── network_optimizer.py     ← Clustering, distance, signal loss
│   ├── cost_estimator.py        ← Fiber + splitter + FDH cost
│   └── plot_layout.py           ← Draws cluster map
│
└── output/
    ├── layout_map.png           ← Output map
    ├── cost_report.xlsx         ← Total cost sheet
    └── loss_distance_report.xlsx ← Signal loss + distance per home
```

---

## 📈 Sample Outputs

- 🗺️ layout_map.png — Cluster map showing homes and FDHs
- 📊 cost_report.xlsx — Total cost (fiber, FDHs, splitters)
- 📄 loss_distance_report.xlsx — Each home's fiber length and signal loss

---

## ▶️ How to Run

1. Clone this repository:
```bash
git clone https://github.com/YOUR_USERNAME/FTTH-Network-Design.git
cd FTTH-Network-Design
```

2. Install the required libraries:
```bash
pip install -r requirements.txt
```

3. Run the project:
```bash
python main.py
```

4. View the output files in the output/ folder

---

## 📐 Signal Loss Formula

Each home’s signal loss is calculated using:

```
Loss (dB) = (0.35 × fiber_length_km) + splitter_loss_dB
```

- 0.35 dB/km is standard optical attenuation
- Splitter loss typically 3.5 dB (for 1:8 splitters)

---

## 💰 Cost Estimation

| Component       | Estimated Cost     |
|----------------|--------------------|
| Fiber/km        | ₹15,000            |
| Splitter (1:8)  | ₹1,000 each        |
| FDH             | ₹5,000 each        |

All cost logic is in cost_estimator.py — you can adjust values.

---

## 📌 Real Use Case

This system simulates a real-world telecom network planning scenario, like what Jio, Airtel, or ACT Fiber do before laying fiber in residential areas.

- Save cost with optimal placement
- Predict signal loss to ensure quality
- Plan for clusters with 8 or 16 homes per FDH
- Use Excel + Maps for engineering documentation

---

## 👨‍💻 Author

👤 Jagadeesh Kasetti  
🎓 B.Tech Final Year – Electrical and Electronics Engineering  
🔗 GitHub: https://github.com/Jagadeesh62  
🔗 LinkedIn: [Your LinkedIn Profile]

---

## 🏷️ Tags

#ftth #telecom #ai #python #iot #finalyearproject #networkdesign #clustering #fiberoptic #opensource #kmeans #telecomengineering

