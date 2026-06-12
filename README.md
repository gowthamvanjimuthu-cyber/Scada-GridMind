# ⚡ Microgrid SCADA

A real-time **Microgrid Energy Management System (EMS)** and **SCADA Controller** featuring AI-driven dispatch optimization, digital twin simulation, and industrial protocol emulation.

🔗 **Live Demo (MVP)** 

https://gowthamvanjimuthu-cyber.github.io/Scada-GridMind/

---

## 🎯 Project Goal

To provide a full-stack, production-grade simulation of a microgrid SCADA system. This project demonstrates real-time energy management, renewable integration, battery storage optimization, and industrial automation protocols—all accessible through a modern, high-performance web dashboard.

---

## 🚀 Key Features

*   **🔄 Real-Time Simulation Engine:** Physics-based simulator with solar PV curves, wind turbine power models, battery electrochemistry, and load demand profiling (1s updates).
*   **🤖 AI-Powered EMS Dispatch:** Intelligent energy dispatch using a strict priority state machine (Renewables → Battery → Grid) with reinforcement learning optimization.
*   **📊 Live SCADA Dashboard:** Industrial-grade React dashboard with SVG dial gauges, odometer displays, real-time charts, and animated power flow visualization.
*   **🔋 Battery Management System (BMS):** Full SOC/SOH tracking, thermal management with fan control (Auto/Manual/Faulted), charge/discharge physics, and thermal runaway simulation.
*   **🌐 Industrial Protocol Emulation:** Modbus TCP registers, OPC UA nodes, IEC 61850 logical nodes, CAN Bus BMS frames, and MQTT telemetry publishing.
*   **🚨 Alarm Management:** Real-time alarm detection with severity levels (WARNING/CRITICAL), AI Fault Advisor for root cause analysis, and one-click self-repair.
*   **🔮 24-Hour Forecasting:** MLP neural network load forecaster, renewable generation predictor, and forward EMS dispatch simulation.
*   **🧪 Digital Twin Failure Simulation:** Inject faults (Fan Failure, Battery Thermal Runaway, Inverter Overcurrent Trip) and observe automated system responses.
*   **📂 Dataset Replay Mode:** Upload CSV datasets (Solar, Wind, Battery, Load, Grid, Inverter) to replay recorded field data.
*   **🌍 Carbon Analytics:** Track CO₂ savings, renewable utilization share, grid import/export kWh, and carbon offset metrics.
*   **💰 Tariff-Aware Optimization:** Peak/off-peak electricity tariff scheduling with cost-optimized dispatch and grid export revenue tracking.
*   **🔐 Role-Based Access Control:** Four user roles (Admin, Operator, Engineer, Viewer) with JWT-based authentication and permission-gated API endpoints.
*   **🌙 Theme Support:** Dark, Light, and custom theme modes for the dashboard interface.
*   **📈 Data Export:** Download full telemetry history and grid export records as CSV files.
*   **⚙️ Load Shedding:** Automatic 3-level load shedding during islanding or battery depletion scenarios.

---

## 🧠 AI & Machine Learning

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Reinforcement Learning** | Q-Learning | Optimizes battery charge/discharge scheduling to minimize cost and wear. |
| **Load Forecasting** | MLP Neural Network | Predicts 24-hour consumption patterns from historical telemetry data. |
| **Renewable Forecaster** | Physics-Informed Model | Predicts solar/wind generation based on time, cloud cover, and temperature. |
| **Anomaly Detection** | Statistical Analysis | Identifies unusual telemetry patterns and generates diagnostic alarms. |
| **Predictive Maintenance** | Health Scoring | Computes asset health scores for solar panels, turbines, and inverters. |

---

## 🛠️ Tech Stack

| Layer | Technology |
| :--- | :--- |
| **Backend** | Python 3, FastAPI, Uvicorn |
| **Frontend** | React 19, Vite, Tailwind CSS |
| **Charts/UI** | Recharts, Framer Motion, Lucide Icons |
| **Database** | SQLite (via SQLAlchemy) |
| **ML/AI** | Scikit-Learn (MLP, Random Forest), NumPy |
| **Protocols** | Modbus TCP, OPC UA, IEC 61850, CAN Bus, MQTT |
| **Real-Time** | WebSockets, REST API |

---

## 📱 Application Flow

1.  **Login:** Authenticate as Admin, Operator, Engineer, or Viewer.
2.  **Dashboard:** View real-time telemetry (Solar, Wind, Battery, Grid, Load) with live gauges and charts.
3.  **EMS Control:** Switch simulation modes, toggle component isolation, and adjust overrides.
4.  **Alarm Monitor:** View/Manage active alarms and use AI Fault Advisor for diagnosis.
5.  **Forecasting:** Analyze 24-hour ahead predictions for power generation and consumption.
6.  **Protocols:** Inspect live industrial protocol registers and frames.
7.  **Digital Twin:** Simulate hardware faults to test system resilience.
8.  **Reports:** Export telemetry and metrics for offline analysis.

---

## 🔧 Setup Instructions

### Prerequisites
*   Python 3.10+
*   Node.js 18+

### Backend Setup
```bash
cd backend
pip install -r requirements.txt
python main.py
```
*The API server starts at `http://localhost:8000`*

### Frontend Setup
```bash
cd frontend
npm install
npm run dev
```
*The dashboard opens at `http://localhost:5173`*

### Running Tests
```bash
cd backend
python test_backend.py
```

---

## 🔑 Default Credentials

| Role | Username | Password |
| :--- | :--- | :--- |
| **Admin** | admin | admin |
| **Operator** | operator | operator |
| **Engineer** | engineer | engineer |
| **Viewer** | viewer | viewer |

---

## 👨‍💻 Author

**Gowtham K**

---

> [!NOTE]
> This is an educational prototype demonstrating the integration of industrial SCADA systems, energy management algorithms, and AI/ML pipelines with a modern real-time web interface.
