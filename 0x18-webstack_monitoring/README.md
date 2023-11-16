# 0x18. Webstack monitoring
## Concepts
* [Monitoring](monitoring.md)
* [Server](server.md)
![image](https://github.com/gillohsylvia/alx-system_engineering-devops/assets/104779232/2d1ec68a-bcb7-4829-a921-561cbbb1a339)

# Background Context
“You cannot fix or improve what you cannot measure” is a famous saying in the Tech industry. In the age of the data-ism, monitoring how our Software systems are doing is an important thing. In this project, we will implement one of many tools to measure what is going on our servers.

Web stack monitoring can be broken down into 2 categories:
* Application monitoring: getting data about your running software and making sure it is behaving as expected
* Server monitoring: getting data about your virtual or physical server and making sure they are not overloaded (could be CPU, memory, disk or network overload)

![image](https://github.com/gillohsylvia/alx-system_engineering-devops/assets/104779232/67240856-6be3-4019-939e-2346d658abb4)

# Resources
* [What is server monitoring](https://www.sumologic.com/glossary/server-monitoring/)
* [What is application monitoring](https://en.wikipedia.org/wiki/Application_performance_management)
* [System monitoring by Google](https://sre.google/sre-book/monitoring-distributed-systems/)
* [Nginx logging and monitoring](https://docs.nginx.com/nginx/admin-guide/monitoring/logging/)

# Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:
* Why is monitoring needed
* What are the 2 main area of monitoring
* What are access logs for a web server (such as Nginx)
* What are error logs for a web server (such as Nginx)

# Tasks
## 0. Sign up for Datadog and install datadog-agent
For this task head to https://www.datadoghq.com/ and sign up for a free `Datadog` account. When signing up, you’ll have the option of selecting statistics from your current stack that `Datadog` can monitor for you. Once you have an account set up, follow the instructions given on the website to install the `Datadog` agent.

![image](https://github.com/gillohsylvia/alx-system_engineering-devops/assets/104779232/a52a6595-b4d9-4e09-b215-acbe63786f16)

* Sign up for Datadog - Please make sure you are using the US website of Datagog (https://app.datadoghq.com)
* Use the US1 region
* Install `datadog-agent` on web-01
* Create an `application key`
* Copy-paste in your Intranet user profile (here) your DataDog API key and your DataDog application key.
* Your server web-01 should be visible in Datadog under the host name XX-web-01
  * You can validate it by using this [API](https://docs.datadoghq.com/api/latest/hosts/)
  * If needed, you will need to update the hostname of your server

#### Repo:
* GitHub repository: alx-system_engineering-devops
* Directory: 0x18-webstack_monitoring
     
## 1. Monitor some metrics
Among the litany of data your monitoring service can report to you are system metrics. You can use these metrics to determine statistics such as reads/writes per second, which can help your company determine if/how they should scale. Set up some `monitors` within the `Datadog` dashboard to monitor and alert you of a few. You can read about the various system metrics that you can monitor here: [System Check.](https://docs.datadoghq.com/integrations/system/)

![image](https://github.com/gillohsylvia/alx-system_engineering-devops/assets/104779232/a97d752c-5af0-4e9d-8e83-6e80f824dc28)

* Set up a monitor that checks the number of read requests issued to the device per second.
* Set up a monitor that checks the number of write requests issued to the device per second.
#### Repo:
* GitHub repository: alx-system_engineering-devops
* Directory: 0x18-webstack_monitoring
    
## 2. Create a dashboard
Now create a dashboard with different metrics displayed in order to get a few different visualizations.
* Create a new `dashboard`
* Add at least 4 `widgets` to your dashboard. They can be of any type and monitor whatever you’d like
* Create the answer file `2-setup_datadog` which has the `dashboard_id` on the first line. Note: in order to get the id of your dashboard, you may need to use [Datadog’s API](https://docs.datadoghq.com/api/latest/)

#### Repo:
* GitHub repository: alx-system_engineering-devops
* Directory: 0x18-webstack_monitoring
* File: 2-setup_datadog
    
Copyright © 2023 ALX, All rights reserved.
