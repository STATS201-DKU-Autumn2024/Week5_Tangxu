# Predictive Maintenance Data for Vehicle Systems

This project uses two comprehensive datasets to explore predictive maintenance in vehicle systems. The **MetroPT dataset** (Veloso et al. 2022) provides a detailed archive of maintenance activities, operational metrics, and failure events from Lisbon's metro system. It is structured to support predictive maintenance modeling, offering valuable insights into operational patterns and component degradation.

Additionally, the **Turbofan Engine Degradation Simulation Data Set** (Saxena and Goebel 2008) from NASA’s Prognostics Data Repository includes time-series sensor data on turbofan engines under simulated degradation conditions. This dataset captures real-time wear patterns in high-stress components, supporting the development of models focused on early failure detection.

These datasets allow for the integration of multimodal data to enhance predictive maintenance across transportation sectors.

## References
- Saxena, A., & Goebel, K. 2008. "Turbofan Engine Degradation Simulation Data Set." NASA Prognostics Data Repository, NASA Ames Research Center, Moffett Field, CA. https://data.nasa.gov/Aeorspace/CMAPSS-Jet-Engine-Simulated-Data/ff5v-kuh6
- Veloso, B., Gama, J., Ribeiro, R., & Pereira, P. 2022. "MetroPT: A Benchmark Dataset for Predictive Maintenance." Zenodo. https://doi.org/10.5281/zenodo.6854240.

Here is a structured data dictionary for the datasets:
# Data Dictionary for the Predictive Maintenance Project

## MetroPT Dataset

| **Variable**       | **Description**                                                                                 | **Type**   | **Unit**              |
|--------------------|-------------------------------------------------------------------------------------------------|------------|------------------------|
| COMPONENT_ID       | Unique identifier for each component in the metro system.                                       | Integer    | -                      |
| MAINTENANCE_TYPE   | Type of maintenance activity performed (e.g., preventive, corrective).                          | String     | -                      |
| FAILURE_EVENT      | Indicates whether a failure occurred (1 = Yes, 0 = No).                                         | Integer    | -                      |
| OPERATIONAL_HOURS  | Total hours of operation for the component at the time of maintenance or failure.               | Float      | Hours                  |
| TEMPERATURE        | Recorded temperature for the component or system during operation.                              | Float      | Degrees Celsius        |
| VIBRATION_LEVEL    | Measured vibration level of the component during operation.                                     | Float      | m/s²                   |
| INSPECTION_DATE    | Date of the most recent inspection or maintenance activity.                                     | Date       | YYYY-MM-DD             |

## NASA Turbofan Engine Degradation Simulation Dataset (FD001, FD002, FD003, FD004)

| **Variable**           | **Description**                                                                                             | **Type**   | **Unit**          |
|------------------------|-------------------------------------------------------------------------------------------------------------|------------|--------------------|
| UNIT_NUMBER            | Unique identifier for each engine in the dataset.                                                           | Integer    | -                 |
| TIME_CYCLES            | Time in operational cycles, representing a single unit of operation for the engine.                         | Integer    | Cycles            |
| OP_SETTING_1           | Operational setting 1, one of three settings affecting engine performance.                                  | Float      | -                 |
| OP_SETTING_2           | Operational setting 2, affecting engine performance in various conditions.                                  | Float      | -                 |
| OP_SETTING_3           | Operational setting 3, another parameter influencing engine performance under different conditions.         | Float      | -                 |
| SENSOR_1               | Sensor measurement 1, indicative of engine condition and performance.                                       | Float      | -                 |
| SENSOR_2               | Sensor measurement 2, representing real-time engine metrics.                                                | Float      | -                 |
| SENSOR_3 to SENSOR_26  | Additional sensor measurements (3-26) capturing various engine conditions and degradation metrics.          | Float      | -                 |
| RUL (Test Set only)    | Remaining Useful Life (RUL) values provided for test data, indicating the number of cycles remaining until failure. | Integer | Cycles            |

### Dataset Summary
- **FD001**: 100 train and 100 test trajectories, one operational condition (Sea Level) and one fault mode (HPC Degradation).
- **FD002**: 260 train and 259 test trajectories, six operational conditions and one fault mode (HPC Degradation).
- **FD003**: 100 train and 100 test trajectories, one operational condition (Sea Level) and two fault modes (HPC Degradation, Fan Degradation).
- **FD004**: 248 train and 249 test trajectories, six operational conditions and two fault modes (HPC Degradation, Fan Degradation).

This data dictionary outlines the key variables across multiple subsets (FD001-FD004) within the dataset, capturing time-series sensor readings, operational settings, and real-time metrics essential for predictive maintenance modeling.
