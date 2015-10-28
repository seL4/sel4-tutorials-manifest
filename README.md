# seL4 Tutorial Manifests

These are the manifests for the seL4 and CAmkES tutorials. 

Please see [the sel4-tutorials repo](https://github.com/sel4-projects/sel4-tutorials.git) for more information.

## Main Manifests

There are four key manifests here, they will check out relevant repositories and set them up for:

[`sel4-tutorials.xml`](sel4-tutorials.xml)
- seL4 API and library exercises.  


[`camkes-tutorials.xml`](camkes-tutorials.xml)
- CAmkES exercises. 


[`sel4-solutions.xml`](sel4-solutions.xml)
- solutions for seL4 API and library exercises. 


[`camkes-solutions.xml`](camkes-solutions.xml)
- solutions for CAmkES exercises. 


To use a manifest do (for example, using `sel4-tutorials.xml`):

        mkdir sel4-tutorials
        cd sel4-tutorials
        repo init -u http://github.com/sel4-projects/sel4-tutorials-manifest -m sel4-tutorials.xml
        repo sync 


## Snapshots

There are also manifests in the [`snapshots`](snapshots) directory that freeze the state of the manifest at given points in time.  
We generally create a snapshot every time we present the tutorial to an external audience.

To use a snapshot manifest do (for example, using `sel4-tutorials.devday2.xml`):

        mkdir sel4-tutorials.devday2
        cd sel4-tutorials.devday2
        repo init -u http://github.com/sel4-projects/sel4-tutorials-manifest -m snapshots/sel4-tutorials.devday2.xml
        repo sync 
