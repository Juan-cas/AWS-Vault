2024-10-06 16:07

Status:

Tags:
[[AWS Orchestration & Management Index]]

# AWS Step Functions

You can create workflows, also called [State Machines](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-statemachines.html), to build distributed applications, automate processes, orchestrate micro-services, and create data and machine learning pipelines.

Step Functions is based on "state machines and tasks". In step functions, state machines are called workflows, which are a series of event-driven steps. Each step in a workflow is called a state.

For example, a Task state represents a unit of work that another AWS service performs, such as calling another AWS service or API. instances of running workflows performing tasks are called executions in Step functions.

the work in your state machine tasks can also be done using Activities which are workers that exist outside of Step Functions.

Example diagram:

![[AWS Step functions Diagram.png]]

References 
[AWS Step Functions](https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html)