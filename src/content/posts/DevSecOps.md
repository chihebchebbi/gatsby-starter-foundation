---
template: blog-post
slug: /DevSecOps
date: 2022-03-19T05:53:16.102Z
title: "DevSecOps: How to integrate Security into the DevOps Process"
featuredImage: /assets/Digi-Tech.jpeg
---

## Overview
I had the honor yes of attending the TEK-UP DIGITECH CONFERENCE in Istanbul, 
Where I got the chance to expound on the DevSecOps topic, How to integrate Security in the DevOps Process.

To understand DevSecOps, let’s look at a common DevOps flow where things are automated and fast. 
So the developers check in the code and an application delivery pipeline starts.

The changes are tested with automated tests, and any version is built and deployed an automated test will run.
And when everything is fine, the new version has to be released.
So this super optimized flow makes application delivery fast without manual effort from developers or testers.
And the new version of the application is ready to be released in production.

![Royal Mail](/assets/Pipeline.png "Pipline CI/CD")

In fact, not really, because what about security?
If your application is an online banking app or a social media platform that millions of people use, or other sensitive personal data.
you want to make sure that there are no security holes in your application, because getting hacked and leaking sensitive data of your users
may be detrimental to your business.
So before deploying it to production, the security team must test the new version for any vulnerabilities and other security issues.
What if the developers used a new library that has some vulnerabilities?
What if passwords are exposed? or container image has security issues?
or the Kubernetes components for the application are misconfigured?

![Royal Mail](/assets/Security Tests.png "Security Tests")

And of course, these could be things that developers themselves aren’t even aware of. 
So the security team will run tests and analyze the code and look
for any security issues in the application. And this may take hours or days.
Or if you have a complex application, maybe even weeks
So you see the problem here, that security audit takes so long time?
because platforms nowadays consume many microservices
and they expose APIs to communicate, which means much more attack surface. 
and On top of that, we have tons of services that microservices use like databases, message brokers, Mesh applications,
and now this may all run in containers, which is another layer where security issues may arise, And all these may run on a
cloud platform, maybe on a Kubernetes cluster.

![Royal Mail](/assets/Security Weakness.png "Security Risks")

So you see that we have many layers of infrastructure and application
and many components which need securing. And the security teams themselves need to also learn and understand all these platforms and technologies to be able to identify the issues.
So how to fix the problem?
The answer is by integrating security in the DevOps,
So instead of thinking about security as a separate task start thinking about security at the beginning and solve it right away as soon as security issues appear.

So the question here how would that work in practice?
And how can security be infused or integrated into this DevOps process?
first of all, security becomes a developer’s responsibility too, instead of just being a responsibility of dedicated professionals.
And the security team itself becomes more of an advisor to developers and operations teams, helping them to understand and
manage security rather than being like external police that blocks the development speed.

![Royal Mail](/assets/DevSecOps in Practice.png "DevSecOps in Practice")

So the security team will create security policies. Then they will create or select proper automation tools and platforms for detecting and identifying any security issues and vulnerabilities.
And this could be security scans, code quality checks, automated security tests of the application, etc.
And they will train and teach developers and operations team how to interpret the output of these tools so that they can identify and fix the issues themselves.
