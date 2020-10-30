# CircleCI Workspaces vs. Caching  
  
## Introduction
This blurb will briefly describe the differences between Workspaces and Caching within CircleCI. Looking at the diagram below, you will find that the two serve very different purposes.
![image](workspaces.png)

## Workspaces
Workspaces are much like they sound -- spaces in which a run works. Think about the workspaces on your operating system. Each space contains data (applications, files, input from your keyboard, etc.) that can be shared amongst those applications and files. The same goes for workspaces in CircleCI. Per each run, a workspace is shared by all jobs, keeping data output from other jobs from within the same workspace, to be passed and consumed accordingly.

## Caching
Caching, on the other hand, serves a completely different purpose from workspaces. While the two both offer a means of storage,  a cache is shared run to run, as opposed to job to job. Think of the autofill feature on your computer. Each time you fill out a form, your browser becomes more efficient in the data it caches from the previous time you filled out a different form. This lowers the amount of time it takes you to fill out the new form. The same can be said for caches in CircleCI. Caches will save dependencies and source code in object storage in order to speed up the amount of time it takes to build between runs.

## Conclusion
As mentioned before and shown in the diagram, both workspaces and caching are storage mechanisms.  However, one serves as a container for job related data, while the other serves as a container for data related from run to run in its entirety (while also speeding up the runs themselves). In addition, workspaces live for the duration of the workflow, or sequence of jobs, whereas caches can live for months. All in all, both play a huge role in the efficiency of your CI/CD process.
