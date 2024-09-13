# Efficient Data Stream Anomaly Detection
![alt text](Result1.png)
![alt text](Result2.png)
![alt text](Result3.png)


## Project Overview
This project demonstrates an anomaly detection system that simulates continuous data streams, detects anomalies in real time, and visualizes the results. The data stream can represent metrics such as financial transactions or system measurements, and the system uses the ADWIN algorithm for detecting concept drift and Z-score analysis for anomaly detection.

## Key Features:
- **Simulated Data Stream**: Data includes regular patterns, seasonal fluctuations, and occasional anomalies.
- **Anomaly Detection**: Combines ADWIN for detecting concept drift and Z-score for identifying anomalies.
- **Real-Time Visualization**: Continuously plots the data stream and marks detected anomalies in real-time.

## Project Structure
- **`simulate_data.py`**: Simulates real-time sensor data with regular patterns, seasonal variations, and random noise. It occasionally introduces anomalies and sends the data to the server.
- **`server.py`**: Processes the incoming data using the ADWIN algorithm to detect concept drift and Z-score anomaly detection. It sends appropriate feedback to the client.
- **`visualize.py`**: Plots the real-time data stream, highlighting anomalies with red dots.

## Installation

### Prerequisites
- Python 3.x
- Required packages can be installed using pip.

### Steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/Akshyansu3479/Efficient_Data_Stream_Anomaly_Detection.git
    ```

2. Navigate to the project directory:

    ```bash
    cd Efficient_Data_Stream_Anomaly_Detection
    ```

3. Create a virtual environment:
   This is optional.
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

4. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## How to Run

### Step 1: Start the Server
Run the server script to begin listening for simulated data.

```bash
cd server
python server.py
```

### Step 2: Start the Client (Simulating Data)
Open a new terminal window and run the client simulation to start sending data.

```bash
cd client
python simulate_data.py
```

### Step 3: Visualize Data
Run the visualization script to display the real-time data stream and detected anomalies(this should also be in a new terminal)

```bash
cd client
python visualize.py
```
### Step 4: Results
The real-time graph will show the data stream in blue.
Anomalies will be highlighted with red points in the graph.

