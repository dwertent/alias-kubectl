# Kubectl alias

List of alias I found useful when running `kubectl` command.

Feel free to suggest other alias.

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


### Convention

`<kubectl>` `<command>` `<kind>`

e.g. : `kubectl get deployment`   -> `kgd`
e.g. : `kubectl get replicaset`   -> `kgrs`
e.g. : `kubectl delete pod`       -> `kdp`
e.g. : `kubectl describe service` -> `kds`
e.g. : `kubectl edit namespace`   -> `kens`
