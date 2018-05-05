# A paper list on distributed systems

## Algorithms

1. Nancy Lynch. Distributed Algorithms. *Book*. 

2. Consensus. 

    1. Leslie Lamport. [The Part-Time Parliament](https://www.microsoft.com/en-us/research/publication/part-time-parliament/). TOCS, 16(2), 1998.  **(Paxos)**
  
    2. Leslie Lamport. [Paxos Made Simple](https://www.microsoft.com/en-us/research/publication/paxos-made-simple/). ACM SIGACT News (Distributed Computing Column) 32, 4 (Whole Number 121, December 2001).  
  
    3. Romain Boichat, Partha Dutta, Svend Frolund and Rachid Guerraoui. [Destructing Paxos](http://www.cs.utexas.edu/~lorenzo/corsi/cs380d/papers/deconstr_paxos.pdf). ACM SIGACT News, Volume 34, Issue 1, March 2003.
   
    4. D. Ongaro and J. Ousterhout. [In Search of an Understandable Consensus Algorithm](https://web.stanford.edu/~ouster/cgi-bin/papers/raft-atc14). In USENIX ATC, June 2014.  **(Raft)**
   
    5. Miguel Castro and Barbara Liskov. [Practical Byzantine Fault Tolerance](http://pmg.csail.mit.edu/papers/osdi99.pdf). In OSDI, 1999.  **(PBFT)**
  
    6. Jean-Philippe Martin, Lorenzo Alvisi. [Fast Byzantine Consensus](http://www.cs.cornell.edu/lorenzo/papers/fab.pdf). IEEE Transactions on Dependable and Secure Computing, Volume 3 Issue 3, July 2006.
    
    7. Douglas B. Terry, Marvin M. Theimer, Karin Petersen, Alan J. Demers, Mike J. Spreitzer and Carl H. Hauser. [Managing update conflicts in Bayou, a weakly connected replicated storage system](https://dl.acm.org/citation.cfm?id=224070). In SOSP, 1995. 

3. Conflict-free Replicated Data Types (CRDTs). 

    1. Wiki: [Conflict-free replicated data type](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type).  

    2. M. Shapiro, N. Preguica, C. Baquero, and M. Zawirski. [A Comprehensive Study of Convergent and Commutative Replicated Data Types](https://hal.inria.fr/inria-00555588/document). Technical Report 7506, INRIA, 2011.
   
    3. M. Shapiro, N. Preguica, C. Baquero, and M. Zawirski. [Conflict-Free Replicated Data Types](http://lip6.fr/Marc.Shapiro/papers/RR-7687.pdf). In SSS, 2011.
    
    4. [Readings in conflict-free replicated data types](http://christophermeiklejohn.com/crdt/2014/07/22/readings-in-crdts.html). 
    
    5. H.-G. Roh, M. Jeon, J.-S. Kim, and J. Lee. [Replicated Abstract Data Types: Building Blocks for Collaborative Applications](https://sites.google.com/site/myeongjae/). J. Parallel Distrib. Comput., 71(3), 2011.
    
    6. S. Weiss, P. Urso, and P. Molli. [Logoot: A Scalable Optimistic Replication Algorithm for Collaborative Editing on P2P Networks](https://hal.inria.fr/inria-00432368/file/main.pdf). In ICDCS, 2009.
   
    7. Hagit Attiya, Sebastian Burckhardt, Alexey Gotsman, Adam Morrison, Hongseok Yang, and Marek Zawirski. [Specification and Complexity of Collaborative Text Editing](http://software.imdea.org/~gotsman/papers/editing-podc16.pdf). In PODC, 2016. 
    
    8. A. Bieniusa, M. Zawirski, N. Preguic¸a, M. Shapiro, C. Baquero, V. Balegas and S. Duarte. [An optimized conflict-free replicated set](https://arxiv.org/pdf/1210.3368.pdf). Technical Report 8083, INRIA, 2012.

    9. Y. Sovran, R. Power, M. K. Aguilera, and J. Li. [Transactional Storage for Geo-Replicated Systems](https://dl.acm.org/citation.cfm?id=2043592). In SOSP, 2011.
    
4. Possibly Non-Commutative Replicated Data Types.

    1. Nicholas V. Lewchenko, Arjun Radhakrishna and Pavol Černý. [Conflict-Aware Replicated Data Types](https://arxiv.org/pdf/1802.08733.pdf). Draft. 

    2. S. Burckhardt, M. Fahndrich, D. Leijen, and B. P. Wood. [Cloud Types for Eventual Consistency](https://link.springer.com/chapter/10.1007/978-3-642-31057-7_14). In ECOOP, 2012.

5. Operational Transformation.

    1. Wiki: [Operational transforation](https://en.wikipedia.org/wiki/Operational_transformation).
    
    2. C. A. Ellis and S. J. Gibbs. [Concurrency control in groupware systems](https://perso.telecom-paristech.fr/kuznetso/INF346-2015/papers/opertr.pdf). In SIGMOD, 1989. 
    
    3. Ariel J. Feldman, William P. Zeller, Michael J. Freedman and Edward W. Felten. [SPORC: Group Collaboration using Untrusted Cloud Resources](https://www.usenix.org/legacy/event/osdi10/tech/full_papers/Feldman.pdf). In OSDI, 2010. 

6. Databases.

    1. Wiki: [Key-value database](https://en.wikipedia.org/wiki/Key-value_database). 

    2. G. DeCandia et al. [Dynamo: Amazon’s Highly Available Key-Value Store](https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf). In SOSP, 2007.
    
    3. [Amazon DynamoDB](http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/APISummary.html). 
    
    4. [Riak](http://docs.basho.com/riak/kv/2.2.3/developing/). 
    
    5. [Microsoft Azure Cosmos DB](https://docs.microsoft.com/en-us/azure/cosmos-db/consistency-levels).

## Consistency Definitions

1. Eventual Consistency.

    1. Sebastian Burckhardt. [Principles of Eventual Consistency](https://www.microsoft.com/en-us/research/publication/principles-of-eventual-consistency/). Foundations and Trends in Programming Languages, vol. 1, no. 1-2, pp. 1–150, 2014.

    2. S. Burckhardt, D. Leijen, M. Fahndrich, and M. Sagiv. [Eventually consistent transactions](https://www.microsoft.com/en-us/research/publication/eventually-consistent-transactions/). In ESOP, 2012.   **("operational")**
    
    3. Matthieu Perrin, Achour Mostefaoui and Claude Jard. [Causal consistency: beyond memory](https://hal.archives-ouvertes.fr/hal-01286755/document). In PPoPP, 2016.  **("with sequential specifications")**
    
    4. Douglas B. Terry, Alan J. Demers, Karin Petersen, Mike Spreitzer, Marvin Theimer, and Brent W. Welch. [Session guarantees for weakly consistent replicated data](http://www.cs.utexas.edu/~dahlin/Classes/GradOS/papers/SessionGuaranteesPDIS.pdf). In PDIS, 1994.
    
    5. A. Fekete, D. Gupta, V. Luchangco, N. Lynch, and A. Shvartsman. [Eventually-serializable data services](https://groups.csail.mit.edu/tds/papers/Lynch/podc96-esds.pdf). In PODC, 1996.
    
    6. Lucas Brutschy, Dimitar Dimitrov, Peter Müller, and Martin Vechev. [Serializability for Eventual Consistency: Criterion, Analysis, and Applications](https://www.sri.inf.ethz.ch/papers/popl17-serializability.pdf). In POPL, 2017. 

    7. Andrea Cerone, Alexey Gotsman, and Hongseok Yang. [Algebraic laws for weak consistency](http://software.imdea.org/~gotsman/papers/vis2rf-concur17.pdf). In CONCUR, 2017. 

    8. Alexey Gotsman and Sebastian Burckhardt. [Consistency models with global operation sequencing and their composition](http://software.imdea.org/~gotsman/papers/gsp-disc17.pdf). In DISC, 2017. 

    9. Alexey Gotsman and Hongseok Yang. [Composite replicated data types](http://software.imdea.org/~gotsman/papers/compos-esop15.pdf). In ESOP, 2015. 
    
2. Mixed Consistency.

    1. Matthew P. Milano and Andrew C. Myers. [MixT: A Language for Mixing Consistency in Geodistributed Transactions](http://www.cs.cornell.edu/andru/papers/mixt/mixt.pdf). In PLDI, 2018. 

    2. KC Sivaramakrishnan, Gowtham Kaki and Suresh Jagannathan. [Declarative programming over eventually consistent data stores](http://kcsrk.info/papers/quelea_pldi15.pdf). In PLDI, 2015. 

    3. C. Li, J. Leitao, A. Clement, N. M. Preguica, R. Rodrigues and V. Vafeiadis. [Automating the choice of consistency levels in replicated systems](https://www.usenix.org/system/files/conference/atc14/atc14-paper-li_cheng.pdf). In USENIX ATC, 2014.

    4. C. Li, D. Porto, A. Clement, R. Rodrigues, N. Preguica and J. Gehrke. [Making geo-replicated systems fast if possible, consistent when necessary](http://www.cs.otago.ac.nz/cosc440/readings/osdi12-final-162.pdf). In OSDI, 2012.  **(RedBlue Consistency)**

    5. V. Balegas, N. Preguic¸a, R. Rodrigues, S. Duarte, C. Ferreira, M. Najafzadeh and M. Shapiro. [Putting the consistency back into eventual consistency](https://pages.lip6.fr/Marc.Shapiro/papers/putting-consistency-back-EuroSys-2015.pdf). In EuroSys, 2015.

3. For Transactions. 

    1. Wiki: [Snapshot isolation](https://en.wikipedia.org/wiki/Snapshot_isolation); [Serializability](https://en.wikipedia.org/wiki/Serializability).
    
    2. Andrea Cerone, Alexey Gotsman and Hongseok Yang. [Transaction chopping for parallel snapshot isolation](http://software.imdea.org/~gotsman/papers/chopping-disc15.pdf). In DISC, 2015. 

    3. Andrea Cerone and Alexey Gotsman. [Analysing snapshot isolation](http://software.imdea.org/~gotsman/papers/si-jacm.pdf). Journal of the ACM, 65(2), 11:1-11:41. ACM, 2018. 

    4. Andrea Cerone, Giovanni Bernardi and Alexey Gotsman. [A framework for transactional consistency models with atomic visibility](http://software.imdea.org/~gotsman/papers/framework-concur15.pdf). In CONCUR, 2015. 

    5. Giovanni Bernardi and Alexey Gotsman. [Robustness against consistency models with atomic visibility](http://software.imdea.org/~gotsman/papers/robustness-concur16.pdf). In CONCUR, 2016. 

## Verification

1. Sebastian Burckhardt, Alexey Gotsman, Hongseok Yang, and Marek Zawirski. [Replicated Data Types: Specification, Verification, Optimality](http://software.imdea.org/~gotsman/papers/distrmm-popl14.pdf). In POPL, 2014.

2. Alexey Gotsman, Hongseok Yang, Carla Ferreira, Mahsa Najafzadeh, and Marc Shapiro. ['Cause I'm strong enough: reasoning about consistency choices in distributed systems](http://software.imdea.org/~gotsman/papers/logic-popl16.pdf). In POPL, 2016. 

3. Álvaro García-Pérez, Alexey Gotsman, Yuri Meshman, and Ilya Sergey. [Paxos consensus, deconstructed and abstracted](http://software.imdea.org/~gotsman/papers/paxos-esop18.pdf). In ESOP, 2018. 

4. James R. Wilcox, Doug Woos, Pavel Panchekha, Zachary Tatlock, Xi Wang, Michael D. Ernst and Thomas Anderson. [Verdi: A Framework for Implementing and Formally Verifying Distributed Systems](https://homes.cs.washington.edu/~ztatlock/pubs/verdi-wilcox-pldi15.pdf). In PLDI, 2015. 

5. Doug Woos, James R. Wilcox, Steve Anton, Zachary Tatlock, Michael D. Ernst and Thomas Anderson. [Planning for Change in a Formal Verification of the Raft Consensus Protocol](https://verdi.uwplse.org/raft-proof.pdf). In CPP, 2016. 

6. C. Hawblitzel et al. [IronFleet: Proving Practical Distributed Systems Correct](https://web.eecs.umich.edu/~manosk/assets/papers/ironfleet.pdf). In SOSP, 2015. 

7. Vincent Rahli, Ivana Vukotic, Marcus Völp and Paulo Esteves-Verissimo. [Velisarios: Byzantine Fault-Tolerant Protocols Powered by Coq](https://link.springer.com/chapter/10.1007/978-3-319-89884-1_22). In ESOP, 2018. 

8. Pedro Fonseca, Kaiyuan Zhang, Xi Wang and Arvind Krishnamurthy. [An Empirical Study on the Correctness of Formally Verified Distributed Systems](). In EuroSys, 2017. 

9. Ilya Sergey, James R. Wilcox and Zachary Tatlock. [Programming and proving with distributed protocols](https://homes.cs.washington.edu/~jrw12/disel.pdf). In POPL, 2018.

10. Ahmed Bouajjani, Constantin Enea, Rachid Guerraoui and Jad Hamza. [On verifying causal consistency](https://dl.acm.org/citation.cfm?id=3009888). In POPL, 2017.  **(Decidability, Model Checking)**

11. Hengfeng Wei, Yu Huang and Jian Lu. [Specification and Implementation of Replicated List: The Jupiter Protocol Revisited](https://arxiv.org/pdf/1708.04754.pdf). Draft. 

12. 
