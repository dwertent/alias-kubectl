# Kubectl alias

List of alias I found useful when running the `kubectl` command.

Feel free to suggest any other aliases 🤓

### Convention

`<kubectl>` `<command>` `<kind>`

e.g.

* `kubectl get deployment`   -> `kgd`
* `kubectl get replicaset`   -> `kgrs`
* `kubectl delete pod`       -> `kdp`
* `kubectl describe service` -> `kdess`
* `kubectl edit namespace`   -> `kens` 


### Usage

Clone project and add to `~/.bashrc` file ->

1. Clone repo
1. `vim ~/.bashrc`
3. paste (edit file location):
    ```
    if [ -f <path-to-cloned-repo>/kubectl_aliases ]; then
        source <path-to-cloned-repo>/kubectl_aliases
    fi
    ```

#### BASIC

| alias | command |
| --- | --- |
| `k` | `kubectl` |
| `kl` | `kubectl logs` |
| `kexec` | `kubectl exec -it` |
| `kpf` | `kubectl port-forward` |
| `kaci` | `kubectl auth can-i` |
| `katt` | `kubectl attach` |
| `kapir` | `kubectl api-resources` |
| `kapiv` | `kubectl api-versions` |

#### GET

| alias | command |
| --- | --- |
| `ke` | `kubectl get` |
| `kens` | `kubectl get namespaces` |
| `kep` | `kubectl get pods` |
| `ked` | `kubectl get deployments` |
| `kes` | `kubectl get secret` |
| `kers` | `kubectl get replicasets` |
| `kess` | `kubectl get statefulsets` |
| `keds` | `kubectl get daemonsets` |
| `kesvc` | `kubectl get services -o wide` |
| `ken` | `kubectl get nodes -o wide` |
| `kecm` | `kubectl get configmaps` |
| `kecj` | `kubectl get cronjobs` |
| `kej` | `kubectl get jobs` |
| `kesa` | `kubectl get serviceaccounts` |
| `ker` | `kubectl get roles` |
| `kerb` | `kubectl get rolebindings` |
| `kecr` | `kubectl get clusterroles` |
| `kecrb` | `kubectl get clusterrolebindings` |
 
#### DESCRIBE

| alias | command |
| --- | --- |
| `kd` | `kubectl describe` |
| `kdns` | `kubectl describe namespaces` |
| `kdp` | `kubectl describe pods` |
| `kdd` | `kubectl describe deployments` |
| `kds` | `kubectl describe secret` |
| `kdrs` | `kubectl describe replicasets` |
| `kdss` | `kubectl describe statefulsets` |
| `kdds` | `kubectl describe daemonsets` |
| `kdsvc` | `kubectl describe services -o wide` |
| `kdn` | `kubectl describe nodes -o wide` |
| `kdcm` | `kubectl describe configmaps` |
| `kdcj` | `kubectl describe cronjobs` |
| `kdj` | `kubectl describe jobs` |
| `kdsa` | `kubectl describe serviceaccounts` |
| `kdr` | `kubectl describe roles` |
| `kdrb` | `kubectl describe rolebindings` |
| `kdcr` | `kubectl describe clusterroles` |
| `kdcrb` | `kubectl describe clusterrolebindings` |

#### EDIT

| alias | command |
| --- | --- |
| `ke` | `kubectl edit` |
| `kens` | `kubectl edit namespaces` |
| `ked` | `kubectl edit deployments` |
| `kers` | `kubectl edit replicasets` |
| `kes` | `kubectl edit secret` |
| `kess` | `kubectl edit statefulsets` |
| `keds` | `kubectl edit daemonsets` |
| `kesvc` | `kubectl edit services` |
| `kecm` | `kubectl edit configmaps` |
| `kecj` | `kubectl edit cronjobs` |
| `kesa` | `kubectl edit serviceaccounts` |
| `ker` | `kubectl edit roles` |
| `kerb` | `kubectl edit rolebindings` |
| `kecr` | `kubectl edit clusterroles` |
| `kecrb` | `kubectl edit clusterrolebindings` |

#### DELETE

| alias | command |
| --- | --- |
| `kdel` | `kubectl delete` |
| `kdelns` | `kubectl delete namespaces` |
| `kdelp` | `kubectl delete pods` |
| `kdeld` | `kubectl delete deployments` |
| `kdelrs` | `kubectl delete replicasets` |
| `kdelss` | `kubectl delete statefulsets` |
| `kdelds` | `kubectl delete daemonsets` |
| `kdelsvc` | `kubectl delete services` |
| `kdels` | `kubectl delete secret` |
| `kdelcm` | `kubectl delete configmaps` |
| `kdelcj` | `kubectl delete cronjobs` |
| `kdelj` | `kubectl delete jobs` |
| `kdelsa` | `kubectl delete serviceaccounts` |
| `kdelr` | `kubectl delete roles` |
| `kdelrb` | `kubectl delete rolebindings` |
| `kdelcr` | `kubectl delete clusterroles` |
| `kdelcrb` | `kubectl delete clusterrolebindings` |

#### DRY-RUN (MOCK)

| alias | command |
| --- | --- |
| `kmock` | `kubectl create mock -o yaml --dry-run=client` |
| `kens` | `kubectl create mock -o yaml --dry-run=client namespaces` |
| `kecm` | `kubectl create mock -o yaml --dry-run=client configmaps` |
| `kesa` | `kubectl create mock -o yaml --dry-run=client serviceaccounts` |

#### CONFIG

| alias | command |
| --- | --- |
| `kcfg` | `kubectl config` |
| `kcfgv` | `kubectl config view` |
| `kcfgns` | `kubectl config set-context --current --namespace` |
| `kcfgcurrent` | `kubectl config current-context` |
| `kcfgsc` | `kubectl config set-context` |
| `kcfggc` | `kubectl config get-contexts` |
| `kcfguc` | `kubectl config use-context` |
