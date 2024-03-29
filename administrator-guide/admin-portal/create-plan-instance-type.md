# Create/Plan Instance Type

**Instance Type**, is a resources allocation setting. According to the it, PrimeHub will try to allocate these resources for launching an instance for a JupyterHub or a Job if vacant resources are sufficient.

This quick-start shows how to crete an instance type and give an advice of planning them according to a real circumstance (CPUs/MEM/GPUs).

### Advice of Plan

In a real circumstance, we have to manage/arrange resources of CPUs, Memory or even GPUs. For the sake of resources utilization, via instance types, we can plan our resources for different groups/projects according to different demands for computing resources. A good arrangement of instance types can not only utilize resources efficient, but also can prevent an instance from occupying massive resources.

Since PrimeHub cluster uses certain of resources for operating the cluster properly, we are not able to allocate all of resources for running instances. _It is recommended to leave 10%-15% resources of CPU/MEM for the cluster itself._

Projects require various computing resources. We can start arranging/planning our instance types for different scales of resources allocations (such as small/medium/large), users can choose the appropriate scale of instance type for projects for the allocation of requested resources. We, of course, can create a specific instance type for a specific project as well.

If you are new to plan instance types, here is an advice.

**Let's assume a circumstance of \_CPU 40 / MEM 512GB / GPU 4**\_**:**

#### CPU-Only instance type

| Scale  | CPU | Mem  | % of Total |
| ------ | --- | ---- | ---------- |
| Small  | 4   | 128G | 10-25      |
| Medium | 16  | 256G | 40-60      |
| Large  | 32  | 420G | 80+        |

#### GPU-Equipped instance type

| Scale  | CPU | Mem  | GPU | % of Total |
| ------ | --- | ---- | --- | ---------- |
| Small  | 4   | 128G | 1   | 10-25      |
| Medium | 16  | 256G | 2   | 40-60      |
| Large  | 32  | 420G | 4   | 80+        |

### Let's Add Instance Types

According to our plan, let's create instance types for users, here we will create a GPU-equipped instance type of medium-scale.

1. Log in as an administrator and [switch to Admin Portal](./).
2. Enter `Instance Types` management.
3. Fill in `Name` with _medium-with-gpu_.
4. Fill in `CPU Limit` with _16_ and fill in `Memory Limit` with _256GB_.
5. Fill in `GPU Limit` with _2_.
6. (Optional) `Overcommitting`, if required, enabled it and fill in `CPU Request` with _14_ and `Memory Request` with _200GB_. More detail \[[Overcommitting](../instance-type-management/#overcommitting-advanced-feature)].
7. Click `edit groups` and select groups which can have this instance type.
8. (Optional) `Tolerations` if required: \[[Reference](../instance-type-management/toleration.md)]
9. (Optional) `NodeSelector` if required: \[[Reference](../instance-type-management/nodeselector.md)]
10. Click `Confirm` to save it.

### Next

We have created the instance type, _medium-with-gpu_, which requests medium-scale resources allocation and assigned it to groups. Users who belong to these groups are able to select it for launching instances. Next, let's add images as working environments for instances.
