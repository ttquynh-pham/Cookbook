
Basic Data Engineering Skills
=============================

## Contents

- [Learn to Code](02-BasicSkills.md#learn-to-code)
- [Get Familiar with Git](02-BasicSkills.md#get-familiar-with-git)
- [Agile Development](02-BasicSkills.md#agile-development)
  - [Why Is Agile So Important?](02-BasicSkills.md#Why-is-agile-so-important)
  - [Agile Rules I Learned Over the Years](02-BasicSkills.md#agile-rules-i-learned-over-the-years)
  - [Agile Frameworks](02-BasicSkills.md#agile-frameworks)
    - [Scrum](02-BasicSkills.md#scrum)
    - [OKR](02-BasicSkills.md#okr)
- [Software Engineering Culture](02-BasicSkills.md#software-engineering-culture)
- [Learn How a Computer Works](02-BasicSkills.md#learn-how-a-computer-works)
- [Data Network Transmission](02-BasicSkills.md#data-network-transmission)
- [Security and Privacy](02-BasicSkills.md#security-and-privacy)
  - [SSL Public and Private Key Certificates](02-BasicSkills.md#ssl-public-and-private-key-Certificates)
  - [JSON Web Tokens](02-BasicSkills.md#json-web-tokens)
  - [GDPR Regulations](02-BasicSkills.md#gdpr-regulations)
- [Linux](02-BasicSkills.md#linux)
  - [OS Basics](02-BasicSkills.md#os-basics)
  - [Shell Scripting](02-BasicSkills.md#shell-scripting)
  - [Cron Jobs](02-BasicSkills.md#cron-jobs)
  - [Packet Management](02-BasicSkills.md#packet-management)
- [Docker](02-BasicSkills.md#docker)
  - [What Docker Is and How It Works](02-BasicSkills.md#what-is-docker-and-what-do-you-use-it-for)
    - [Don't Mess Up Your System](02-BasicSkills.md#dont-mess-up-your-system)
    - [Preconfigured Images](02-BasicSkills.md#preconfigured-images)
    - [Take It With You](02-BasicSkills.md#take-it-with-you)
    - [Kubernetes Container Deployment](02-BasicSkills.md#kubernetes-container-deployment)
    - [How to Create, Start, and Stop a Container](02-BasicSkills.md#how-to-create-start-stop-a-container)
    - [Docker Micro Services](02-BasicSkills.md#docker-micro-services)
    - [Kubernetes](02-BasicSkills.md#kubernetes)
    - [Why and How to Do Docker Container Orchestration](02-BasicSkills.md#why-and-how-to-do-docker-container-orchestration)
    - [Useful Docker Commands](02-BasicSkills.md#useful-docker-commands)
- [The Cloud](02-BasicSkills.md#the-cloud)
  - [IaaS vs. PaaS vs. SaaS](02-BasicSkills.md#iaas-vs-paas-vs-saas)
  - [AWS Azure IBM Google](02-BasicSkills.md#aws-azure-ibm-google)
  - [Cloud vs. On-Premises](02-BasicSkills.md#cloud-vs-on-premises)
  - [Security](02-BasicSkills.md#security)
  - [Hybrid Clouds](02-BasicSkills.md#hybrid-clouds)
- [Security Zone Design](02-BasicSkills.md#security-zone-design)
  - [How to Secure a Multi-:ayered Application](02-BasicSkills.md#how-to-secure-a-multi-layered-application)
  - [Cluster Security With Kerberos](02-BasicSkills.md#cluster-security-with-kerberos)



Learn to Code
-------------

Why this is important: Without coding you cannot do much in data
engineering. I cannot count the number of times I needed a quick Java
hack.

The possibilities are endless:

-   Writing or quickly getting some data out of a SQL DB.

-   Testing to produce messages to a Kafka topic.

-   Understanding the source code of a Java webservice.

-   Reading counter statistics out of a HBase key-value store.

So, which language do I recommend then?

I highly recommend Java. It's everywhere!

When you are getting into data processing with Spark, you should use
Scala. But, after learning Java, this is easy to do.

Also, Python is a great choice. It is super versatile.

Personally, however, I am not that big into Python. But, I am going to
look into it.

Where to learn? There's a Java course on Udemy you could look at:
<https://www.udemy.com/java-programming-tutorial-for-beginners>

-   Object-oriented programming (OOP).

-   What are unit tests to make sure what your code is working.

-   Functional programming.

-   How to use build management tools like Maven.

-   Resilience testing (?).

I talked about the importance of learning by doing in this podcast:
<https://anchor.fm/andreaskayy/episodes/Learning-By-Doing-Is-The-Best-Thing-Ever---PoDS-035-e25g44>

Get Familiar with Git
---------------------

Why this is important: One of the major problems with coding is to keep
track of changes. It is also almost impossible to maintain a program you
have multiple versions of.

Another problem is the topic of collaboration and documentation, which
is super important.

Let's say you work on a Spark application and your colleagues need to
make changes while you are on holiday. Without some code management, they
are in huge trouble:

Where is the code? What have you changed last? Where is the
documentation? How do we mark what we have changed?

But, if you put your code on GitHub, your colleagues can find your code.
They can understand it through your documentation (please also have
in-line comments).

Developers can pull your code, make a new branch, and do the changes.
After your holiday, you can inspect what they have done and merge it with
your original code, and you end up having only one application.

Where to learn: Check out the GitHub Guides page where you can learn all
the basics: <https://guides.github.com/introduction/flow/>

This great GitHub commands cheat sheet saved my butt multiple times:
<https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet>

Also look into:

-   Pull

-   Push

-   Branching

-   Forking

GitHub uses markdown to write pages, a super simple language that is actually a lot of fun to write. Here's a markdown cheat cheatsheet:
<https://www.markdownguide.org/cheat-sheet/>

Pandoc is a great tool to convert any text file to and from markdown:
<https://pandoc.org>


Agile Development
-----------------

Agility is the ability to adapt quickly to changing circumstances.

These days, everyone wants to be agile. Big and small companies are
looking for the "startup mentality."

Many think it's the corporate culture. Others think it's the process of how
we create things that matters.

In this article, I am going to talk about agility and self-reliance,
about how you can incorporate agility in your professional career.

### Why Is Agile So Important?

Historically, development has been practiced as an explicitly defined process. You
think of something, specify it, have it developed, and then build in mass
production.

It's a bit of an arrogant process. You assume that you already know
exactly what a customer wants, or how a product has to look and how
everything works out.

The problem is that the world does not work this way!

Oftentimes the circumstances change because of internal factors.

Sometimes things just do not work out as planned or stuff is harder than
you think.

You need to adapt.

Other times you find out that you built something customers do not like
and needs to be changed.

You need to adapt.

That's why people jump on the Scrum train -- because Scrum is the
definition of agile development, right?

### Agile Rules I Learned Over the Years

#### Is the Method Making a Difference?

Yes, Scrum or Google's OKR can help to be more agile. The secret to
being agile, however, is not only how you create.

What makes me cringe is people trying to tell you that being agile
starts in your head. So, the problem is you?

No!

The biggest lesson I have learned over the past years is this: Agility
goes down the drain when you outsource work.

#### The Problem with Outsourcing

I know on paper outsourcing seems like a no-brainer: development costs
against the fixed costs.

It is expensive to bind existing resources on a task. It is even more
expensive if you need to hire new employees.

The problem with outsourcing is that you pay someone to build stuff for
you.

It does not matter who you pay to do something for you. He needs to make
money.

His agenda will be to spend as little time as possible on your work. That
is why outsourcing requires contracts, detailed specifications,
timetables, and delivery dates.

He doesn't want to spend additional time on a project, only because you
want changes in the middle. Every unplanned change costs him time and
therefore money.

If so, you need to make another detailed specification and a contract
change.

He is not going to put his mind into improving the product while
developing. Firstly, because he does not have the big picture. Secondly,
because he does not want to.

He is doing as he is told.

Who can blame him? If I were the subcontractor, I would do exactly the
same!

Does this sound agile to you?

#### Knowledge Is King: A lesson from Elon Musk

Doing everything in house -- that's why startups are so productive. No
time is wasted on waiting for someone else.

If something does not work or needs to be changed, there is someone on
the team who can do it right away.

One very prominent example who follows this strategy is Elon Musk.

Tesla's Gigafactories are designed to get raw materials in on one side
and spit out cars on the other. Why do you think Tesla is building
Gigafactories that cost a lot of money?

Why is SpaceX building its own space engines? Clearly, there are other,
older companies who could do that for them.

Why is Elon building tunnel boring machines at his new boring company?

At first glance, this makes no sense!

#### How You Really Can Be Agile

If you look closer, it all comes down to control and knowledge. You, your
team, your company, needs to do as much as possible on your own.
Self-reliance is king.

Build up your knowledge and therefore the team's knowledge. When you have
the ability to do everything yourself, you are in full control.

You can build electric cars, build rocket engines, or bore tunnels.

Don't largely rely on others, and be confident to just do stuff on your
own.

Dream big, and JUST DO IT!

PS. Don't get me wrong. You can still outsource work. Just do it in a
smart way by outsourcing small independent parts.

### Agile Frameworks

#### Scrum

There's an interesting Medium article with a lot of details
about Scrum: <https://medium.com/serious-scrum>

Also, this Scrum guide webpage has good info:
<https://www.scrumguides.org/scrum-guide.html>

#### OKR

I personally love OKR and have been using it for years. Especially for smaller
teams, OKR is great. You don't have a lot of overhead and get work done.
It helps you stay focused and look at the bigger picture.

I recommend doing a sync meeting every Monday. There you talk about what
happened last week and what you are going to work on this week.

I talked about this in this podcast:
<https://anchor.fm/andreaskayy/embed/episodes/Agile-Development-Is-Important-But-Please-Dont-Do-Scrum--PoDS-041-e2e2j4>

There is also this awesome 1,5-hour startup guide from Google:
<https://youtu.be/mJB83EZtAjc> I really love this video; I rewatched it
multiple times.

### Software Engineering Culture

The software engineering and development culture is super important. How
does a company handle product development with hundreds of developers?
Check out this podcast:

| Podcast episode: #070 Engineering Culture At Spotify
|------------------
|In this podcast, we look at the engineering culture at Spotify, my favorite music streaming service. The process behind the development of Spotify is really awesome.
  |[Watch on YouTube](https://youtu.be/1asVrsUDbp0) \ [Listen on Anchor](https://anchor.fm/andreaskayy/episodes/070-The-Engineering-Culture-At-Spotify-e45ipa)|


**Some interesting slides:**

<https://labs.spotify.com/2014/03/27/spotify-engineering-culture-part-1/>

<https://labs.spotify.com/2014/09/20/spotify-engineering-culture-part-2/>

Learn How a Computer Works
--------------------------

### CPU,RAM,GPU,HDD

### Differences Between PCs and Servers

I talked about computer hardware and GPU processing in this podcast:
<https://anchor.fm/andreaskayy/embed/episodes/Why-the-hardware-and-the-GPU-is-super-important--PoDS-030-e23rig>

Data Network Transmission
---------------------------------------

### OSI Model

The OSI Model describes how data flows through the network. It
consists of layers starting from physical layers, basically how the data
is transmitted over the line or optic fiber.

Check out this article for a deeper understanding of the layers and processes outlined in the OSI model:
<https://www.studytonight.com/computer-networks/complete-osi-model>

The Wikipedia page is also very good:
<https://en.wikipedia.org/wiki/OSI_model>

###### Which Protocol Lives on Which Layer?

Check out this network protocol map. Unfortunately, it is really hard to
find it theses days:
<https://www.blackmagicboxes.com/wp-content/uploads/2016/12/Network-Protocols-Map-Poster.jpg>

### IP Subnetting

Check out this IP address and subnet guide from Cisco:
<https://www.cisco.com/c/en/us/support/docs/ip/routing-information-protocol-rip/13788-3.html>

A calculator for subnets:
<https://www.calculator.net/ip-subnet-calculator.html>

### Switch, Layer-3 Switch

For an introduction to how ethernet went from broadcasts, to bridges, to
Ethernet MAC switching, to ethernet & IP (layer 3) switching, to
software-defined networking, and to programmable data planes that can
switch on any packet field and perform complex packet processing, see
this video: <https://youtu.be/E0zt_ZdnTcM?t=144>

### Router

### Firewalls

I talked about network infrastructure and techniques in this podcast:
<https://anchor.fm/andreaskayy/embed/episodes/IT-Networking-Infrastructure-and-Linux-031-PoDS-e242bh>

Security and Privacy
--------------------

### SSL Public and Private Key Certificates

### What Is a Certificate Authority

### JSON Web Tokens

Link to the Wiki page: <https://en.wikipedia.org/wiki/JSON_Web_Token>

### GDPR Regulations

The EU created the GDPR \"General Data Protection Regulation\" to
protect your personal data like: name, age, address, and so
on.

It's huge and quite complicated. If you want to do online business in
the EU, you need to apply these rules. The GDPR is applicable since May
25th, 2018. So, if you haven't looked into it, now is the time.

The penalties can be crazy high if you make mistakes here.

Check out the full GDPR regulation here: <https://gdpr-info.eu>

By the way, if you do profiling or analyse big data in general, look
into it. There are some important regulations, unfortunately.

I spend months with GDPR compliance. Super fun. Not! Hahaha

### Privacy by Design

When should you look into privacy regulations and solutions?

Creating the product or service first and then bolting on the privacy is
a bad choice. The best way is to start implementing privacy right away
in the engineering phase.

This is called privacy by design. Privacy is an integral part of your
business, not just something optional.

Check out the Wikipedia page to get a feeling for the important
principles: <https://en.wikipedia.org/wiki/Privacy_by_design>

Linux
-----

Linux is very important to learn, at least the basics. Most big-data
tools or NoSQL databases run on Linux.

From time to time, you need to modify stuff through the operating system,
especially if you run an infrastructure as a service solution like
Cloudera CDH, Hortonworks, or a MapR Hadoop distribution.

### OS Basics

Show all historic commands:

    history | grep docker

### Shell scripting

Ah, creating shell scripts in 2019? Believe it or not, scripting in the
command line is still important.

Start a process, automatically rename, move or do a quick compaction of
log files. It still makes a lot of sense.

Check out this cheat sheet to get started with scripting in Linux:
<https://devhints.io/bash>

There's also this Medium article with a super-simple example for
beginners:
<https://medium.com/@saswat.sipun/shell-scripting-cheat-sheet-c0ecfb80391>

### Cron Jobs

Cron jobs are super important to automate simple processes or jobs in
Linux. You need this here and there, I promise. Check out these three
guides:

<https://linuxconfig.org/linux-crontab-reference-guide>

<https://www.ostechnix.com/a-beginners-guide-to-cron-jobs/>

And, of course, Wikipedia, which is surprisingly good:
<https://en.wikipedia.org/wiki/Cron>

Pro tip: Don't forget to end your cron files with an empty line or a
comment, otherwise it will not work.

### Packet Management

Linux tips are the second part of this podcast:
<https://anchor.fm/andreaskayy/embed/episodes/IT-Networking-Infrastructure-and-Linux-031-PoDS-e242bh>


Docker
------

### What is Docker, and What Do You Use It for?

Have you played around with Docker yet? If you're a data science learner
or a data scientist, you need to check it out!

It's awesome because it simplifies the way you can set up development
environments for data science. If you want to set up a dev environment,
you usually have to install a lot of packages and tools.

#### Don't Mess Up Your System

What this does is basically mess up your operating system. If you're
just starting out, you don't know which packages you need to install. You don't
know which tools you need to install.

If you want to, for instance, start with Jupyter Notebooks, you need to
install that on your PC somehow. Or, you need to start installing tools
like PyCharm or Anaconda.

All that gets added to your system, and so you mess up your system more
and more and more. What Docker brings you, especially if you're on a Mac
or a Linux system, is simplicity.

#### Preconfigured Images

Because it is so easy to install on those systems, another cool thing
about Docker images is you can just search them in the Docker store,
download them, and install them on your system.

Running them in a completely pre-configured environment, you don't need
to think about stuff. You go to the Docker library, and you search for Deep
Learning, GPU and Python.

You get a list of images you can download. You download one, start it
up, go to the browser and hit up the URL, and just start coding.

Start doing the work. The only other thing you need to do is bind some
drives to that instance so you can exchange files. And, then that's it!

There is no way that you can crash or mess up your system. It's all
encapsulated into Docker. Why this works is because Docker has native
access to your hardware.

#### Take It With You

It's not a completely virtualized environment like a VirtualBox. An
image has the upside that you can take it wherever you want. So, if
you're on your PC at home, use that there.

Make a quick build, take the image, and go somewhere else. Install the
image, which is usually quite fast, and just use it like you're at home.

It's that awesome!

### Kubernetes Container Deployment

I am getting into Docker a lot more myself. For a some different reasons.

What I'm looking for is using Docker with Kubernetes. With Kubernetes,
you can automate the whole container deployment process.

The idea is that you have a cluster of machines. Lets say you have
a 10-server cluster and you run Kubernetes on it.

Kubernetes lets you spin up Docker containers on demand to execute
tasks. You can set up how much resources like CPU, RAM, and network your
Docker container can use.

You can basically spin up containers, on the cluster on demand, whenever
you need to do an analytics task.

That's perfect for data science.

### How to Create, Start, Stop a Container

### Docker Micro-Services?

### Kubernetes

### Why and How to Do Docker Container Orchestration

Podcast about how data science learners use Docker (for data
scientists):
<https://anchor.fm/andreaskayy/embed/episodes/Learn-Data-Science-Go-Docker-e10n7u>

### Useful Docker Commands

Create a container:

    docker run CONTAINER --network NETWORK

Start a stopped container:

    docker start CONTAINER NAME

Stop a running container:

    docker stop

List all running containers:

    docker ps

List all containers including stopped ones:

    docker ps -a

Inspect the container configuration (e.g. network settings, etc.):

    docker inspect CONTAINER

List all available virtual networks:

    docker network ls

Create a new network:

    docker network create NETWORK --driver bridge

Connect a running container to a network:

    docker network connect NETWORK CONTAINER

Disconnect a running container from a network:

    docker network disconnect NETWORK CONTAINER

Remove a network:

    docker network rm NETWORK


The Cloud
---------

### IaaS vs. PaaS vs. SaaS

Check out this podcast. It will help you understand the
difference and how to decide what to use.

| Podcast episode: #082 Reading Tweets With Apache Niﬁ & IaaS vs PaaS vs SaaS
|------------------|
|In this episode, we talk about the differences between infrastructure as a service, platform as a service, and application as a service. Then, we install the Niﬁ Docker container and look into how we can extract the twitter data.
| [Watch on YouTube](https://youtu.be/pWuT4UAocUY) \ [Listen on Anchor](https://anchor.fm/andreaskayy/episodes/082-Reading-Tweets-With-Apache-Nifi--IaaS-vs-PaaS-vs-SaaS-e45j50)|


### AWS, Azure, IBM, Google

Each of these have their own answer to IaaS, Paas, and SaaS. Pricing and
pricing models vary greatly between each provider. Likewise, each
provider's service may have limitations and strengths.

#### AWS

Here is the [full list of AWS services](https://www.amazonaws.cn/en/products/). Studying for the [AWS Certified Cloud Practitioner](https://aws.amazon.com/certification/certified-cloud-practitioner/?ch=cta&cta=header&p=2) and/or [AWS Certified Solutions Architect](https://aws.amazon.com/certification/certified-solutions-architect-associate/?ch=sec&sec=rmg&d=1) exams can be helpful to quickly gain an understanding of all these services. 
Here are links for free digital training for the [AWS Certified Cloud Practitioner](https://explore.skillbuilder.aws/learn/public/learning_plan/view/82/cloud-foundations-learning-plan) and [AWS Certified Solutions Architect Associate](https://explore.skillbuilder.aws/learn/public/learning_plan/view/78/architect-learning-plan).

Here is a free 17 hour [Data Analytics Learning plan](https://explore.skillbuilder.aws/learn/public/learning_plan/view/97/data-analytics-learning-plan) for AWS's [Analytics](https://aws.amazon.com/big-data/datalakes-and-analytics/?nc2=h_ql_prod_an)/Data Engineering services.

#### Azure
[Full list of Azure services](https://azure.microsoft.com/en-us/services/).
[Get started with mini courses](https://docs.microsoft.com/en-us/learn/browse/).

#### IBM

#### Google

Google Cloud Platform offers a wide, ever-evolving variety of services.
[List of GCP services with brief description](https://github.com/gregsramblings/google-cloud-4-words). In
recent years, documentation and tutorials have com a long way to help
[getting started with
GCP](https://cloud.google.com/gcp/getting-started/). You can start with
a free account, but to use many of the services, you will need to turn on
billing. Once you do enable billing, always remember to turn off services
that you have spun up for learning purposes. It is also a good idea to
turn on billing limits and alerts.

### Cloud vs. On-Premises

| Podcast episode: #076 Cloud vs. On-Premise
|------------------|
|How to choose between cloud and on-premises, pros and cons and what you have to think about. There are good reasons to not go cloud. Also, thoughts on how to choose between the cloud providers by just comparing instance prices. Otherwise, the comparison will drive you insane. My suggestion: Basically use them as IaaS and something like Cloudera as PaaS. Then build your solution on top of that.  
| [Watch on YouTube](https://youtu.be/BAzj0yGcrnE) \ [Listen on Anchor](https://anchor.fm/andreaskayy/episodes/076-Cloud-vs-On-Premise-How-To-Decide-e45ivk)|


### Security

Listen to a few thoughts about the cloud in this podcast:
<https://anchor.fm/andreaskayy/embed/episodes/Dont-Be-Arrogant-The-Cloud-is-Safer-Then-Your-On-Premise-e16k9s>

### Hybrid Clouds

Hybrid clouds are a mixture of on-premises and cloud deployment. A very
interesting example for this is Google Anthos:

<https://cloud.google.com/anthos/>

Security Zone Design
--------------------

### How to Secure a Multi-Layered Application

(UI in different zone than SQL DB)

### Cluster Security With Kerberos

I talked about security zone design and lambda architecture in this
podcast:
<https://anchor.fm/andreaskayy/embed/episodes/How-to-Design-Security-Zones-and-Lambda-Architecture--PoDS-032-e248q2>
