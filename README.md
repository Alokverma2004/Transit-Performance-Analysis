Swift Assignment Summary: Transit Performance Analysis
This project analyzes shipment tracking data from a courier logistics network to evaluate transit performance, operational efficiency, and delivery accuracy. The dataset, provided in nested JSON format, contains detailed shipment and event-level tracking information (including facility movements, timestamps, and delivery milestones).

Objective
To extract, process, and analyze courier shipment data to compute key logistics performance indicators such as:

Total transit time, facility touchpoints, and inter-facility movement efficiency

Average transit velocity and service-type comparison

Delivery success metrics (first-attempt delivery rates, out-for-delivery attempts)

Approach
The analysis was performed in six structured phases:

Data Loading & Exploration: Loaded and inspected the hierarchical JSON data structure to identify key shipment and event attributes.

Data Flattening: Extracted shipment-level and event-level details into a structured tabular DataFrame for analysis.

Transit Metric Computation: Calculated per-shipment performance metrics — including total transit hours, facility visits, inter-facility transit time, and delivery attempts.

Edge Case Handling: Implemented robust handling for missing fields, inconsistent timestamps ($numberLong vs ISO), null addresses, empty event arrays, and duplicate timestamps.

Detailed Output Generation: Exported a clean, shipment-level dataset (transit_performance_detailed.csv) with all computed metrics standardized and timestamped in IST.

Network Summary Analysis: Produced an aggregated summary file (transit_performance_summary.csv) capturing overall network trends, facility utilization, service-type comparison, and delivery performance statistics.

Outcome
The final outputs enable a clear view of courier network performance:

Average transit time: ~94 hours (≈3.9 days)

Average facilities per shipment: 2.8

First-attempt delivery rate: ~85%

Service analyzed: FedEx Express Saver

This end-to-end analysis provides actionable insights into shipment flow efficiency, delivery accuracy, and potential bottlenecks in transit operations — forming the foundation for data-driven logistics optimization.
