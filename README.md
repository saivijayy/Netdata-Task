# Data Analyst Internship - Task 7: Monitor System Resources Using Netdata

## Objective:
In this task, we used Netdata, an open-source real-time monitoring tool, to monitor system resources such as CPU, memory, disk, and Docker containers.

## Tools Used:
- **Netdata** (Docker-based monitoring tool)
- **Docker**

## Task Steps:
### 1. Run Netdata via Docker:
   We used the following Docker command to run Netdata in a container:

   ```bash
   docker run -d --name=netdata -p 19999:19999 netdata/netdata
   ```
### 2. Access Netdata Dashboard:
```bash
Copy
Edit
http://localhost:19999
```
### 3. Explore Metrics: On the Netdata dashboard, we monitored real-time metrics for:

CPU usage

Memory usage

Disk usage

Docker containers

### 4. Explore Alerts and Chart Panels: We explored the various chart panels for system metrics and alerts. We also examined logs in /var/log/netdata for monitoring system activities.

Log files:

access.log

collector.log

debug.log

error.log

health.log

### 5. Netdata Logs: Logs were found in the /var/log/netdata directory in the container. They provided insights into the status of various Netdata components.

### 6. Insights:
Netdata offers a real-time monitoring interface for system performance.

It provides a quick view of essential KPIs like CPU, memory, and disk usage.

It can be easily deployed with Docker, and the dashboard is accessible via http://localhost:19999.

Log files and alert systems help in monitoring the health of the system.
