# MAJOR-PROJECT-
### Disaster Relief Routing System
Overview

The Disaster Relief Routing System is a solution designed to enhance the efficiency of resource distribution in disaster-stricken areas. The system models the affected regions as a graph where the nodes represent the areas and the edges represent the roads connecting them. The primary goal is to determine the most effective routes for delivering aid, considering factors like road conditions and area priorities.

---

### Key Features:

**Graph Representation**: Each area is modeled as a node, and the roads between them are represented as weighted edges in the graph.

**Priority Areas**: Specific areas, such as hospitals or emergency shelters, may require prioritization for relief, influencing the routing decisions.

**Efficient Pathfinding**: The system utilizes a pathfinding algorithm to calculate the shortest routes while factoring in road damage and area importance.

---

### System Workflow
**Graph Construction**: The disaster-stricken regions are represented as nodes within the graph. The roads between these regions are modeled as edges, each associated with a distance or weight.

**Prioritization of Areas**: Certain regions (e.g., hospitals, shelters) are given priority due to their critical nature. These areas are assigned reduced travel costs to ensure faster access.

**Shortest Path Algorithm**: The system uses an algorithm to determine the shortest route from a specified origin area to all other areas. It adjusts the route based on the importance of each area and the state of the roads.

---

### Input Parameters:
**Total Regions**: The number of areas (nodes) to be modeled.

**Roads/Connections**: The roads (edges) connecting the areas, each with an associated distance.

**Priority Areas**: Areas with special priority levels that affect their routing preferences.

**Start Area**: The initial region from which the program will calculate the shortest paths.

### Output:
The program outputs the shortest route from the start area to all other regions.
If any area is unreachable, the system will notify the user that it is inaccessible.

---

### Features
**Flexible Graph Setup**: Users can easily define areas and road connections interactively.

**Priority Management**: Users can assign priority levels to specific regions, influencing route calculations.

**Pathfinding**: An algorithm calculates and displays the shortest route from a starting region, adjusting for road damage and priority areas.

**Interactive User Inputs**: All necessary parameters, such as areas, connections, and priorities, are provided by the user at runtime.

---

### Getting Started

**Step-by-Step Guide:**
Clone the Repository: First, clone this repository to your local machine:

 ```bash
git clone https://github.com/yourusername/disaster-relief-routing-system.git
```
Compile the Code: Navigate to the project directory and compile the code with a C++ compiler:

```bash
g++ -std=c++11 -o ReliefRoutingSystem ReliefRoutingSystem.cpp
```
This will generate an executable named ReliefRoutingSystem (or ReliefRoutingSystem.exe for Windows).

Run the Program: After compiling, execute the program:

```bash
./ReliefRoutingSystem
```
The system will prompt you to input the number of areas, road connections, priority levels, and the origin area. Follow the instructions to proceed with the program.

---

### Sample Interaction
Here’s an example of how the program interacts with the user:
```
mathematica

Copy code
Enter the number of areas: 5
Enter the number of connections: 4
Enter connection 1 (start area, end area, length): 0 1 2
Enter connection 2 (start area, end area, length): 1 2 3
Enter connection 3 (start area, end area, length): 2 3 4
Enter connection 4 (start area, end area, length): 3 4 5
Enter the number of priority areas: 2
Enter area index and priority level for area 2: 2 1
Enter area index and priority level for area 4: 4 3
Enter the origin area for path calculation: 0
This will output the shortest path distances from the origin area:

mathematica

Copy code
Shortest distances from origin (Area 0):
Area 0 -> Distance: 0
Area 1 -> Distance: 2
Area 2 -> Distance: 5
Area 3 -> Distance: 9
Area 4 -> Distance: 14
```
