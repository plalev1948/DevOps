<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<h1> DevOps Goals </h1>
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

<h3> Understanding What DevOps Replaces: </h3>

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


<h3> Verifying Knowledge in DevOps: </h3>

* `How a build fails is at least as important as how it succeeds.`
* `Version control is an example of a first-class artifact.`
* `The product development cycle is the process of constructing certainty.`
* `Automated Deployment Wrap-up:`
  * `All DevOps is a combination of science and lore.`
  * `You want to maximize the science and minimize the lore.`
  * `The lore was the publish and artifact drop.`
  * `Don't be discourated, if you run into fiddly bits.`
* `We need two things when deplyoing a database so that it is consistent - a known state in the target db and a script to migrate us to the new state`

<h3> Adopting DevOps in Your Enterprise: </h3>

* `DevOps, Lean, and Agile in the broad sense are all just systems to force you to stop pretending that you know more than you really do.`

<h2> Test-driven Development in DevOps: </h2>

<h3> Why We Test </h3>

* `Test as Little as Possible, as much as Possible`
* `Many small tests, not fewer big tests`
* `The smaller the test, the more specific the knowledge created`

<h2> Understanding Test Automation and Test-driven Development </h2>

* `The TDD Paradigm:`
  * `Write a test from the spec`
  * `Make the code compile`
  * `Make the test pass`

* `Performance Testing`
  * `Benchmarking` - good for comparing different ways to solve problems; this is a type of unit testing;
  * `Load Testing` - type of integration testing;

<h2> Continuous Integration and Continuous Delivery </h2>

* `Integration` - consists of integration and build
* `Deployment` - consists of release, instructions and operations

<h3> Benefits of Continuous Integration: </h3>

* `Integration takes less effort`
* `Issues will come up more early`
* `Automation means less issues`
* `The process is more visible`
* `Improved team communication`
* `Short integration iterations means more flexibility`
* `The code is ready to be delivered more often`

<h3> Benefits of Continuous Delivery: </h3>

* `Releasing takes less effort`
* `Releasing is more reliable and repeatable`
* `Higher Quality`
* `Faster Delivery`
* `More Flexibility`

<h3> Advanced Continuous Delivery topics: </h3>

* `Blue-green Deployment`
* `Canary Release`
* `Feature Flags`

`Some times all of these items are called and are part of Progressive Delivery`.

* `GitOps`

<h3> Implement Continuous Integration: </h3>

* `Get to a Single Source Control Repository`
* `Create an Automated Process`
  * `Setup a dedicated server`
  * `Install a build engine`
  * `Create build definition(s)`
* `Create an Automated Test Process`
  * `Run static tests with the build`
  * `Deploy the build result to a (temporary) environment`
  * `Run (UI) tests`

<h3> Implement Continuous Delivery: </h3>

* `Have Continuous Integration in place`
* `Unite developers and Operations`
* `Deploy and Test the Release`
  * `Configure a deployment server`
  * `Create release definition(s)`
  * `Run tests`
* `Create an Iac Process`
  * `Scripts your environments`
  * `Create release definition(s)`
  * `Run tests`

<h2> Security and DevSecOps: </h2>

* `Protect your software supply chain`
* `Improve your security`
* `Incorporate automated scanning`

* `SDLC` = System development life cycle

* `Main points:`
  * `securing your pipeline`
  * `understanding scan standards`
  * `understanding scan categories`

* `STRIDE = spoofing, tampering, repudiation, information disclosure, evaluation of privilege`

<h3> Fitting Security Into Your Infrastructure: </h3>

* `We have a couple of different types of Infrastructures: there are virtual, cloud and Multi-platform Infrastructures`.
* `Run regular updates to your software for security reasons.`

<h3> Implement DevSecOps: </h3>

* `General best practices for implementing the philosophy of DevSecOps:`
  * `recruit partners`
  * `pick your "fights"`
  * `use the maturity models`
  * `follow industry developments`

* `The "shift left" philosophy means there is much value in moving the security interventions as close to the start of the pipeline as possible. `


</div>
</body>
</html>