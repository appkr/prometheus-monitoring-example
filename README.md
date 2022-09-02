## Prometheus monitoring example on MacOS

### Run

```shell
$ docker compose up
```

```shell
# grafana, Login with admin / secret
$ open http://localhost:3000

# prometheus
$ open http://localhost:9090
# http://localhost:9090/metrics

# cadvisor
$ open http://localhost:8000
# http://localhost:8000/metrics

# node exporter
# $ curl -s http://localhost:9100/metrics
# http://localhost:9100/metrics
```

### Issue

Exporters like cadvisor, node-exporter are designed for Linux OS. Barely work on Mac OS!! 

### References

- [Monitoring a Linux host with Prometheus, Node Exporter, and Docker Compose ](https://grafana.com/docs/grafana-cloud/quickstart/docker-compose-linux/)
- [DOCKER - PROMETHEUS AND GRAFANA WITH DOCKER-COMPOSE](https://www.bogotobogo.com/DevOps/Docker/Docker_Prometheus_Grafana.php)
- [dockprom](https://github.com/stefanprodan/dockprom)
- [A Prometheus & Grafana docker-compose stack](https://github.com/vegasbrianc/prometheus) 
- [Docker and system monitoring
](https://grafana.com/grafana/dashboards/893-main/)