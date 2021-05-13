# gcp-helloworld

Simple gcp-helloworld chart.

## Installing the Chart

Install the chart.

```
helm install gcp-helloworld .
```

## Reaching public endpoint

Get the public IP and the node port you need to issue a browser request

```
kubectl describe services gcp-helloworld
```

```
curl http://<load-balancer-ingress-ip>:<http-node-port>
```

You would see a message something like

```
Congratulations, you successfully deployed a Kubernetes application with Cloud Code!
```
