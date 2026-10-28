# Kubectl alias

List of alias I found useful when running the `kubectl` command.

Feel free to suggest any other aliases 🤓

### Convention

`<kubectl>` `<command>` `<kind>`

e.g.

* `kubectl get deployment`   -> `kgd`
* `kubectl get replicaset`   -> `kgrs`
* `kubectl delete pod`       -> `kdp`
* `kubectl describe service` -> `kdsvc`
* `kubectl edit namespace`   -> `kens` 


### Usage

Clone the project and source it from your shell's startup file:

1. Clone repo
2. Pick the startup file for your shell (macOS defaults to zsh):
    * zsh -> `~/.zshrc`
    * bash -> `~/.bashrc` (on macOS, `~/.bash_profile`)
3. Append (edit file location):
    ```
    if [ -f <path>/alias-kubectl/kubectl_aliases ]; then
        source <path>/alias-kubectl/kubectl_aliases
    fi
    ```
    The path must point to the `kubectl_aliases` file itself, not the repo directory (`-f` is false for a directory, so nothing gets loaded).
4. Reload with `source ~/.zshrc` (or open a new terminal). Check with `alias k`.

> Use `~/.zshrc` rather than `~/.zprofile` so aliases load in every interactive terminal, not just login shells.

#### BASIC

| alias | command |
| --- | --- |
| `k` | `kubectl` |
| `kl` | `kubectl logs` |
| `kexec` | `kubectl exec -it` |
| `kpf` | `kubectl port-forward` |
| `kaci` | `kubectl auth can-i` |
| `kat` | `kubectl attach` |
| `kapir` | `kubectl api-resources` |
| `kapiv` | `kubectl api-versions` |

#### GET

| alias | command |
| --- | --- |
| `kg` | `kubectl get` |
| `kgns` | `kubectl get namespaces` |
| `kgp` | `kubectl get pods` |
| `kgd` | `kubectl get deployments` |
| `kgs` | `kubectl get secret` |
| `kgrs` | `kubectl get replicasets` |
| `kgss` | `kubectl get statefulsets` |
| `kgds` | `kubectl get daemonsets` |
| `kgsvc` | `kubectl get services -o wide` |
| `kgn` | `kubectl get nodes -o wide` |
| `kgcm` | `kubectl get configmaps` |
| `kgcj` | `kubectl get cronjobs` |
| `kgj` | `kubectl get jobs` |
| `kgsa` | `kubectl get serviceaccounts` |
| `kgr` | `kubectl get roles` |
| `kgrb` | `kubectl get rolebindings` |
| `kgcr` | `kubectl get clusterroles` |
| `kgcrb` | `kubectl get clusterrolebindings` |
 
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
| `kmockns` | `kubectl create ns mock -o yaml --dry-run=client` |
| `kmockcm` | `kubectl create cm mock -o yaml --dry-run=client` |
| `kmocksa` | `kubectl create sa mock -o yaml --dry-run=client` |

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
