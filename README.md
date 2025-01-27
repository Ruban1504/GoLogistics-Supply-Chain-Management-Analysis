# Go-Logistics -  Last-Mile Logistics Optimization

![picture](https://imgur.com/mYRbiRM.png)
![picture](https://imgur.com/UUZQ8mv.png)

## Overview
This repository contains a project focused on optimizing last-mile logistics operations using **Business Intelligence (BI)**  and **Data Analysis** techniques. It leverages the **last Miles Dataset** to improve delivery efficiency, reduce costs, and enhance customer satisfaction.

---

## Problem Statement
GoLogistics faces inefficiencies in last-mile delivery operations due to suboptimal allocation of delivery partners. This project addresses the challenges of:
1. Increasing delivery costs.
2. Delays caused by traffic and poor route planning.
3. Underutilization of delivery partner resources.

---

## Objectives
- **BI Analysis**: Create dashboards to monitor delivery performance, costs, and regional trends.
- **Report**: Createreport for each dashboard summarizing the insight and calculations performed in the dashboard.
---

## Dataset
The **Dataset** is a real-world dataset containing:
- **10 million+ package records**.
- Information about delivery times, locations, traffic density, and courier performance.
- Six months of data from diverse regions, including Shanghai and Hangzhou.
---

## Project Workflow

1. **Data Preprocessing**:
   - Clean raw data.
   - Engineer features like `delivery_distance` and `traffic_impact`.
   - Tools: Excel, JupyterNotebook.

2. **BI Dashboards**:
   - Visualize KPIs: delivery cost trends, partner performance, and delay analysis.
   - Develop charts that aids to the analysis.
   - Tools: Power BI, Excel.

3. **Documentation**:
   - Documented all the data preprocessing and pushed to github repo.

Description
Below is the detailed field of each sub-dataset.
## Pickup Dataset
| Data field                 | Description                                  | Unit/format  |
|----------------------------|----------------------------------------------|--------------|
| **Package information**    |                                              |              |
| package_id                 | Unique identifier of each package             | Id           |
| time_window_start          | Start of the required time window             | Time         |
| time_window_end            | End of the required time window               | Time         |
| **Stop information**       |                                              |              |
| lng/lat                    | Coordinates of each stop                      | Float        |
| city                       | City                                         | String       |
| region_id                  | Id of the Region                              | String       |
| aoi_id                     | Id of the AOI (Area of Interest)              | Id           |
| aoi_type                   | Type of the AOI                               | Categorical  |
| **Courier Information**    |                                              |              |
| courier_id                 | Id of the courier                             | Id           |
| **Task-event Information** |                                              |              |
| accept_time                | The time when the courier accepts the task    | Time         |
| accept_gps_time            | The time of the GPS point closest to accept time | Time       |
| accept_gps_lng/lat         | Coordinates when the courier accepts the task | Float        |
| pickup_time                | The time when the courier picks up the task   | Time         |
| pickup_gps_time            | The time of the GPS point closest to pickup_time | Time       |
| pickup_gps_lng/lat         | Coordinates when the courier picks up the task | Float        |
| **Context information**    |                                              |              |
| ds                         | The date of the package pickup                | Date         |


## Delivery Dataset
| Data field            | Description                          | Unit/format   |
|-----------------------|--------------------------------------|---------------|
| **Package information**   |                                      |               |
| package_id            | Unique identifier of each package     | Id            |
| **Stop information**      |                                      |               |
| lng/lat               | Coordinates of each stop              | Float         |
| city                  | City                                 | String        |
| region_id             | Id of the region                      | Id            |
| aoi_id                | Id of the AOI                         | Id            |
| aoi_type              | Type of the AOI                       | Categorical   |
| **Courier Information**   |                                      |               |
| courier_id            | Id of the courier                     | Id            |
| **Task-event Information**|                                      |               |
| accept_time           | The time when the courier accepts the task | Time      |
| accept_gps_time       | The time of the GPS point whose time is the closest to accept time | Time |
| accept_gps_lng/accept_gps_lat | Coordinates when the courier accepts the task | Float |
| delivery_time         | The time when the courier finishes delivering the task | Time |
| delivery_gps_time     | The time of the GPS point whose time is the closest to the delivery time | Time |
| delivery_gps_lng/delivery_gps_lat | Coordinates when the courier finishes the task | Float |
| **Context information**  |                                      |               |
| ds                    | The date of the package delivery      | Date          |

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Ruban1504/GoLogistics-Supply-Chain-Management-Analysis.git
