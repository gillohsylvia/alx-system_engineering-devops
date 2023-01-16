# 0x15. API
Old-school system administrators usually only know Bash and that is what they use to build their scripts. While Bash is perfectly fine for a lot of things, it can quickly get messy and not efficient compared to other programming languages. The new generation of system administrators, usually called SREs, are pretty much regular software engineers but instead of building products, they are managing systems. And one of the big differences with their predecessors is that they know more than just Bash scripting.

One popular way to expose an application and dataset is to use an API. Often, they are the public facing part of websites and micro-services so that allow outsiders to interact with them – access and modify their data. In this project, you will access employee data via an API to organize and export them to different data structures.

This is a perfect example of a task that is not suited for Bash scripting, so let’s build Python scripts.
## Learning Objectives
+ What Bash scripting should not be used for
+ What is an API
+ What is a REST API
+ What are microservices
+ What is the CSV format
+ What is the JSON format
+ Pythonic Package and module name style
+ Pythonic Class name style
+ Pythonic Variable name style
+ Pythonic Function name style
+ Pythonic Constant name style
+ Significance of CapWords or CamelCase in Python
## Resources
+ The GET Request https://realpython.com/python-requests/#the-get-request
+ Requests: HTTP for Humans https://docs.python-requests.org/en/latest/
+ API vs REST API Simplified: 6 Critical Differences  https://hevodata.com/learn/api-vs-rest-api/
+ REST, SOAP, GraphQL – Basics & Differences Between APIs https://www.techtic.com/blog/comprehensive-guide-to-soap-rest-graphql-web-protocols/
+ Names and Python Syntax https://www.cs.williams.edu/~jannen/teaching/f16/cs135/lectures/lecture.27.pdf
+ Friends don’t let friends program in shell script https://www.turnkeylinux.org/blog/friends-dont-let-friends-program-shell-script
+ What is an API https://www.webopedia.com/definitions/api/
+ What is an API? In English, please https://www.freecodecamp.org/news/what-is-an-api-in-english-please-b880a3214a82/
+ What is a REST API https://www.sitepoint.com/rest-api/
+ What are microservices https://smartbear.com/solutions/microservices/
+ PEP8 Python style - having a clean code respecting style guide is really appreciated in the industry https://peps.python.org/pep-0008/