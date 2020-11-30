Banker's Algorithm is used majorly in the banking system to avoid deadlock.

X: Indicates the total number of processes of the system.
Y: Indicates the total number of resources present in the system.
Available
[I: Y] indicate which resource is available.

Max
[l:X,l: Y]: Expression of the maximum number of resources of type j or process i

Allocation
[l:X,l:Y]. Indicate where process you have received a resource of type j

Need
Express how many more resources can be allocated in the future



Step 1) When a total requested instance of all resources is lesser than the process, move to step 2.

Step 2) When a requested instance of each and every resource type is lesser compared to the available resources of each type, it will be processed to the next step. Otherwise, the process requires to wait because of the unavailability of sufficient resources.

Step 3) Resource is allocated as shown in the below given Pseudocode.


             Available = Available – Request (y)
             Allocation(x) = Allocation(x) + Request(x)
             Need(x) = Need(x) - Request(x)
