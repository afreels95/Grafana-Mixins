
# Prometheus Exporter <https://github.com/devinotelecom/prometheus-vmware-exporter>


# Example Docker-Compose Install of Exporter

```yaml
vmware-esxi-exporter:
       image: devinotelecom/prometheus-vmware-exporter
       container_name: vmware-exporter
       ports:
         - 9512:9512
       environment:
         - "ESX_HOST=url"
         - "ESX_USERNAME=username"
         - "ESX_PASSWORD=password"
         - "ESX_LOG=debug"
```
