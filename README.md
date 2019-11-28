# kubectl-unbound-pvc

A small plugin to list Persistent Volume Claims which are not in `Bound` state.

## Prerequisites
* jq

## Installation

* Download the zip for the latest tag, for example:
  ```
  wget https://github.com/ishantanu/kubectl-unbound-pvc/archive/v0.0.1.zip
  ```
* Unzip the downloaded file
  ```
  unzip v0.0.1
  ```
* Move the `kubectl-unbound_pvc` binary from the `kubectl-unbound-pvc-0.0.1/` path and add it to your `$PATH`. For example:
  ```
  mv kubectl-unbound-pvc-0.0.1/kubectl-unbound_pvc /usr/local/bin/
  ```
* Now, you can start using the plugin right away:
  ```
  ❯ kubectl unbound-pvc -l
  NAME                      STATUS
  task-pv-claim             Pending
  task-pv-claim1            Pending
  ```
