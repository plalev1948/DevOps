<h1> Google Cloud Fundamentals: Core Infrastructure </h1>

<h2> Resources and Access in the Cloud: </h2>

Google Cloud’s resource hierarchy contains four levels, and starting from the bottom up they are:
* resources – These represent virtual machines, Cloud Storage buckets, tables in BigQuery, or anything else in Google Cloud. 
* projects;
* folders;
* organization node;

This resource hierarchy directly relates to how policies are managed and applied when you use Google Cloud. 

Each Google Cloud project has three identifying attributes: a project ID, a project name, and a project number. 

dentity and Access Management, or IAM is needed to restrict who has access to what. An IAM role is a collection of permissions. 

There are three kinds of roles in IAM:
* basic – they are quite broad in scope. They include owner, editor, viewer and billing administrator.
* predefined - 
* custom -

A word of caution: If several people are working together on a project that contains sensitive data, basic roles are probably too broad. 

Custom roles can only be applied to either the project level or organization level. They can’t be applied to the folder level.

What if you want to give permissions to a Compute Engine virtual machine, rather than to a person? That’s what service accounts are for. So, if a service account has been granted Compute Engine’s Instance Admin role, this would allow an application running in a VM with that service account to create, modify, and delete other Vms. Also, service accounts do need to be managed. 

It’s common to log in to the Google Cloud Console with a Gmail account and then use Google Groups to collaborate. With this setup, there’s no easy way to immediately remove a user’s access to the team’s cloud resources. With a tool called Cloud Identity, organizations can define policies and manage their users and groups using the Google Admin Console.
There are four ways to access and interact with Google Cloud:
* The Cloud Console – Google Cloud’s UI and helps deploy, scale, and diagnose production issues in a simple web-based interface. With the Cloud Console, you can easily find your resources, check their health, have full management control over them, and set budgets to control how much you spend on them.
* The Cloud SDK and Cloud Shell - The Cloud SDK is a set of tools that you can use to manage resources and applications hosted on Google Cloud. These include the Google Cloud CLI, which provides the main command-line interface for Google Cloud products and services, and bq, a command-line tool for BigQuery. Cloud Shell provides command-line access to cloud resources directly from a browser. Cloud Shell is a Debian-based virtual machine with a persistent 5 GB home directory, which makes it easy to manage Google Cloud projects and resources.
* The APIs - The Cloud Console includes a tool called the Google APIs Explorer that shows which APIs are available, and in which versions.
* the Google Cloud App – it can be used to start, stop, and use SSH to connect to Compute Engine instances and see logs from each instance. It also lets you stop and start Cloud SQL instances. Additionally, you can administer applications deployed on App Engine by viewing errors, rolling back deployments, and changing traffic splitting. The app also offers alerts and incident management.