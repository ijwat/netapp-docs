# NetApp FabricPool Technical Writing Project

## Overview

This technical writing project focuses on NetApp's FabricPool feature, detailing its architecture and setup within the ONTAP storage operating system. FabricPool allows for efficient data management by tiering less frequently accessed data (cold data) to lower-cost object storage while retaining frequently accessed data (hot data) on higher-performing storage.

## Project Components

### 1. Understanding FabricPool's Architecture

- **FabricPool Architecture**: Connects local storage with cloud storage to optimize data management. Hot data remains on the local tier, while cold data is moved to the cloud tier.
- **Key Concepts**:
  - **Block Temperature**: Blocks are classified as hot or cold based on usage, which impacts their storage location.
  - **Data Movement**: Cold blocks are collected into 4MB objects and transferred to the cloud tier based on configured thresholds.
  - **Volume Management**: Describes the behavior of data movement between local and cloud tiers, including the volume move process and its impact on performance.

[Full Architecture Documentation](https://github.com/ijwat/netapp-docs/blob/main/architecture.md)

### 2. Setting Up FabricPool

- **Cloud Tiering Configuration**: Ensure proper licensing and certificate installation before attaching third-party object storage.
- **Installation Process**:
  - Confirm cloud tiering licenses.
  - Retrieve and install CA certificates required for cloud tier integration.
  - Avoid common errors related to certificate verification during setup.
 
[Full Set Up Documentation](https://github.com/ijwat/netapp-docs/blob/main/setup.md) 

## Conclusion

The project demonstrates an understanding of NetApp's FabricPool, providing clear documentation on its architecture and setup procedures. This documentation serves as a valuable resource for users looking to implement FabricPool in their ONTAP systems.


