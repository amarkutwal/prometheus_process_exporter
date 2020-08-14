#A bash script to install the prometheus process_exporter on Linux servers.


## About process exporter
1. Prometheus exporter that mines /proc to report on selected processes. It grabs the processes related metrics from server and present to Prometheus.
2. It runs on port 9256 by default.
3. More information related process exporter can be found in https://github.com/ncabatoff/process-exporter

## About Prometheus
1. Prometheus is an open source, metrics-based monitoring and alerting system. It records real-time metrics in a time series database built using a HTTP pull model, with flexible queries and real-time alerting.
2. To know more about Prometheus visit https://prometheus.io/ 

## Deploy
Install the process exporter on those node which you wish to monitor using Prometheus. So basically it should be on client node. Although you can monitor Prometheus server process related metrics as well by install process exporter on your prometheus node as well.

        ```
        chmod u+x process_exporter.sh
        ```
        ```
        sh process_exporter.sh
        ```

