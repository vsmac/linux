# Que.  What is Grafana?
# Ans.  Grafana is an open-source tool used for data monitoring and visualization from various data sources. It allows you to create customizable and interactive dashboards for viewing data in real-time.
 
 #  Key Features:
 #  Dashboards: Displays monitoring data with various visualizations (graphs, charts, gauges).
 # Multiple Data Sources: Can gather data from multiple sources like Prometheus, InfluxDB, MySQL, and Elasticsearch.
 # Alerts: Users can set alerts within their dashboards that send notifications via email, Slack, or other platforms.
 # Open-Source: Free and fully customizable with support for plugins.
 # Real-Time Monitoring: Continuously refreshes data to provide live monitoring capabilities.

                                                  
                    How to install grafana

1. # Install the prerequisite packages
    sudo apt-get install -y apt-transport-https software-properties-common wget

2. # Import the GPG key:
    sudo mkdir -p /etc/apt/keyrings/
wget -q -O - https://apt.grafana.com/gpg.key | gpg --dearmor | sudo tee /etc/apt/keyrings/grafana.gpg > /dev/null 

3. # To add a repository for stable releases, run the following command:
    echo "deb [signed-by=/etc/apt/keyrings/grafana.gpg ] https://apt.grafana.com stable main" | sudo tee -a /etc/apt/sources.list.d/grafana.list

4. # Run the following command to update the list of available packages:    
    sudo apt update
   
5. # To install Grafana OSS, run the following command:
    sudo apt-get install grafana-enterprise

# * Add rules 3000 for grafana