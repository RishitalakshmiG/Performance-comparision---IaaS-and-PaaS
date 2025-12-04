# Performance-comparision---IaaS-and-PaaS
Compares performance of IaaS and PaaS based on Response Time (Avg + Trend), CPU Usage, Memory Usage, Latency Percentiles: P50, P90, P95, P99, Throughput (Requests/sec), Error Rate (%), Scalability (low / medium / high load), Cost Efficiency. Performance Variance

Overview

This project presents a comprehensive performance comparison between Infrastructure as a Service (IaaS) and Platform as a Service (PaaS) using a Python-based benchmarking framework. The notebook evaluates both cloud service models across multiple performance metrics such as response time, throughput, error rate, CPU usage, and memory consumption under varying load conditions.

The goal is to provide a clear, measurable, and repeatable methodology for understanding the strengths and limitations of each cloud model using synthetic API tests.

Objectives

To benchmark IaaS and PaaS using consistent testing methodology.

To analyze performance under different load levels (low, medium, high).

To capture system-level metrics including CPU and memory usage.

To compare error tolerance and performance stability.

To calculate cost efficiency for both cloud models.

To generate visual insights and a structured dataset for further analysis.

Features

Automated benchmarking pipeline with configurable endpoints.

Multi-load performance testing with controlled concurrency.

Detailed metrics captured for each test run:

Response time

Throughput

Error rate

CPU and memory usage

Interactive visualizations using Plotly.

Aggregated analytics in tabular format using Pandas.

Cost efficiency calculation based on user input.

Automatic CSV export (advanced_cloud_benchmark.csv).

Modular, extensible benchmarking functions.

Project Structure
Performance_comparision_Iaas_and_Paas_.ipynb
README.md (you can place this content here)
data/
    advanced_cloud_benchmark.csv (generated after running)


Inside the notebook, the code is organized into the following logical sections:

Dependency Installation

Imports

Endpoint Definitions (IaaS and PaaS URLs)

Utility Functions for Requests

Load Testing Functions

System Resource Monitoring (CPU & Memory)

Data Aggregation and Analysis

Visualization with Plotly

Cost Efficiency Computation

Exporting Results

Requirements

The notebook automatically installs required packages.
Core dependencies include:

python 3.x
requests
psutil
pandas
numpy
plotly
concurrent.futures (built-in)
time (built-in)
statistics (built-in)


Optional (if running locally):

Jupyter Notebook or JupyterLab

Any modern Python environment (Conda, venv, etc.)

How to Run

Open the notebook in:

Jupyter Notebook

JupyterLab

Google Colab (recommended)

VS Code with Jupyter support

Run all cells sequentially.

When prompted, provide approximate cost values for:

IaaS cost

PaaS cost

The notebook will:

Run benchmarking for low, medium, and high loads

Collect system metrics

Generate visual analysis

Export results to CSV

After execution, download or view:

advanced_cloud_benchmark.csv

Plots shown inside the notebook

Evaluation Metrics

The notebook evaluates both cloud platforms on:

1. Response Time

Average, minimum, and maximum time per request.

2. Throughput

Requests successfully completed per second.

3. Error Rate

Percentage of failed or timed-out requests.

4. CPU Usage

Real-time process-level CPU consumption.

5. Memory Usage

RAM usage during each test cycle.

6. Stability Under Load

Performance consistency across low, medium, and high concurrency.

7. Cost Efficiency

Performance-to-cost ratio based on user-provided cost values.

8. Variance and Reliability

Statistical variance observed in response times.

Model Export and Usage

Although this project does not generate a machine learning model, it exports a benchmark dataset for reuse:

Exported File

advanced_cloud_benchmark.csv
This file contains:

Platform name (IaaS, PaaS)

Load category

Response times

Throughput

CPU and memory usage

Error rate

Cost metrics

You can use this dataset to:

Perform external visualization

Train ML models for performance prediction

Build decision-support dashboards

Integrate into DevOps or cloud monitoring workflows

Future Improvements

Add real cloud endpoints from AWS, Azure, or GCP for real-world benchmarking.

Include latency monitoring from multiple geographical regions.

Introduce network-level metrics such as packet loss and jitter.

Support additional benchmarking types such as:

Database read/write performance

File storage benchmarks

Scaling tests

Build a standalone CLI tool for automated cloud performance testing.

Export results to additional formats (JSON, Excel).

Integrate with cloud APIs for cost retrieval instead of manual input.
