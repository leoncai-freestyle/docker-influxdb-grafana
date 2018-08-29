#run docker-compose on web server
#check haproxy?stat url is working or not
curl http://52.64.148.2:8181/haproxy?stats
#modify inputs in telegraf
 [[inputs.haproxy]]
    servers = ["http://52.64.148.2:8181/haproxy?stats"]
#import dashboards to grafana
https://grafana.com/dashboards/1234
#if cannot see the data in influxdb check firewall

