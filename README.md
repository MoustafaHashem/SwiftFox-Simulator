# CPU Scheduler Simulator

**CPU Scheduler Simulator** is a Java-based desktop application built with JavaFX to simulate and visualize various CPU scheduling algorithms in real time. The application offers dynamic process management, live visualization, and detailed statistical analysis—ideal for academic and educational purposes.

### Home Screen
![Home Screen](cpu_scheduler/src/main/resources/com/swiftfox/images/welcomingScene.png "Home Screen")

### Processing Screen
![Processing Screen](cpu_scheduler/src/main/resources/com/swiftfox/images/MainScene.png "Processing Screen")

---

## Table of Contents 📑

1. [Supported Scheduling Algorithms](#supported-scheduling-algorithms)
2. [Key Features](#key-features)
3. [Input Parameters by Scheduler](#input-parameters-by-scheduler)
4. [Documentation 📚](#documentation-)
5. [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Running the Application](#running-the-application)
        - [Option 1: Using the Executable EXE](#option-1-using-the-executable-exe)
        - [Option 2: Using the Executable JAR](#option-2-using-the-executable-jar)
        - [Option 3: From Source (Maven)](#option-3-from-source-maven)

---

## Supported Scheduling Algorithms

1. First-Come, First-Served (FCFS)
2. Shortest Job First (SJF)
   - Preemptive
   - Non-Preemptive
3. Priority Scheduling
   - Preemptive
   - Non-Preemptive
4. Round Robin (RR)

> The application only requests inputs relevant to the selected algorithm (e.g., priority values are not required for FCFS).

---

## Key Features

- Real-time simulation: 1 second = 1 time unit
- Live Gantt Chart rendering and process timeline visualization
- Dynamically add processes while the scheduler is running
- Real-time table of remaining burst times
- Calculation of:
  - Average Waiting Time
  - Average Turnaround Time
- Option to simulate only predefined processes (static scheduling mode)
- Built as a JavaFX desktop application

---

## Input Parameters by Scheduler

| Scheduler      | Required Inputs                          |
|----------------|-------------------------------------------|
| FCFS           | Arrival Time, Burst Time                  |
| SJF            | Arrival Time, Burst Time                  |
| Priority       | Arrival Time, Burst Time, Priority        |
| Round Robin    | Arrival Time, Burst Time, Time Quantum    |

---

## Documentation 📚

For detailed documentation on how the project works and how to contribute, please visit the [Documentation](https://moustafahashem.github.io/SwiftFox-Simulator/).
---
## Getting Started

### Prerequisites

- Java JDK 11 or higher
- JavaFX SDK (if not bundled with JDK)
- Maven (used for building and running the project)

### Running the Application

### Option 1: Using the Executable EXE

#### Download the ZIP archive containing the Windows executable from [here](https://github.com/MoustafaHashem/SwiftFox-Simulator/releases/download/ReadyToPublish/SwiftFox.zip), then:

#### 1. Extract the ZIP file.

#### 2. Double-click the `SwiftFox-Simulator.exe` file.

#### 3. The application will launch immediately with no additional setup.

### Option 2: Using the Executable JAR

#### 1. Download the compiled .jar file from the dist/ directory.

#### 2. Run the application using:
   ```bush
   java -jar SwiftFox-Simulator.jar
   ```
### Option 3: From Source (Maven)

#### 1. Clone the repository
```bash
git clone https://github.com/MoustafaHashem/SwiftFox-Simulator.git
cd SwiftFox-Simulator
```

#### 2. Build and run using Maven:
```bash
mvn clean javafx:run
```
Note: Ensure your `pom.xml` is configured to use the JavaFX Maven Plugin and includes the necessary JavaFX modules (`javafx.controls`, `javafx.fxml`, etc.).
