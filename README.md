# docker-learnings

Recording the learnings @psbanka and I achieve from the [Developing and Delivering Software with Docker](https://www.linkedin.com/learning/paths/developing-and-delivering-software-with-docker?u=83558730) series

## Docker Orchestration

[Specifically, this course](https://www.linkedin.com/learning/docker-essential-training-2-orchestration/welcome?autoplay=true&contextUrn=urn%3Ali%3AlyndaLearningPath%3A5bb4fa9b498e2e532e6df920&u=83558730)

### What do we know before hand? 
* What is Kubernetes? 
It is an orchestration tool that can be used in conjunction with docker to... do stuff?
- plumb connections between containers
- container healthchecks
- dynamic starting and stopping
- adding resources
- rmanaging volumes? 
- managing container dependencies on one another (don't start the app until the DB is up and healthy)

### What it turns out we're learning
[Docker Swarm](https://docs.docker.com/engine/swarm/)! (Is this what Devly is built on?)
[Docker v. Kubernetes](https://circleci.com/blog/docker-swarm-vs-kubernetes/#:~:text=Docker%20Swarm%20is%20a%20lightweight,capabilities%20out%20of%20the%20box)

- What is a node?
An instance of a Docker engine? 
**Manager Nodes:**
Assign tasks to workers
Manage the state of the cluster/swarm

**Worker Nodes:**
Carry out the tasks
Notify the manager of the current state
May also _be_ a manager node? Because reasons?


Docker docs gonna Docker docs. This shit is not helpful.