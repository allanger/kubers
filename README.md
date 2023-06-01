# kubers
> Kubecl Reveal Secrets

kubers is a super simple tool that reveals k8s secrets using kubectl and yq

The tool requires `yq` and `kubectl`

Usage:
  kubers [-V | --version] [-h | --help] [-n | --namespace <namespace>] [-c <name>=<value>]
           <secret_name> [<entry_name>]

Examples:
  If you want to reveal all entries in the current k8s namespace
  
  ```
  $ kubers $SECRET_NAME
  ```
  
  If you want to reveal only one entry from the secret in the current namepspace 
 
  ```
  $ kubers $SECRET_NAME $SECRET_ENTRY
  ```

  If you want to reveal a secret from another namespace 

  ```
  $ kubers -n  $SECRET_NAME
  ```
