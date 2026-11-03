it's alpine with kubectl and jq installed

```yaml
apiVersion: "v1"
kind: "Pod"
metadata:
  name: "my-pod"
spec:
  serviceAccountName: "account-with-some-privileges"
  containers:
  - name: "kubectl-jq"
    image: "ghcr.io/mlibrary/kubectl-jq:latest"
    command:
    - "sh"
    - "-c"
    - |
      #!/bin/sh
      set -e

      # ...
```
