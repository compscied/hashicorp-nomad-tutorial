# Hashicorp Nomad Tutorial

**What is Nomad?**
- Nomad is cluster manager and scheduler designed for microservices and batch workloads. Nomad is distributed, highly available, and scales to thousands of nodes spanning multiple datacenters and regions.
- Nomad provides a common workflow to deploy applications across an infrastructure. Developers use a declarative job specification to define how an application should be deployed and the resources it requires (CPU, memory, disk). Nomad accepts these jobs and finds available resources to run them. The scheduling algorithm ensures all constraints are satisfied, and packs as many applications on a host as possible to optimize resource utilization. Additionally, Nomad supports virtualized, containerized, or standalone applications running on all major operating systems giving it the flexibility to support a broad range of workloads.
 
**Let's start first by downloading nomad**
- https://www.nomadproject.io/downloads.html

**Unzip**
- unzip nomad*.zip

**Run nomad**
- ./nomad

You should see output
~~~~~~~
usage: nomad [--version] [--help] <command> [<args>]

Available commands are:
    agent                 Runs a Nomad agent
    agent-info            Display status information about the local agent
    alloc-status          Display allocation status information and metadata
    client-config         View or modify client configuration details
    eval-status           Display evaluation status and placement failure reasons
    fs                    Inspect the contents of an allocation directory
    init                  Create an example job file
    inspect               Inspect a submitted job
    logs                  Streams the logs of a task.
    node-drain            Toggle drain mode on a given node
    node-status           Display status information about nodes
    plan                  Dry-run a job update to determine its effects
    run                   Run a new job or update an existing job
    server-force-leave    Force a server into the 'left' state
    server-join           Join server nodes together
    server-members        Display a list of known servers and their status
    status                Display status information about jobs
    stop                  Stop a running job
    validate              Checks if a given job specification is valid
    version               Prints the Nomad version
~~~~~~~

**Run nomad agent in dev mode**
- ./nomad agent -dev

**Let's query the status**
- ./nomad agent-info

**Next lets install vagrant**
https://www.vagrantup.com/docs/installation/

you might need to install virtualbox you have not already
https://www.virtualbox.org/wiki/Downloads
