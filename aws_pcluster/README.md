# AWS ParallelCluster

## Install CLI

It is recommended to install AWS ParallelCluster CLI in a python virtual environment. [Install AWS ParallelCluster CLI in a virtual environment](https://docs.aws.amazon.com/parallelcluster/latest/ug/install-v3-virtual-environment.html)

```bash
pip install aws-parallelcluster
```

We can also install AWS CLI in the same virtual environment.

```bash
pip install awscli
```

## Getting Started

[AWS ParallelCluster User Guide v3](https://docs.aws.amazon.com/parallelcluster/latest/ug/install-v3-configuring.html)

- Since using free tier account, make sure the instance types are eligible for free tier when configuring a cluster.
- Region ca-central-1 has no rocky9 AMI (2025-09-21), we will use rehl9 instead.
  - We can also specify the custom AMI (can be found on rocky linux official site) id in the config file to use rocky9.
  - However,using the official AMI is recommended because slurm is pre-installed and configured on the official AMI.
