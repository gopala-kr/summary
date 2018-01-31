## <a name='consensus'> Consensus and Consistency

* [Paxos Made Simple](http://research.microsoft.com/en-us/um/people/lamport/pubs/paxos-simple.pdf) (2001): Paxos is a fault-tolerant distributed consensus protocol. It forms the basis of a wide variety of distributed systems. The idea is simple, but notoriously difficult to understand (perhaps due to the way the original Paxos paper was written).

* [The Raft Consensus Algorithm](https://ramcloud.stanford.edu/wiki/download/attachments/11370504/raft.pdf) (2014) : Raft is a consensus algorithm designed as an alternative to Paxos. It was meant to be more understandable than Paxos by means of separation of logic, but it is also formally proven safe and offers some new features.[1] Raft offers a generic way to distribute a state machine across a cluster of computing systems, ensuring that each node in the cluster agrees upon the same series of state transitions. 

* [CAP Twelve Years Later: How the "Rules" Have Changed](http://www.computer.org/cms/Computer.org/ComputingNow/homepage/2012/0512/T_CO2_CAP12YearsLater.pdf) (2012): The CAP theorem, proposed by Eric Brewer, asserts that any net­worked shared-data system can have only two of three desirable properties: Consistency, Availability, and Partition-Tolerance. A number of NoSQL stores reference CAP to justify their decision to sacrifice consistency. This is Eric Brewer's writeup on CAP in retrospective, explaining "'2 of 3' formulation was always misleading because it tended to oversimplify the tensions among properties."


## <a name='trends'> Trends (Cloud Computing, Warehouse-scale Computing, New Hardware)

* [A View of Cloud Computing](http://www.cs.berkeley.edu/~rxin/db-papers/cloudcomputing.pdf) (2010): This is THE paper on Cloud Computing. This paper discusses the economics and obstacles of cloud computing (referring to the elasticity of resources, not the consumer-facing "cloud") from a technical perspective. The obstacles presented in this paper will impact design decisions for systems running in the cloud.

* [The Datacenter as a Computer: An Introduction to the Design of Warehouse-Scale Machines](http://www.cs.berkeley.edu/~rxin/db-papers/WarehouseScaleComputing.pdf): Google's Luiz André Barroso and Urs Hölzle explains the basics of data center hardware and software for warehouse-scale computing. There is an [accompanying video](http://dl.acm.org/citation.cfm?id=2019527&bnc=1). The video talks about the importance of cutting long-tail latency in massively parallel systems. The other key idea is the disaggregation of resources. Technologies such as GFS/HDFS already disaggregate disks because of high network bandwidth, but yet to see the same trend applying to DRAMs because that'd require low-latency networking.
