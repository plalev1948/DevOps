<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<h1> DevOps Goals </h1>
<!-- <p> <p> -->
</head>

<body>
<div class="main-paragraph">
<h2> The Big Picture in DevOps: </h2>

<h3> What is Lean all about? </h3>

* Focus on value
* Eliminate waste
* One-piece flow
* Continuous learning
* No overburdening of people
* Apply Theory of Constraints

<h3> How Lean Relates to Software Delivery? </h3>

* Reorient towards product thinking
* Remove wasteful processes
* Continuously deliver software in small batches
* Focus on continuous improvement
* Automate to remove overburdening of staff
* Attack bottlenecks that decrease flow

<h3> Defining DevOps </h3>
DevOps represents a change in IT culture, focusing on rapid IT service delivery through the adoption of agile, lean practices in the context of a system-oriented approach. It can also be seen as: a combination of cultural philosophies, practices, and tools that increase an organization's ability to deliver applications and services at high velocity.

<h3> What DevOps Is Not </h3>

* DevOps is not a team or software methodology
* DevOps is not something you buy
* DevOps is not an IT-only effort
* DevOps is not just automating infrastructure
* DevOps is not easy!

<h3> Adopting DevOps Culture, Practices, and Technologies </h3>

* The Cultural changes
* The Organizational changes
* The Practice and Process changes
* The Technologies that are part of DevOps
  * `Lean method for visualizing, analyzing, and improving the delivery process` - Identidy bottlenecks, create cross-org collaboration, and provide context about how you deliver value; Create by talking to stakeholders, collecting data, observing processes - solutions in this space from Lucidchart, Atlassian, and Tasktop
  * `Embrace Flexible Planning Tools` - create Kanban boards or use methods to track priorities and WIP - use Trello or Jira
  * `Consolidate Issue Tracking Systems` - use a shared system to capture and assign issues - solutions from Zendesk, GitHub and Atlassian
  * `Expand your use of Source Control` - manage changes to code, configurations, scripts used to deliver software - solutions from GitHub, GitLab and Bitbucket
  * `Employ a Range of Testing Tools` - solutions from JUnit, XUnit, JMeter, Selenium and Gremlin
  * `CI/CD Pipelines` - create automation to merge, build, package and deploy software; it's done to get fast quality feedback and ship value to the customer more often - solutions from Jenkins, CircleCI and cloud vendors
  * `Leverage Configuration Management` - establish consistency for infrastructure and applications through automation; develop more stable systems - solutions Terraform, Ansible and Puppet
  * `Take Advantage of Public Clouds` - API-driven platforms for on-demand, elastic infrastructure and services; reduce waiting waste, while getting fully automated provisioning and management of planet-scale systems - solutions in this space frm Google, Microsoft and Amazon
  * `Improve Monitoring and Observability` - instrument software and processes to capture data about system state and user interactions; increase transparency, identify problems - solutions Datadog, Splunk and New Relic
  * `Infuse Security Practices Throughout` - enabling automated security checks throughout the software delivery process; improve software quality, increase empowerment of team members, and build confidence with stakeholders - solutions Snyk, Twistlock and Aqua

<h2> Core Concepts and Fundamentals in DevOps: </h2>

* The principles of Lean Development - eliminate waste;
* least privilege principle
* deliver early means `deliver fast` - this will help facilitate feedback and deliver often
* `The seven Wastes` = `partially done work`, `extra features`, `relearning`, `handoffs`, `task switching`, `delays`, `defects`
* creating quality in a lean context = `pareto analysis`; optimize the human experience and `create interoperability` means compose the one, true build

<h2> Understanding What DevOps Replaces: </h2>

The effect on version control:
* all this feeds back into version control practices
* you merge too often
* all the merge conflicts landed on his plate

To create a Build you need a `build engine` and a `build script`.

* Demo: a super-simple build:

* `dotnet new webapp --name BuildWebApp`
* `cd BuildWebApp`
* `cls`
* `dir`
* `dotnet build` = this is the build command

After that select a build tool.

* `git init` = initialize the repo

`Infrastructure as Code` means one simple thing, a script to build your infrastructure from the ground up. This includes using Docker and containers as well.
`IaC` is typically JSON. `Configuration Drift` = configuration changes after the initial IaC sync; you need to keep your infrastructure in configuration.

* Demo: Infrastructure as Code Approaches:

Look into an Azure Resource Template in Azure, how it works, running a simple Dockerfile and talk about how that would work.

* Secrets and Security in DevOps
  * `Secrets` do not belong in version control. They belong in a secure store.
  * `Security` belongs in version control.


<h2> Verifying Knowledge in DevOps: </h2>

* `How a build fails is at least as important as how it succeeds.`


<div>
</body>
</html>