Entwurf von Softwaresystemen  
Christoph Krenn  
1017553  

Proseminar sheet 9
==================

Exercise 3
----------

###Continous Integration

####General Idea

The idea behind Continous Integration (CI) is to integrate code into a shared  
repository several times a day to locate errors easier and more quickly.  
Further benefits of such a technique are shorter integrations, less time  
requirements for debugging, an increase of visibility which leads to better  
comminucation and more opportunities to test if your code is working.

####Practices

CI uses different practices, like maintaining a single source repository,  
automate the build, make your build self-testing and keep it fast, automate  
deployment and many more. 

####How it is done

It is done by checking out code into their private workspaces. When  
done, the commit changes to the repository. After that, the CI server does a bunch  
of tasks, like monitoring the repository and checking out changes when they occur  
and building the system and running unit and integration tests. If the build or  
tests fail, the CI server alerts the team which then fix the problem at the earliest  
opportunity. Repeat continually integrating and testing throughout the project.  
Team responsibilities are to frequently check in, don't go home after checking in  
until the system builds and so on. Many teams even develop rituals around these  
policies, meaning the teams effectively manages themselves. 

####Benefits

Wrapping the last lines up, the intended benefits should be to avoid last-minute  
chaos at release dates, a constant availability of a "current" build for testing,  
demo, or release purposes. Additionally, frequent code check-in pushes developers  
to create modular, less complex code.

####Drawbacks

There are certain scenarios where CI can be pricy: e.g. if your build or tests take  
a long time. Also, constructing an automated test suite requires a considerable  
amount of work, including ongoing effort to cover new features and follow intentional  
code modifications. CI can be performed without any test suite, but the cost of  
quality assurance to produce a releasable product can be high if it must be done  
manually and frequently.

####Sources
* [thoughtworks.com]  
*http://www.thoughtworks.com/continuous-integration*

* [Wikipedia english]  
*http://en.wikipedia.org/wiki/Continuous_integration*

* [Wikipedia german]  
*http://de.wikipedia.org/wiki/Kontinuierliche_Integration*
