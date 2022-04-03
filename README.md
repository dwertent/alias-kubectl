# Kubectl alias

List of alias I found useful when running the `kubectl` command.

Feel free to suggest any other aliases 🤓

### Convention

`<kubectl>` `<command>` `<kind>`

e.g.

* `kubectl get deployment`   -> `kgd`
* `kubectl get replicaset`   -> `kgrs`
* `kubectl delete pod`       -> `kdp`
* `kubectl describe service` -> `kds`
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