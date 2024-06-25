# Multi-period Location Routing Instances
This repository contains the instances used in the numerical experiments perfomed in the master thesis titled "An ALNS-based Matheuristic Algorithm for an Offshore Multi-period Location Routing Problem". The instances are designed to model the offshore multi-period location routing problem and evaluate the proposed solution approach.

# Instance Format

This section explains the format and contents of the instances file used in the thesis, which includes information about nodes (turbines and substations) and various operational parameters.

## Node Data

The node data is presented in a tabular format with each row representing a different node. The columns are as follows:

1. **Node**: The sequential number of the node starting from 0.
2. **ID**: The identifier for the node (e.g., T01, S01), where 'T' stands for Turbine and 'S' stands for Substation.
3. **X**: The X-coordinate of the node's location in euclidian coordinates.
4. **Y**: The Y-coordinate of the node's location in euclidian coordinates.
5. **Demand**: The demand of the node. For turbines, this is a positive value representing their maintenance time demand. For substations, this value is 0.
6. **Kind**: The type of node, either "Turbine" or "Substation".

## Operational Parameters

Following the node data, several key operational parameters are listed.

1. **num_vessels**: The number of vessels available for operations.
2. **charge_capacity**: The energy capacity of each vessel [kWh].
3. **velocity**: The speed of the vessels [knots].
4. **consumption_rate**: The rate at which the vessels consume energy [kWh/m].
5. **vessel_cost**: The cost associated with operating a vessel.
6. **station_cost**: The cost associated with each station.
7. **sailing_cost**: The cost per unit distance for sailing.
8. **num_time_windows**: The number of time windows available for during the planning period.
