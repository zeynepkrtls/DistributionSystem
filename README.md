# Distribution System Simulation in AnyLogic

A discrete-event simulation project developed using **AnyLogic** to model a real-world **distribution system** between a **Production Center** and a **Retail Store**. This simulation analyzes how inventory, customer demand, and delivery delays interact within a supply chain.

## 🎯 Project Overview

As global production and consumption patterns evolve, the efficiency of distribution systems becomes critical. This simulation project aims to:

- Model a retail store interacting with a production center
- Handle customer arrivals and purchasing behavior
- Manage dynamic inventory levels
- Trigger restocking based on threshold logic
- Track and fulfill backorders
- Visualize system performance using real-time graphs

## 🛠️ Tools & Technologies

- [AnyLogic](https://www.anylogic.com/) (Simulation software)
- Java (internal scripting used within AnyLogic blocks)

## 🧩 System Components

### Agents

- **RetailOutlet**: Represents the retail store, handles customer arrivals, manages inventory, and places orders.
- **ProductionCenter**: Produces and delivers stock to the retail outlet.

### Key Parameters

- `initialInventory`: Starting stock level at the retail store (150 units)
- `minInventoryLevel`: Threshold for reordering (75 units)
- `orderSize`: Amount ordered per request (150 units)
- `dayOfWeek`, `isWeekend`: Control customer arrival rates (2/hour weekdays, 4/hour weekends)

### Variables

- `retailInventory`: Tracks current inventory
- `backOrderCount`: Monitors unfulfilled customer requests
- `orderPlaced`: Indicates whether an order has been made

### Blocks Used

- `Source`, `Queue`, `Service`, `Delay`, `Sink`, `TimeMeasureStart/End`
- Custom logic blocks to control order placement and backorder handling

## 📈 Key Features

- Dynamic visualization of:
  - Inventory levels
  - Backorder quantities
- Realistic delays using triangular distribution (min: 2.5 days, mode: 3, max: 4)
- Conditional logic for stock replenishment and customer demand simulation
- Scenarios tested with varying customer arrival rates (weekday vs weekend)
  
## 📈 Simulation Output

- 📊 Inventory level is maintained without depletion.
- 🔄 Backorders are tracked and fulfilled when inventory is restocked.
- 📉 Realistic delay modeling reflects real-world delivery cycles.
- 👥 System tested with different customer intensities (weekday vs weekend).

## 📌 How to Run

1. Open the `.alp` file in AnyLogic.
2. Click **Run** to start the simulation.
3. Use the bar and time graphs to observe inventory and backorder changes over time.


