# App-prereq-helm-chart

## Logging and Monitoring Deployment

## Objective
Deploying EFK, Prometheus and Grafana on Kubernetes Cluster using Helm Chart 

### Maintainer
<table>
    <thead>
      <tr>
        <th>Name</th>
        <th>NUID</th>
      </tr>
    </thead>
    <tbody>
        <tr>
            <td>Akshay Babaji Phapale</td>
            <td>001316563</td>
        </tr>
        <tr>
            <td>Naresh Agrawal</td>
            <td>001054600</td>
        </tr>
    </tbody>
</table>

### Technology Stack
* Kubernetes
* Helm chart            

### Prerequisites
* Kubernetes Cluster
* Helm


### Build Instructions
- To deploye EFK stack
```
 $ helm install logging --namespace logging ./efk-stack/
```

- To deploye Prometheus
```
 $ helm install prometheus --namespace monitoring ./prometheus/
```

- To deploye Grafana
```
 $helm install grafana --namespace monitoring ./grafana/
```

<b>Note</b>: Change variables value according to need in values.yaml

### Destroy Instruction 
- To destroy EFK stack
```
 $ helm delete logging --namespace logging
```

- To destroy Prometheus
```
 $ helm delete prometheus --namespace monitoring 
```

- To destroy Grafana
```
 $helm delete grafana --namespace monitoring
```