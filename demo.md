```mermaid
---
config:
  flowchart:
    curve: linear
---
graph TD;
	__start__([<p>__start__</p>]):::first
	analyze_job(analyze_job)
	generate_application(generate_application)
	review_application(review_application)
	reject_application(reject_application)
	__end__([<p>__end__</p>]):::last
	__start__ --> analyze_job;
	analyze_job -.-> generate_application;
	analyze_job -.-> reject_application;
	generate_application --> review_application;
	reject_application --> __end__;
	review_application --> __end__;
	classDef default fill:#f2f0ff,line-height:1.2
	classDef first fill-opacity:0
	classDef last fill:#bfb6fc


```
