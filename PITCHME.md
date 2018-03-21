
@title[Introduction]

# Elasticity Management

Note:
Introduce yourself. 
Show overview by showing table of contents.
Hope not to be boring 
---
@title[Elasticity]
# Elasticity

Note:
ask what is it? you can blackout
describe a person who is elastic

+++?image=assets/elasticity.png&size=auto 90%

@title[Example]

Note: 
describe what each axis means
give an example with reddit 

---
@title[Problems]
# Problems
- Elasticity requirements |
- Monitoring |
- Provisioning time | 

Note:
of course there are problems with elasticity
1. how do we know how much machines do we need
2. how do we measure the demand
3. how to be quick when we need to provision (describe what provisioning is)

+++

# Elasticity requirements

Note: 
for example when we go to the provider 
we need to tell him how much machines do we want on 1000 user
we need to not to take too much or too less machines
we take too much - we lose money
we take too less - we lose users
it is just individual - depends on the system - no clear way - just try and get the good result

+++

# Monitoring

Note:
how do we know how busy is our system
what do we need to measure 

+++

# Provisioning time

Note:
more low level
we need few machines, but all machines requires a setup which takes time
and we need it quick
usually, we have quite spare ones that are already setup

---

@title[How to make an application more elastic?]

## How can we make application more elastic?
- By solving the problems mentioned above |
- By having a scalable applications |

Note: 
0. ask the question 
1. solve every problem 
2. read it. ask what exactly does it mean? 

---

@title[Scalability]

# Scalability

Note:
Describe what scaling means normally
Describe what scalability is in cloud computing
the capability of a system, network, or process to handle a growing amount of work
give example with 100 users and 1 server, 1000 users and 10 or 20 servers

+++

## What is the difference between scalability and elasticity?

Note:
One may ask, what is the difference? 

+++?image=assets/elasticity.png&size=auto 90%

@title[Elasticity vs Scalability]

Note:
show on the screen where is elasticity and where is scalability
show them that they can see that more scalable - more elastic

---

# Types of scalability
- Vertical | 
- Horizontal |

Note: 
There are a few types of scalability
1. vertical
2. horizontal 
what does it mean? 

+++

# Vertical scalability
- boosting the server |
- short term |
- limited |

Note: 
ability to be better when adding more ram, getting better cpu etc. 
short term 
there is a limit for that

+++

# Horizontal scalability
- adding nodes |
- having load balancer |
- long term |
- complicated |

Note:
1. ability to perform better when adding nodes. describe what node is. example with aws having eu and us nodes. 
2. load balancer - balancing the incoming load. describe what it is.  
2.1 depends on the incoming protocol https or tcp, can choose different nodes.
2.2 different scheduling strategies - whole different presentation for that 
2.2.1 round robin, by cookies etc.
3. its long term. its easier to add another node then more ram
4. complicated - usually handled well by provider

---

# Problems 

+++

# Technology 
- single node vs multiple nodes |

Note:
1. proper architecture, for example node.js has only single node so it does not make sense. elixir
erlang got 2 million concurrent users on one server

+++

# Explosions 
- real explosions |
- power outage |

Note: 
what does it mean?
go through two points
what will happen if there is an explosion where one node is? 
usually we wont notice it - it is a responsibility of the provider
usually it happens automatically to change 

+++

# Bottleneck
- Database |
- Horizontal Partitioning (Sharding) |
- Vertical Partitioning |

Note:
0.what is  the bottleneck? get a bottle. imagine performance of the system as the pouring water into the bottle - bottle neck is something that is making our pouring go very slow 
1. database is almost always a bottle neck
its just slow. it is where all the data lays. 
2. for that we are using sharding - what is sharding? still we have to have a good architecture for that. it is complicated. For example we can have names from a to g in one db, from g to m in other etc.
3. multiplying data. example with instagram table. 


---

# Resilience

Note: 
Elasticity is also about resilience. What is resilience? Ability to recover from whatever error. for example, some machine fails, new one must be there. 

+++

# How to prevent errors? 
- Monitoring |
- Reacting quickly |
- Automating everything |

Note:
0. we would like to of course prevent errors. is it possible? 
1. we have to monitor everything constantly. and get messages of errors instantly
2. whenever we have an error we have to react quickly. sometimes it involves having someone hired exactly for that job.
3. we will try to automate everything. it reduces the work and need for devops engineer. reduces machine/software errors. introduces new human errors

+++

# Failure is normal 
## We should design for errors because they happen |

Note:
the truth is - we cannot really prevent them
0. failure is normal - ofc to some degree - we cannot have everything failing all over again
1. that is why we should design for errors. we should know how to solve them, when they happen, where they happen, have someone who can fix it. 

---

@title[Summary]

# Summary

Note:
elasiticity is how well we adapt to the changes
scalability is how well our system scales

---

@title[References]
# References
#### https://turbonomic.com/blog/on-technology/cloud-elasticity-vs-cloud-scalability/
#### https://en.wikipedia.org/wiki/Elasticity_(cloud_computing)
#### https://www.cloudassessments.com/blog/elasticity-cloud-computing/
