# Airbyte v2 
Hey, this is ramesh, if you'd like to install your own version of airbyte do the following : 
1. Add the airbyte helm repo
``` bash
helm repo add airbyte-v2 https://airbytehq.github.io/charts
helm repo update
```

2. Then modify the current `values.yaml` as per your liking and deploy: 
``` bash
# find compatible chart versions
helm search repo airbyte-v2 --versions

# you can install Airbyte 2.0 with chart 2.0.18
helm install airbyte airbyte-v2/airbyte \
  --namespace airbyte-v2 \
  --values ./values.yaml \
  --version 2.0.18
```

## Airbyte Deps : 
This Directory involves all the necessary tools and values required to test airbyte locally using minikube :smirk:
feel free to use it or contribute to it