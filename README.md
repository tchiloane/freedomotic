Freedomotic
=================================

Official website is http://freedomotic.com

Freedomotic is an open source, flexible, secure Internet of Things (IoT) application framework, useful to build and manage modern smart spaces. It is targeted to private individuals (home automation) as well as business users (smart retail environments, ambient aware marketing, monitoring and analytics, ...). Learn more at http://freedomotic.com

Freedomotic can run also on **Raspberry Pi** and can easily interact with DIY **Arduino** projects.

Starting from 2 Feb 2014, this is the freedomotic mainstream repository. Previous repository was hosted on googlecode http://code.google.com/p/freedomotic

Requirements: 
- **Java Open JDK** version 7 or oracle jdk _(to install on ubuntu: sudo apt-get install openjdk-7-jdk)_
- **Maven** version 2 or 3 _(to install on ubuntu: sudo apt-get install maven)_
- **Any OS** with java support _(Linux, Windows, Mac, Solaris ...)_

Development status:
- **Current released version**: 5.5.0 'Bender' (released on 24 Jan 2014)
- **Version in development (HEAD of this repository)**: 5.6.0 'Commander'


Developers Quick Start
======================

Follow this instructions if you want to compile freedomotic from source (eg: to develop your own plugins). If you just want to try it, just download the precompiled binaries you can find at the official download page http://freedomotic.com/content/download

**1) Fork freedomotic on GitHub**

* Create an account on https://github.com if you don't have one.
* **Fork Freedomotic** [_(What does it mean?)_](https://help.github.com/articles/fork-a-repo) following this link: <https://github.com/freedomotic/freedomotic/fork>. 
* Create the local clone of your online fork with this command:

```
git clone https://github.com/YOUR-GITHUB-USERNAME/freedomotic.git
```

Now the repository is ready to work with.

**2) Enter the new local folder**

    cd freedomotic
    
**3) Compile freedomotic with maven**

    mvn clean install
    
**4) IMPORTANT!!!! THIS IS REQUIRED: Copy the example-data folder into freedomotic-core/data.** If you miss this step freedomotic won't start

    cp -r data-example/ framework/freedomotic-core/data
    
**5) Run Freedomotic**

    java -jar framework/freedomotic-core/target/freedomotic-core/freedomotic.jar

As an alternative you can start **freedomotic-core** project from your favourite IDE. Here an example with NetBeans IDE http://freedomotic.com/content/faq-troubleshooting#Getting_started_with_netbeans
    
If you experience compile or startup errors please refer to [Faq & Troubleshooting](https://github.com/freedomotic/freedomotic/wiki/Faq-&-Troubleshooting)

Tools
======

- Issue Tracker: http://freedomotic.myjetbrains.com/youtrack/dashboard
- Continuuous Integration: http://teamcity.codebetter.com/project.html?projectId=Freedomotic
- Internationalization: https://www.transifex.com/projects/p/freedomotic-open-source-buildi/
- Wiki: https://github.com/freedomotic/freedomotic/wiki
- Source Code: https://github.com/freedomotic/freedomotic


Git reporitory is an SDK
========================

The GIT repository is a complete SDK with all you need to code and test your freedomotic plugins. Once compiled for the first time open the freedomotic-core project with your favourite IDE and start it to try freedomotic.

To develop your own plugin you can start from the "hello-world" example project included in GIT_ROOT/plugins/devices/hello-world. Open it in your IDE, make some changes and compile. It will be automatically installed into the freedomotic runtime (freedomotic-core project). Just start freedomotic-core to try your latest changes.

Try it on Raspberry Pi
======================
We have a script to do it automatically, follow this short tutorial http://freedomotic.com/content/install-freedomotic-raspberry-pi

Give feedback
=============

Please write on the forum http://freedomotic.com/content/forum or reach us by mail at info@freedomotic.com
