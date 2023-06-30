# kubeplugin
## Instalation
- Download kubeplugin
    ```bash
    curl -O https://github.com/spolish/kubeplugin/raw/main/script/kubeplugin
    ```
- Add permissions to the file
    ```bash
    sudo chmod +x kubeplugin 
    ```
- Move file to /usr/local/bin
    ```bash
    sudo cp ./kubeplugin /usr/local/bin/kubectl-kubeplugin
    ```
- Check plugin list 
    ```bash
    kubectl plugin list
    ```

## Usage
 ```bash
kubectl kubeplugin [<resource_type>] [<namespace>]
```

## Example
```bash
kubectl kubeplugin pod  kube-system
Resource   Namespace       Name                                     CPU      Memory
pod        kube-system     local-path-provisioner-76d776f6f9-gr2b4  1/1        Running
pod        kube-system     coredns-59b4f5bbd5-wjg8g                 1/1        Running
pod        kube-system     metrics-server-7b67f64457-56tfs          1/1        Running
pod        kube-system     helm-install-traefik-crd-q5cbr           0/1        Completed
pod        kube-system     helm-install-traefik-96dml               0/1        Completed
pod        kube-system     traefik-56b8c5fb5c-22jw8                 1/1        Running
pod        kube-system     svclb-traefik-35557e4f-7fpvv             2/2        Running
```
