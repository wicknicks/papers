# Papers 

Scrub: Online TroubleShooting for Large Mission-Critical Applications
---------------------------------------------------------------------

Conference paper [pdf](https://github.com/wicknicks/papers/blob/master/scrub-eurosys18.pdf), published at [ACM DL](https://dl.acm.org/citation.cfm?id=3190513), presented at [Eurosys 18](http://eurosys2018.org/).

Scrub is a troubleshooting tool for distributed applications that operate under strict SLOs common in production environments. It allows users to formulate queries on events occurring during execution in order to assess the correctness of the application’s operation.

Scrub has been in use for two years at Turn, where developers and users have relied on it to resolve numerous issues in its online advertisement bidding platform. This platform spans thousands of machines across the globe, serving several million bid requests per second, and dispensing many millions of dollars in advertising budgets.

Troubleshooting distributed applications is notoriously hard, and its difficulty is exacerbated by the presence of strict SLOs, which requires the troubleshooting tool to have only minimal impact on the hosts running the application. Furthermore, with large amounts of money at stake, users expect to be able to run frequent diagnostics and demand quick evaluation and remediation of any problems. These constraints have led to a number of design and implementation decisions, that go counter to conventional wisdom. In particular, Scrub supports only a restricted form of joins. Its query execution strategy eschews imposing any overhead on the application hosts. In particular, joins, group-by operations and aggregations are sent to a dedicated centralized facility. In terms of implementation, Scrub avoids the overhead and security concerns of dynamic instrumentation. Finally, at all levels of the system, accuracy is traded for minimal impact on the hosts.

Discovering Context to Prune Large and Complex Search Spaces
------------------------------------------------------------

Conference paper [pdf](https://github.com/wicknicks/papers/blob/master/cuenet-context17-final.pdf), published at [Springer Link](https://link.springer.com/chapter/10.1007/978-3-319-57837-8_7), presented at [Context 17](http://context17.lip6.fr/).

Journal paper [pdf](https://github.com/wicknicks/papers/blob/master/cuenet-openscience18-final.pdf), published at [OpenScience](https://www.openscience.fr/Discovering-Context-for-Real-World-Events). 

Abstract
--------

Specifying the search space is an important step in designing multimedia annotation systems. With the large amount of data available from sensors and web services, context-aware approaches for pruning search spaces are becoming increasingly common. In these approaches, the search space is limited by the contextual information obtained from a fixed set of sources. For example, a system for tagging faces in photos might rely on a static list of candidates obtained from the photo owner’s Facebook profile. These contextual sources can get extremely large, which leads to lower accuracy in the annotation problem.

We present our novel Context Discovery Algorithm, a technique to progressively discover the most relevant search space from a dynamic set of context sources. This allows us to reap the benefits of context, while keeping the size of the search space within bounds.

As a concrete application for our approach, we present a simple photo management application, which tags faces of people in a user’s personal photos. We empirically study the role of CueNet in the face tagging application to tag photos taken at real world events, such as conferences, weddings or social gatherings. Our results show that the availability of event context, and its dynamic discovery, can produce 80% smaller search spaces with nearly 100% correct tags

