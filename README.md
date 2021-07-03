# helm-jaegar-operator

Example Helm chart for setting up Jaegar oeprator in your EKS cluster.


Table of Contents
=================

   * [helm-jaegar-operator](#helm-jaegar-operator)
      * [Pre-requisites](#pre-requisites)
         * [Namespace](#namespace)
      * [Install/Upgrade Chart](#installupgrade-chart)

## Pre-requisites

### Namespace

Create a new namespace `jaegar-operator` where we will install the operator.

```bash
kubectl create namespace jaegar-operator
```

## Install/Upgrade Chart

Run below commands to install/upgrade the chart.

```bash
helm upgrade -i jaegar-operator . -n jaegar-operator --values=stages/shared-values.yaml
```
