THE MODEL
---------

![The maturity model for continuous delivery](http://bekkopen.github.io/maturity-model)

In the model, we use seven aspects or categories that we find to be essential to continuous delivery. They are process & organisation, technology, quality assurance, deployment routines, configuration management, and build & continuous integration (CI). For each of these aspects, we assess the organisation's maturity level. We use the levels big challenges, baseline, intermediate and advanced. The organisation should aim to move to a higher level to achieve continuous delivery.

HOW TO USE THE MODEL
--------------------

The first thing you need to establish is your current level of maturity within each category in the model. This will give you an idea of your strengths and weaknesses. Second, you need to prioritise. It is important to focus your efforts on the bottlenecks in your delivery process. To identify bottlenecks, it can be helpful to visualise your value stream and focus your attention on the steps that are most error prone or slow.

Prioritising which category to start with will vary. You will have to make your own assessment on which category will give the most value. You should try to keep the overall maturity level fairly even as most categories at the same level either depend on or complement each other. Furthermore, you should not skip levels or try to implement them all at once. As in any agile approach you should introduce changes in an incremental and iterative way.

PROCESS & ORGANISATION
----------------------

Organisations are different, and they all have a variety of processes. Yet there are some common organisation types that can be identified. Silo organisations are typically a bad idea. People that depend on one another's work are not co-located and don’t work together. This causes ineffective handoffs, less insight into the whole, misunderstandings and a blaming culture. No one can get their own work done before others have completed theirs. Since the silos “own” the stuff they are in charge of, they don’t let others touch it. When developers don’t have access to production logs they are unable to see what goes on in production, and troubleshooting becomes almost impossible.

When organisations begin to adopt agile, the communication with business improves and releases become more frequent. The boundaries between the fractions get blurred and for the sake of sanity the developers get access to production logs. Gradually the teams become more efficient, and they measure and seek ways to reduce cycle times between deployments. By always having their code production ready they can release at any given moment. With freedom the teams usually self-organise, given that they are cross-functional. Everyone understands that they all must work together to create the system. Developers and operations share common goals (DevOps) and everyone works on the system as a whole.

TECHNOLOGY
----------

The transformation must also be supported by the best technology. “Enterprise” infrastructure that promises to solve every problem and that only can be configured via a GUI just doesn’t cut it. One must choose each technology carefully and put together a stack that best suits your specific needs. Open source technologies are often easier to configure, easier to script, and a lot easier to understand (!). When your stack is put together in a “loose” fashion it is easy to replace one part with another when something better comes along.

QUALITY ASSURANCE
-----------------

To be able to shorten delivery time you have to ensure that quality assurance is built into the process itself in an automated way. Handing your code over to a test department or spending two days of testing each time you release becomes impossible. This doesn’t mean you should test less. The mantra of continuous delivery is to automate everything that can be automated, and all the different flavours of testing are obvious candidates for automation.

DEPLOYMENT ROUTINES
-------------------

Speeding up the cycle time from idea to production is what continuous delivery is all about. Nothing has any value unless it’s in production. Deployment shouldn’t be something you spend a lot of time focusing on. It should “just happen”, and it shouldn’t involve any risk. Automate both deploy and rollback, have a feature toggle safety net, and pay special attention to your database. When releasing often you should be able to deploy without downtime.

CONFIGURATION MANAGEMENT
------------------------

Having configuration scattered all around makes it hard to understand how your application works and makes it difficult to pinpoint the cause when trouble arises. Keep it in source control and in one place.

An application bug is not the only thing that can cause trouble in production, a badly configured infrastructure can do it just as easily. Therefore, you should treat your configuration as you would your code, put it in source control, and consider using a provisioning framework. Make sure you test your infrastructure and use the same configuration in all environments (dev, test, qa and prod).

BUILD & CI
----------

This category is closely related to the Quality Assurance, Deployment Routines and Configuration management categories. While the first provides the feedback, the second the deployment machinery, and the third the infrastructure, Build & CI puts it all together in a pipeline and provide feedback at every stage.

The most basic mechanisms merely runs tests every time code is checked in. A more advanced setup will have the feedback mechanisms triggered by any change in any environment, including code changes, deployments or configuration changes.

SUMMARY
-------

Continuous delivery is all about reducing risk and making sure business get their return on investment as soon as possible. It’s about removing focus from repetitive and risky tasks and devoting all you effort into delivering business value.

Hopefully you will find the maturity model valuable and useful in your own environment, and that it can help and inspire you to become better at obtaining your goals. Good luck!

