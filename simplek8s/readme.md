# apiVersion

- `apiVersion` specifies the types of objects we can create within a given configuration file.

<img src="./assets/Screen%20Shot%202021-10-20%20at%201.53.15%20PM.png">

# kind

- `kind` represents the "kind of `object` we are trying to make".
- Question: What exactly is an `object`? What are they used for?
  - They are essentially things that are going to be created inside our k8s cluster to get our application to work they way we would expect. Every type of object we create has a slightly different purpose.
    - `Pods` are used to run containers.
    - `Services` set up networking.

# Pods

- Question: _What is a pod_?
  - When `minicube start` is ran from terminal, our computer starts up a virtual machine. We refer to this virtual machine as a `node`. A `pod` is a grouping of containers with a very specific purpose. In kubernetes we have no ability to run a single naked container. The smallest thing that can be deployed is a `pod`, or more specifically, a `pod` containing `containers`.
- Requirement of a `pod` we must run 1 or more `containers` inside of it.
- Importantly, a `pod` should group together `containers` with a very specific purpose.

<img src="./assets/Screen%20Shot%202021-10-20%20at%201.56.31%20PM.png">
<img src="./assets/Screen%20Shot%202021-10-20%20at%202.33.10%20PM.png">
<img src="./assets/Screen%20Shot%202021-10-20%20at%202.41.58%20PM.png">
