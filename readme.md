# Docker image to run the automatic grader for Java Assesment 01

## Requirements

- Docker (tested with 19.03.5 on linux)
- docker-compose (tested with 1.25.4 on linux)
- Port 8888 is available on the machine (for JupyterLab)

## Usage

1. Put the workspaces under the directory workspaces
2. Make sure that there are three directories namely workspaces, work, and results in the directory that contains the readme.md
3. Run the docker by `docker-compose up` and finds a URL looks like http://127.0.0.1:8888/?token=...
...
4. Find main.ipynb in the file browser in the left sidebar and open it
4. (Optional) Disable autosave via "Settings"  in the menu bar
5. Run all cells
6. Open results/result.csv

## Shut down

Click "Shut Down" in the "File" menu.

## Structure of the workspaces
```
workspaces
├── Trainee01
│   └── src
│       ├── form
│       │   └── BusinessTrip.java
│       ├── main
│       │   └── Application.java
│       └── utility
│           └── StandardInputReader.java
├── Trainee02
│   └── src
│       ├── form
│       │   └── BusinessTrip.java
│       ├── main
│       │   └── Application.java
│       ├── module-info.java
│       └── utility
│           └── StandardInputReader.java
├── Trainee03
│   └── src
│       ├── form
│       │   └── BusinessTrip.java
│       ├── main
│       │   └── Application.java
│       └── utility
│           └── StandardInputReader.java
...
```