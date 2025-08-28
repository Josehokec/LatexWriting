
## Introduction
- The ubiquity and unprecedented growth of time-varying measurements across scientific and industrial settings are responsible for the increasing popularity of time-series analysis.
- In this work we propose the Transformer, a model architecture eschewing recurrence and instead relying entirely on an attention mechanism to draw global dependencies between input and output.
- To handle these distortions, dozens of distance measures have been proposed in the time-series literature.
- However, implementing a transaction engine on top of a programmable switch does not come "for free" and many challenges need to be addressed.
- There is a recent flurry of research on how to best integrate SIMD into column scans.
- We use the terms "point" and "record" interchangeably.
- LLMs truly have the potential to disrupt our entire field
- In most data systems that leverage LLMs for data processing, including those proposed in recent work, LLM operations are treated as a given, i.e., as black-box invocations on monolithic user inputs and data, where, akin to other types of UDFs, the data system doesn't attempt to fully understand the underlying data, user intent, or constituent operations, and just does as they are told.
- Simply showing raw execution traces or complete datasets is overwhelming and impractical, as users cannot reasonably review large amounts of data to verify correctness.
- Unfortunately, none of these technologies were designed for the specific demands of Internet of Things use cases, which include: (1), (2), and (3).
- While RDBMSes are unquestionably versatile, their generalization prevents them from being ideal for several recently identified use cases [9], one of which is IoT workloads.
- Albeit promising, tracking the wireless earphones is non-trivial.
- While EBS1 had been successfully deployed on more than 300 HDD-backed clusters, its limitations also unfolded. The straightforward virtualization led to severe space amplification and performance bottlenecks.

### Approach
- To address the MCTM problem, we develop two optimal algorithms that have different theoretical time complexity and no one can dominate the other in all possible cases.
- And while technically an equality predicate has no endpoint since it isn’t a range, for notational consistency we can think of S(x) as an endpoint of the predicate B = x.
- Also, with segmentation, failover is no longer at the granularity of the whole VD but a segment—BlockManager migrates the impacted segment to another BlockServer.
- EBS2 uses a similar network setup as EBS1 except for two fundamental differences. First, for the frontend network, we replace the kernel TCP with our user-space TCP implementation (called Luna [46]) over a 2×25 Gbps network. Luna achieves high performance (up to 3.5× throughput improvement and 53% latency reduction) by leveraging a run-to-completion thread model and a zero-copy memory model. Second, for the backend network, we use a 2 × 25 Gbps RDMA network to meet the demanding SLAs [29]. Note that the two changes above only affect the data path.
- The benefit is obvious since there are many fewer VDs influenced by a global event now. However, this approach, while straightforward and effective, would not alleviate regional and individual failure events.
- 
## Theoretical analysis 
- For the sake of convenience, we omit the proof to save the space.

## Reference
- For a comprehensive review of Bloom filters, see Broder and Mitzenmacher.
- We refer to the recent survey [xxx] for further details.

## Experiment
- The diagram unfolds a clear comparison between... and ...
- All experiments were conducted on a machine equipped with an Intel Xeon Gold 5218R CPU @ 2.10GHz (80 cores) with 256GB Memory. All algorithms are implemented in Python with the Numba library.
- Moreover, unless otherwise stated, we use the following system parameters. We set the number of monitors to 60.
- We now demonstrate that, contrary to state-of-the-art predicate evaluation methods, Column Sketches provide an efficient and robust access method regardless of data distribution, data clustering, or selectivity.
- For range queries, the period index performs in par with the interval tree and the 1D-grid.
- Since FG is not open-source, we implement FG from scratch faithfully following the original design principles, as well as caching the top-level nodes on compute nodes for better performance.
- Again, Figure X confirms that our technique is especially effective in XXX for XXX.
- Figure xxx sheds some insight on XXX.
- Our technique can improve xxx for three reasons. First, xxx. Second, xxx. Third, xxx.
- For range queries, the period index performs in par with the interval tree and the 1D-grid.
