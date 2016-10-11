# Bash scripts for generate ssl certificates for kubernetes

Scripts for generate and deploy ssl certificates mostly taken from https://github.com/coreos/coreos-kubernetes/tree/f6ad494c6b3ddfe127f95ef624f16e8e29821eff/lib

Example:

```./init-ssl-ca .```

```./init-ssl . master kube-master IP.1=138.68.145.154,IP.2=138.68.145.67,IP.3=188.166.159.81,IP.4=10.0.3.1```

```./init-ssl . kubelet kubelet IP.1=138.68.145.153,IP.2=10.131.20.85,IP.3=138.68.145.104,IP.7=10.3.0.1```

```./init-ssl . admin kube-admin```

```./deployer . /etc/kubernetes/ssl 138.68.145.154,138.68.145.67 core```