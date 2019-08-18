GSoC submission 2019 
===================

### GSoC-2019---EAT---JBoss-Community

Link to the work done on the project: [Project2ndChance](https://github.com/Lkop/Project2ndChance), [Project2ndChanceAT](https://github.com/Lkop/Project2ndChanceAT)


Link to the workshop: [EAT_workshop ](https://www.dropbox.com/s/bebhyd1iz7cg1i2/EAT_WORKSHOP.odt?dl=0)

Link to project proposal: [EAT](https://summerofcode.withgoogle.com/projects/#5914339578478592)

----------

Introduction
-------------

Our project, which is included in the category of Software Testing, is related to EAT(EAP Additional Testsuite) with which we can test infinite software project versions. 


#### The advantages of EAT are :

1. Writing the tests once and testing against infinite number of Application Servers.
2. Having all the tests at one place.
3. Comparison of the servers based on the testsuite.
4. Guarding against regression.
5. Faster convergence among the servers.
6. Comparison of the servers based on tests of the past and the present.
7. Addition of tests with possible future features that are not at the moment available.
8. It makes possible to push a testcase of a fix regarding a specific component of the server, without the component version to have been updated at the server pom.
9. Ability to merge tests from remote testsuites.


#### This GSoC 2019 Project had three goals :

1. Going through the EAT workshop lab : [EAT_workshop ](https://www.dropbox.com/s/bebhyd1iz7cg1i2/EAT_WORKSHOP.odt?dl=0) .
2. Adding the latest release of Wildfly (at the time) in EAT and using OpenShift.
3. Use the generalized AT structure to create an AT (Additional Testsuite) for a multi-versioned project.


GSoC 2019 RESULT / PRODUCTION
------------------------------

#### Phase 1

During the 1st phase I went through the workshop lab. 

Among the tasks was downloading and building the sources of different JBoss servers and JBoss server versions such as [Wildfly](https://github.com/wildfly/wildfly), [Wildfly 17.0.0](https://github.com/wildfly/wildfly/releases/tag/17.0.0.Final) and testing them using [EAT](https://github.com/jboss-set/eap-additional-testsuite). 

Below, there is a url link which contains screenshots of the EAT runs for all the servers / server versions done during this phase :
[Phase-1 Screenshots](https://www.dropbox.com/sh/dphkoqquhkob97o/AAD9UE9ru8-Wt6Iz-_Vytm_Ea/Build%20Screenshots)

During this phase I have added the latest release (at the time) of Wildfly server in EAT, creating a new test set, which was used with the EAT Travis CI build on Github.  Here is the PR that was merged : [EAT PR 1](https://github.com/jboss-set/eap-additional-testsuite/pull/82), [EAT PR 2](https://github.com/jboss-set/eap-additional-testsuite/pull/86), [EAT PR 3](https://github.com/jboss-set/eap-additional-testsuite/pull/87) and here is the latest successful [Travis CI build](https://travis-ci.org/jboss-set/eap-additional-testsuite/builds/544100495).

This work was tracked by the following Jira : [GSoC-2019 : Adding latest Wildfly Release 17.0.0.Final in EAT](https://issues.jboss.org/browse/WFLY-12178)

Also, during this phase, I have tested different versions of the [JBoss-Threads](https://github.com/jbossas/jboss-threads) component using JBTAT - JBoss Threads Additional Testsuite ( [JBTAT screenshots 1](https://www.dropbox.com/sh/dphkoqquhkob97o/AAAE-ORHG3ZJz8cwoq34SZNOa/Build%20Screenshots/success-JBTAT-999-SNAPSHOT-15-6-2019.png?dl=0), [JBTAT screenshots 2](https://www.dropbox.com/sh/dphkoqquhkob97o/AAB47M_0wO7yxNdOiKBEFYk3a/Build%20Screenshots/success-JBTAT-TESTS-999-SNAPSHOT-19-6-2019.png?dl=0) ).



#### Phase 2

During this phase, I went through some openshift tutorials and I tested an example image on [RedHat's OpenShift](https://www.openshift.com/) ( [OpenShift screenshots](https://www.dropbox.com/sh/dphkoqquhkob97o/AABNCx9ig99qpTaeguSnwXeqa/openshift-example) ).

I have also started creating [Project2ndChance](https://github.com/Lkop/Project2ndChance) and [Project2ndChanceAT](https://github.com/Lkop/Project2ndChanceAT) described in the next phase.



#### Phase 3

During the 3rd phase, I have continued the AT Structured Project called Project2ndChance (libs, API) and Project2ndChanceAT (tests). The main purpose of the project is the creation of an Additional Testsuite that can be applied in many versions of the Project2ndChance API, in order to check and improve many features of it.

The Additional Testsuite (Project2ndChanceAT) for the Project2ndChance tests different versions of Project2ndChance of different branches such as 1.0.0, 2.0.0, 2.1.1 .

Here are the URLs of the project:
* [Project2ndChance](https://github.com/Lkop/Project2ndChance)
* [Project2ndChanceAT](https://github.com/Lkop/Project2ndChanceAT)

The documentation of this project can be found in the README<span></span>.md file of the Project2ndChance github repository : [Project2ndChance Documentation](https://github.com/Lkop/Project2ndChance/blob/master/README.md)
