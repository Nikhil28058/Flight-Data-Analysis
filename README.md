# Introduction-to-Big-Data

# Flight Data Analysis Project

## Project Overview

This project involves analyzing a large flight dataset using Apache Hadoop and Oozie workflows. We designed and implemented three main tasks to derive insights related to flight schedules, airport taxi times, and flight cancellations. The dataset for this project is sourced from Harvard University ([Dataset Link](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/HG7NV7)).

## Key Analysis Tasks

### 1. **On-Schedule Performance Analysis**
- **Objective**: Identify airlines with superior on-time performance and those with frequent delays.
- **Method**: Analyze flight schedules, departure/arrival times, and delay data.
- **Outcome**: Ranks the top 3 and bottom 3 airlines based on on-time performance.

### 2. **Airport Taxi Time Analysis**
- **Objective**: Examine taxi times at various airports to assess efficiency.
- **Method**: Analyze the taxi-in and taxi-out times for departing and arriving flights.
- **Outcome**: Identifies airports with efficient ground operations and areas needing improvement.

### 3. **Flight Cancellation Analysis**
- **Objective**: Investigate the common reasons behind flight cancellations.
- **Method**: Analyze cancellation data, focusing on weather, operational constraints, and other factors.
- **Outcome**: Identifies the most common causes of cancellations, helping to mitigate disruptions.

## Project Structure

### 1. **Data Source**:  
The dataset used contains flight information over several years, including details such as departure/arrival times, delays, taxi times, and cancellations.

### 2. **Oozie Workflow**:  
An Oozie workflow was implemented to manage and execute three map-reduce programs for the different analysis tasks.

### 3. **Performance Evaluation**:  
We evaluated the system's performance based on two criteria:
- **Increase in Virtual Machines (VMs)**: Analyzed how performance improves as the number of VMs increases.
- **Increase in Dataset Size**: Analyzed how the execution time increases as the dataset size grows.

## PseudoCode and Algorithms

- The project uses custom mappers and reducers to process the flight data.
- Detailed pseudocode and algorithm descriptions are available for each analysis task.

## Performance Insights

- **VM Scaling**: Increasing the number of VMs initially improves performance, but diminishing returns are observed after a certain point.
- **Data Scaling**: As the dataset size increases, the time required for workflow execution increases linearly, with additional factors like data distribution and resource management playing a critical role.

## Running the Project

1. **Prerequisites**:
   - Apache Hadoop and Oozie should be installed and configured.
   - Ensure access to the flight dataset from the provided link.

2. **Execution**:
   - Use the provided Oozie workflow file to schedule and execute the map-reduce programs.

3. **Output**:
   - The output will consist of ranked lists of airlines based on performance, taxi time analysis, and cancellation reasons.

## Conclusion

This project demonstrates the application of Hadoop and Oozie in analyzing large-scale datasets to derive actionable insights related to flight operations. By focusing on flight schedules, taxi times, and cancellations, we provide a comprehensive understanding of operational efficiency and potential areas for improvement in the airline industry.
