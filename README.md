## Contents
- `Performance_Modeling_Public_Transportation_Network.pdf` — Main report (upload here)
- `colombo_bus_dataset.xlsx` — Simulated operational dataset
- `simulation/` — (Optional) Python code for SimPy model
- `figures/` — (Optional) Graphs and charts

## Dataset Schema (`colombo_bus_dataset.xlsx`)
| Field | Description |
|------|-------------|
| bus_id | Unique identifier for each simulated bus (per route) |
| route_no | Route number (103, 144, 171) |
| stop_name | Stop name in route order |
| arrival_time | Timestamp when bus arrives at stop |
| departure_time | Timestamp when bus departs stop |
| boarded | Passengers boarding at the stop |
| alighted | Passengers alighting at the stop |
| occupancy_after | Onboard count after departure |
| dwell_time_s | Stop dwell time (seconds) |
| headway_s | Time since previous bus at the same stop & route (seconds) |
| is_timepoint | TRUE if stop is a timepoint (checkpoint) |
| is_peak | TRUE during peak windows (07:00–09:00, 16:30–19:00) |

## Objectives
- Minimize passenger waiting time
- Maximize fleet utilization
- Reduce headway variance
- Identify bottlenecks (stops/routes causing delays)
- Evaluate scalability under increased demand

## How to Use
1. Upload the PDF report and this dataset to your GitHub repository.
2. (Optional) Implement a SimPy simulation that ingests this dataset to validate and extend the analysis.
3. Create visualizations (e.g., headway distributions, occupancy heatmaps) to support findings.
