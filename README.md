# Formula 1 - Medallion Architecure Using Azure Data Explorer

## Overview
Real-Time Insights: Building a Medallion Architecture for Formula 1 Telemetry with Azure Data Explorer

  ![](./assets/architecture-1.png)

## Requirements
- Forza Mortorsport (Xbox or PC)
- .NET 8
- Forza-Telemetry-Bridge (https://github.com/clemensv/forza-telemetry-bridge)
  - I added some additional telemetry channels, so demo is based on my fork (https://github.com/calloncampbell/forza-telemetry-bridge) 
- Azure Subscription (sign up for [free](https://azure.microsoft.com/en-us/free))
- Azure Data Explorer (get a [free personal cluster](https://dataexplorer.azure.com/))

## Setup
1. Download the Forza-Telemetry-Bridge and follow its installation and configuration.
1. Configurat Forza Mortorsport and go into Settings and enable the UDP Telemetry.
1. Create a free Azure Data Explorer Cluster and create a new database.
1. Run the KQL scripts from this repository to create the tables, functions and materialized views.
1. Create an Azure Data Explorer Dashboard. There is a dashboard file in this repository, just import it and update the data source accordingly.
1. Run the Forza-Telemetry-Bridge console application.
1. Start a race.
1. Analyze your results.

## YouTube
Here is a video I published for one of my racing sessions and then displaying the results in a real-time dashboard:
https://youtu.be/3URkoaY6ogc