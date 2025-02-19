{% note info %}

Since projects run on different {{ yandex-cloud }} platforms with different computing resources, {{ ml-platform-name }} does not guarantee that RAM will be 100% available.

{% endnote %}



| Name | Number of vCPUs | Number of GPUs | RAM, GB |
---- | ---- | ---- | ----
**Configurations with vCPU on the [Intel Cascade Lake platform](../../../compute/concepts/performance-levels.md)**
**c1.4** (default) | 4 | 0 | 32
**c1.8** | 8 | 0 | 64
**c1.32** (available upon request to technical support) | 32 | 0 | 256
**c1.80** (available to legal entities upon request to technical support) | 80 | 0 | 640
**Configurations with vCPU on [Intel Broadwell](../../../compute/concepts/performance-levels.md) and GPU [NVIDIA® Tesla® V100](../../../compute/concepts/gpus.md)**
**g1.1** (available upon request to technical support or with an account balance of at least $10) | 8 | 1 | between 48 and 96
**g1.2** (available upon request to technical support) | 16 | 2 | between 96 and 192
**g1.4** (available upon request to technical support) | 32 | 4 | between 192 and 384
**Configurations with vCPU on [AMD EPYC™](../../../compute/concepts/gpus.md) and GPU [NVIDIA® Ampere® A100](https://www.nvidia.com/en-us/data-center/a100/)**
**g2.mig** | 4 | 1/8 | 16
**g2.1** (available upon request to technical support) | 28 | 1 | 119
**g2.2** (available upon request to technical support) | 56 | 2 | 238
**g2.4** (available upon request to technical support) | 112 | 4 | 476
**g2.8** (available upon request to technical support) | 224 | 8 | 952


