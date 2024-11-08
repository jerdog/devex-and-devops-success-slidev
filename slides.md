---
titleTemplate: "%s - Slidev"
title: "Developer Experience is Central to DevOps Success"
theme: slidev-theme-the-unnamed
info: |
  ## Developer Experience is Central to DevOps Success

  ## Abstract
  Developer Experience (DevEx) encompasses every aspect of the experience that your developers (both internal and external) have with your product, tooling, systems, etc. While platform engineering aims to reduce developer toil, DevEx goes beyond that. It covers deployment pipelines, Infrastructure as Code (IaC) practices, developer efficiencies, productivity, UI/UX, and APIs. In this presentation, we will focus on some of the principles of DevOps (collaboration, communication, shared responsibility), go into the history of DevEx and how it's changed over the years (remember Vim? CFEngine?), and how a strong DevEx mindset can bring together development and operations teams.
author: Jeremy Meiss
conference: ""
socialimg: '../images/bluesky-jerdog-white.png'
keywords: devex,developer experience,devops
presenter: true
download: true
exportFilename: devex-central-devops-success-slidevExport
export:
  format: pdf
  timeout: 30000
  dark: false
  withClicks: false
  withToc: false
remoteAssets: true
selectable: true
record: true
wakeLock: build
mdc: true
colorSchema: auto
aspectRatio: 16/9
favicon: 'https://raw.githubusercontent.com/jerdog/jmeiss-me-website/main/assets/images/fav.png'
fonts:
  sans: Roboto
  serif: Roboto Slab
  mono: Fira Code
defaults:
  layout: center
layout: cover
---

# Developer Experience...

## Central to DevOps Success

<!-- A quick note that most of the images have been autogenerated by AI - which would explain some of the weird shapes and colors in the images. -->

---

# What is "Developer Experience" (DevEx)?

<!--
We've all had that experience using a tool or service that was a disaster. It could be the worst deployment process you've ever seen, or the most painful codebase you've ever had to work with, or documentation that's so confusing it makes your head spin. Or maybe a combination of them… Who here knows what I’m talking about? 

We’ve all seen examples of epicly bad websites, right? 
-->

---
layout: image
image: /images/slides/yale-art-school.jpg
backgroundSize: contain
---

<!--
Here’s an epicly bad website (as of 31-Oct-2024) from none other than the Yale School of Art. So much wrong on one page.
-->

---

```bash
git push heroku main
```

![Heroku deploy button](/images/slides/heroku-deploy-button.png)

<!--
Heroku was long considered the gold standard for developer experience with a simple set of tools and a command-line interface that allowed developers to focus on building applications and delivering them to users. And that was it. Now of course, Heroku is still around (albeit not nearly as developer-centric as they formerly were, but that is changing), but it's not the only game in town. Anyone used Netlify, Vercel, etc.? 
-->

---

## A working definition of DevEx
  
>_"...the **journey** of developers and practitioners as they learn and deploy technology, which if successful, focuses on eliminating obstacles that hinder them from achieving success in their endeavors."_

-**Jessica West**, _Co-Founder, DevEx Institute_

<!--
Let's start with a definition of DevEx - DevEx is the journey of developers as they learn and deploy technology. When successful, it focuses on eliminating obstacles that hinder a developer or practitioner from achieving success in their endeavors.
-->

---
layout: image-left
image: "/images/slides/cornell-devex.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

## DevEx isn't new

_REF: F. Fagerholm and J. Münch, "[Developer experience: Concept and definition](https://ieeexplore.ieee.org/document/6225984?arnumber=6225984)," 2012 International Conference on Software and System Process (ICSSP), Zurich, Switzerland, 2012._

<!--
But DevEx isn't a new thing. The first mention of "developer experience" as a concept was in a paper was presented at the June IEEE 2012 International Conference on Software and System Process in Zurich. There are references in the paper going back to 1985 that deal with "programmer performance and the effects of the workplace." A few things stand out in this paper, which is a really great read.
-->

---
layout: image-left
image: /images/slides/cornell-devex.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
---

## DevEx isn't new

>"New ways of working such as globally distributed development or the integration of self-motivated external developers into software ecosystems will require a better and more comprehensive understanding of developers' feelings, perceptions, motivations and identification with their tasks in their respective project environments."

_REF: F. Fagerholm and J. Münch, "[Developer experience: Concept and definition](https://ieeexplore.ieee.org/document/6225984?arnumber=6225984). 2012."_

---
layout: image-left
image: /images/slides/cornell-devex.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
transition: slide-up
---

## DevEx isn't new

>"...developer experience could be defined as a means for capturing how developers think and feel about their activities within their working environments, with the assumption that an improvement of the developer experience has positive impacts on characteristics such as sustained team and project performance."

_REF: F. Fagerholm and J. Münch, "[Developer experience: Concept and definition](https://ieeexplore.ieee.org/document/6225984?arnumber=6225984). 2012."_

<!--
The second was this line, that DevEx could be a means for capturing how devs think and feel about their activities at work, and that improving their experience impacts things like sustained team and project performance.

So all of this interest in DevEx isn't a new concept - but is largely driven by companies trying to sell you something, from the top down, with very little (if any) focus on developers themselves. We've all been there - we've been told we need to adopt a new way of working, and then had some new tool from some friend on the C-Suite who says that by simply using it, we'll be happier, more productive, and instantly a 10x engineer. Meanwhile, you've used it before and it's shit.
-->

---
layout: intro
transition: slide-down
---

<div class="multiCol">
    <div class="col">
        <h2>Jeremy Meiss</h2>
        <p style="font-weight: 900; font-size: 1.25rem;">Co-Founder, DevEx Consultant</p>
        <p style="font-size: 1rem;"><em>DevEx Institute</em></p>
        <!-- <p style="font-size: 0.8em;"><a href="https://devex.institute" target="_blank">https://DevEx.Institute</a></p> -->
        <p style="font-size: 1rem;">DevOpsDays Kansas City Organizer</p>
    </div>
    <div class="col">
      <img src="/images/profile-pic.jpg" width="60%" alt="Jeremy Meiss" />
    </div>
</div>

<!--

-->

---

## A working definition of DevEx
  
>_"...the **journey** of developers as they learn and deploy technology, which if successful, focuses on eliminating obstacles that hinder a developer or practitioner from achieving success in their endeavors."  
> -Jessica West, Co-Founder, DevEx Institute_

<!--
Let's start with a definition of DevEx - DevEx is the journey of developers as they learn and deploy technology. When successful, it focuses on eliminating obstacles that hinder a developer or practitioner from achieving success in their endeavors.
-->

---

### Point of clarification

<v-clicks>

- "DevEx" by default focuses on "developer"
- View "DevEx" as a whole of the lifecycle

</v-clicks>

<!--
I think it's important to clarify that "DevEx" by default focuses on the "developer", but we should really view DevEx as a whole part of the lifecycle, and not just for developers only.
-->

---
layout: image
image: "/images/slides/good-devex-overall-satisfaction.jpg"
---


<!--
It's their overall satisfaction and efficiency while working on software projects. It's the tools, the processes, and the environments that shape their interactions with code, infrastructure, and each other. A positive DevEx is crucial for enhancing productivity as it directly influences how quickly and effectively developers can build, test, and deploy software.
-->

---
layout: image
image: "/images/slides/devex-integral-dev-lifecycle.jpg"
---

<!--
DevEx is such an integral part of the entire development lifecycle - not just if you're developing tools for use internally, choosing off-the-shelf tools to use, or creating products for other developers and companies to use. That means that the ease of use, reliability, how accessible and understandable documentation, how efficient the build processes are, the effectiveness of testing frameworks, and the smoothness of deployment procedures all have an impact on the overall dev experience.
-->

---
layout: image
image: "/images/slides/text-to-cloud.jpg"
---


<!--
And we've see an evolution in Developer Experience over the years.

Here's an example of how Developer Experience has evolved a particular set of tools and practices:
-->

---

# Evolution of the IDE

## Early text editors

![USER FRIENDLY by Illiad, vi](/images/slides/httpatomoreillycomsourceoreillyimages2055076.png)
REF: O'Reilly "Learning the vi and Vim Editors"

<!--
I think a great example is the evolution of Integrated Development Environments (IDEs). Prior to the 1990's, you had mostly text-based editors that were used to write code, like Vi, which evidently is supposed to be called "SIX". Who knew? It was created in 1976 and included in the first BSD linux release.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-1.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Early text editors

- 1976: Vi

<v-clicks>

- 1985: Emacs

- 1991: Vim

- 1999: nano

</v-clicks>

<!-- Then we had Emacs in 1985, Vim in 1991, my personal favorite, `nano`. And not entirely because I can exit it without having to throw out the computer and buy a new one like I do with Vim. Saving the planet, one less computer thrown away because of Vim at a time. -->

---
layout: image-left
image: "/images/slides/IDE_evolution-3.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Native IDEs in the 1980s

<v-clicks>

- 1983: Turbo Pascal

- 1986: Apple's Macintosh Programmer's Workshop

</v-clicks>

<!--
A few Native IDEs came out in the mid-80s, with Turbo Pascal in 1983 and Apple's Macintosh Programmer's Workshop in 1986.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-2.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## First plug-in IDE

<!-- One of the first IDEs with a plug-in concept was HP Softbench, released in 1989. HP Softbench was one of the first plug-in IDEs, shipped with its own library, -->

---
layout: image-left
image: "/images/slides/hp-softbench-manuals.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## First plug-in IDE

### HP Softbench

<!--
and was extensively talked about in the June 1990 edition of the HP Journal. 
-->

---
layout: image-left
image: "/images/slides/hpjournal-june1990-hpsoftbench.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## First plug-in IDE

### HP Softbench

REF: [HP Journal, June 1990 edition](http://hparchive.com/Journals/HPJ-1990-06.pdf)

<!--
It's a fascinating read, as HP lays out their vision of what software architecture and development should be, including Automated Testing, distributed computing, integrated and interchangeable tools, and more. The link to the PDF is below - I highly recommend reading it
-->

---
layout: image-left
image: "/images/slides/giphy-thumbs-down.gif"
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Early Reviews

> "...the use of an IDE was not well received by developers since it would fence in their creativity."

REF: _Computerwoche_ ("Computer Week", German counterpart of American magazine _Computer World_), 1995.

<!--
The early reviews of IDEs as a concept weren't great.... In 1995 Computer Week in Germany commented that the use of an IDE was not well received by developers since it would fence in their creativity.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-4.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Cross-platform in the 1990s

### 1995: Borland Delphi

<!--
Borland Delphi was released in 1995 and is still around (Embarcadero Delphi v12)
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-5.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## The Web and the 1990s

<v-clicks>

- 1995: SGI WebMagic

- 1995: Microsoft FrontPage

</v-clicks>

<!--
With the launch of the World Wide Web, and then its explosion of growth, the IDEs started becoming more graphical and had a more modern look and feel. Who remembers the first HTML WYSIWYG editor? SGI's WebMagic was released on January 25, 1995 built in less than 90 days. FrontPage (https://softpanorama.org/Office/Frontpage/history.shtml) was soon to follow in October 1995 after Microsoft acquired it from Vermeer.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-6.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Features & Usability

### Late 1990s to 2000s

<v-clicks>

- 1997: Macromedia Dreamweaver
- 1997: Netscape Composer
- 1997: Microsoft Visual Studio
- 1999: Microsoft FrontPage 2000
- 2000: NetBeans
- 2001: IntelliJ IDEA
- 2001: Eclipse IDE
- 2002: Microsoft Visual Studio .NET

</v-clicks>

<!--
Macromedia's Dreamweaver came out in 1997 (after Macromedia acquisition of Backstage from iBand in 1996) Dreamweaver completely changed the game in many respects, as Macromedia had a history of their products getting community-sourced tools, plugins, scripts, etc. Microsoft FrontPage 2000 saw the first inclusion of plugins and integrations in early 1999 to make web management easier (FrontPage Server Extensions). NetBeans was released in 2000 for Java, with IntelliJ and Eclipse following in 2001 along with Visual Studio which offered enhanced functionality and more sophisticated features like intelligent code completion, refactoring tools, and improved version control integration. We saw a noticeable increase in support for multiple languages and frameworks, making these IDEs more versatile. Microsoft Visual Studio .NET was released in 2002, offering a more modern and feature-rich IDE for .NET development.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-7.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Lightweight & Configurable

### 2010s to Now

<v-clicks>

- 2008: Sublime Text

- 2015: Atom

- 2015: Visual Studio Code

</v-clicks>

<!--
Late 2000s brought about more lightweight IDEs, like Sublime Text and later Atom and Visual Studio Code (VSCode) emerged, focusing on speed, user-friendly interfaces, and extensive plugin ecosystems. They catered to a broader range of developers by being less resource-intensive and more customizable. Event saw integrations with popular Ops tools as well.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-8.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Cloud-based Options

### Now

<v-clicks>

- 2009: PHPanywhere (eventually becoming CodeAnywhere)
- 2010: Cloud9 (AWS bought it in 2016)
- 2018: Glitch
- 2019: GitPod
- 2020: GitHub Codespaces
- 2024: Google Project IDX

</v-clicks>

<!--
Then, we have seen the rise of the cloud and the arrival of cloud-based IDEs: The first was PHPanywhere (eventually becoming CodeAnywhere) in 2009, followed by Cloud9 in 2010 (before AWS bought it in 2016), Glitch (2018), GitPod (2019), GitHub Codespaces (2020), and Google’s Project IDX (2024). They've really changed the game by offering fully configured development environments in the cloud, accessible from anywhere, reducing the need for complex local setup. We went from this sentiment about IDEs...
-->

---

# Evolution of the IDE

## A result of DevEx

### Things we never knew we needed...

From this:
> "...the use of an IDE was not well received by developers since it would fence in their creativity."

<!--
We went from this sentiment about IDEs...
-->

---

# Evolution of the IDE

## A result of DevEx

### Things we never knew we needed...

To this:

- Code completion
- Code refactoring
- Syntax highlighting
- Debugging
- VCS integration (no more FTPing files around)
- Multi-language support
- Framework integration
- Pair programming


<!--
We went from this sentiment about IDEs...
-->

---
layout: image
image: /images/slides/devex-evolution.jpg
backgroundSize: contain
---

<!--
I go through all of that to illustrate how the overall Developer Experience with software development has evolved over time, leading to where we sit with IDEs now. Things we didn't know we would want back in the 1960s are now commonplace and the expeected norm now in the 2020s.
-->

---
layout: image
image: /images/slides/modern-dev-practices.jpg
backgroundSize: contain
---

<!--
### Modern Development

The IDE is just one example of the significant strides made in improving the developer experience. DevEx strategies have evolved to meet contemporary development challenges and opportunities. From basic, manually-configured environments to sophisticated, cloud-based, and automated setups, the journey reflects a relentless pursuit of efficiency, usability, and developer productivity.
-->

---
layout: image
image: /images/slides/rise-of-devops.png
backgroundSize: contain
---

<!--
I would say one of the biggest contributing factors to where we are today with DevEx is the rise of DevOps.
DevOps emphasizes collaboration, automation, and continuous integration and delivery, which has led to the development of more integrated and streamlined development environments and tools. As a result we've seen in recent years a heavy emphasis on, and shift twoards, DevEx at all levels of the software development lifecycle and IT operations.
-->

---
layout: image-left
image: /images/slides/devops-nightmare.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Server Environment Setup

## Manual config nightmares

### Late 1990s to Early 2000s

![cfEngine v1](/images/slides/cfengine-earlylogo.png){width=150px}
![cfEngine v2](/images/slides/cfengine-logo.png){width=250px}

<!--
Another quick example is the setup of environments like dev, staging, and production. In the early days, setting up an environment involved manually configuring each tool, library, and dependency, which was time-consuming and error-prone. Practitioners often struggled with version conflicts and compatibility issues between different tools and libraries.
[click]In the mid- to late-90s systems like CFEngine v1 and CFEngine v2 emerged to automate this process.
-->

---

# Server Environment Setup

## Config Mgmt & Containerization

### Mid-2000s to 2010s

<div class="flex items-center gap-10" style="padding-top:25px;">

  <div><img src="/images/slides/puppet-logo.png" style="max-height: 100px !important;"></div>
  <div><img src="/images/slides/chef-logo.png" style="max-height: 100px !important;"></div>
  <div><img src="/images/slides/saltstack-logo-white.png" style="max-height: 100px !important;"></div>
  <div><img src="/images/slides/ansible-logo.png" style="max-height: 100px !important;"></div>
  <div><img src="/images/slides/docker-logo.png" style="max-height: 100px !important;"></div>

</div>

<!--
The advent of tools like Puppet, Chef, Saltstack, and Ansible allowed for automated setup and configuration of environments, reducing manual effort.

Docker’s introduction in 2013 marked a significant shift, allowing practitioners to package applications with all their dependencies into containers, ensuring consistency across environments.
-->

---

# Server Environment Setup

## IaC and DevOps Integration

### 2010s to Present

<div class="flex items-center gap-4">

  <div><img src="/images/slides/terraform-logo.png" style="max-height: 100px !important;"></div>
  <div><img src="/images/slides/aws-cloudformation-logo.png" style="max-height: 100px !important;"></div>

<v-click>


  <div><img src="/images/slides/jenkins-logo.png" style="max-height: 100px !important;"></div>
  <div><img src="/images/slides/github-actions-logo.png" style="max-height: 100px !important;"></div>

</v-click>

</div>

<!--
Tools like Terraform and AWS CloudFormation enabled defining infrastructure through code, making setup reproducible and scalable.

[click]The integration of environments with CI/CD pipelines and DevOps practices streamlined the whole process, allowing for faster and more reliable builds and deployments.
-->

---

## Broader Impact of DevEx

- Deployment pipelines

- Infrastructure as Code (IaC) practices

- Developer Efficiences

<!--
Just as we saw with IDEs, we've see the broader impact of DevEx on DevOps in things like how we deploy software, infrastructure as code, developer efficiencies, and really many more.
-->

---
layout: quote
---

# What is DevOps?

> ### the combination of practices and tools designed to increase an organization's ability to deliver applications and services faster than traditional software development processes

<!--
DevEx at it core aligns perfectly with what DevOps is....

the combination of practices and tools designed to increase an organization's ability to deliver applications and services faster than traditional software development processes

A few of the core DevOps principles really bring this all together.
-->

---
transition: fade
layout: default
---

## DevOps Principles + DevEx alignment

- Collaboration




<!-- 
**Collaboration** in DevOps **is about creating an environment where silos are broken down, and cross-functional teams are empowered to work as a single unit**. It's people first, and 
-->

---
transition: fade
layout: default
---

## DevOps Principles + DevEx alignment

- Enhanced collaboration _**via tools and processes**_


<!-- 
...tools second. When DevOps and DevEx are aligned, we enhace collaboration through tools and processes that **reduce friction and barriers in the development process, enabling teams to focus more on solving business problems together, leading to innovative solutions and a more harmonious working environment.**
-->

---
transition: fade
layout: default
---

## DevOps Principles + DevEx alignment

- Collaboration

- Communication


<!-- 
The backbone of DevOps is effective **communication**, which ensures all members of the development, operations, and broader organizational team are on the same page. With 
-->

---
transition: fade
layout: default
---

## DevOps Principles + DevEx alignment

- Enhanced collaboration **_via tools and processes_**

- Improving communication **_via streamlined info sharing and feedback_**

<!-- 
When we are **improving Communication** , we start to utilize platforms and tools that streamline information sharing and feedback across teams. That includes your CI/CD pipelines, shared dashboards, and automated alerting systems ensure all team members have visibility into the development process, can easily share updates, and quickly address issues.
-->

---
transition: fade
layout: default
---

## DevOps Principles + DevEx alignment

- Collaboration

- Communication

- Shared Responsibility

<!-- 
**Shared Responsibility** in DevOps means there is **collective accountability for the software's quality and reliability, blurring the lines between roles traditionally separated by development and operations.** It's about **moving away from a "not my job" mentality to a "we're in this together" mindset, where success and failures are shared equally**.
-->

---
transition: fade
layout: default
---

## DevOps Principles + DevEx alignment

- Enhanced collaboration **_via tools and processes_**

- Improving communication **_via streamlined info sharing and feedback_**

- Shared responsibility **_by empowering all teams with access and information_**

<!-- 
That **Shared Responsibility** brings empowerment to all team members with access to the tools and information they need to contribute across the entire software lifecycle. **By democratizing access to tools and information, DevEx encourages a culture where everyone feels ownership of the product and is motivated to contribute to its success.**
-->

---
transition: fade
layout: image
image: /images/slides/38-devex-integ-devops-principles.jpg
backgroundSize: contain
---




<!-- 
Organizations seeking to build more cohesive, agile, and effective teams who are better equipped to meet the demands of modern software development, have to ensure that they don't stop at just these core DevOps principles - but that they ensure an emphasis on DevEx in the implementation of the tooling. If it's a poor experience, you aren't going to see the results you want.

I think a good example is what we've seen with Platform Engineering the last few years.
-->

---
transition: fade
---

## Good DevOps == Good DevEx

<v-clicks>

- Facilitates smoother transitions between Dev and Ops

- Minimizes bottlenecks with enhanced collaboration

- Ensures feedback loops are efficient and productive

- Enables DevOps principles to take hold within an organization

</v-clicks>

<!-- 
[click]A good DevEx facilitates **smoother transitions between your dev and ops teams**, helps [click]**minimize bottlenecks and enhances collaboration**. Proper [click]**feedback loops are part of both DevEx & DevOps**, and with them in place you have a positive DevEx that **ensures those loops are efficient and productive**, all of which which [click]**helps DevOps principles** to take firm hold within an organization. There's no better example than what we've seen with Platform Engineering the last few years.
-->

---
layout: image
image: /images/slides/39-devex-devops-one.jpg
backgroundSize: contain
---

# DevOps + DevEx = Platform Engineering

<!-- 
a robust Developer Experience (DevEx) fosters a more integrated and efficient collaboration between development (Dev) and operations (Ops) teams, and highlights best practices for achieving this unity and efficiency. 
-->

---
layout: image-right
image: /images/slides/40-platform-engineering.jpg
class: my-cool-content-on-the-left
---

## The Rise of Platform Engineering

<v-clicks>

- Specific, integrated environments that devs need

- Abstract away infrastructre + backend complexities

- Access to robust, scalable, easy-to-use platforms

- Streamline development processes and reduced setup time

</v-clicks>

<!-- 
The rise of platform engineering represents a paradigm shift [click]**towards creating comprehensive, integrated environments that cater specifically to the needs of developers**. Focusing on [click]**abstracting away the complexities of infrastructure and backend services**, allows developers to concentrate on writing code and creating value. [click]Platform engineering embodies the principles of DevEx by **ensuring that developers have access to robust, scalable, and easy-to-use platforms**. [click]which **streamline development processes, reduce setup time**, and allow for a focus on innovation rather than maintenance, removing a lot of developer toil.
-->

---
layout: image-right
image: /images/slides/self-service-mode.jpg
class: my-cool-content-on-the-left
---

## Self-Service Platforms

<v-clicks>

- Developers empowered with necessary tools

- Leverage automation, templates, policies with agility

- Accelerate development, enhance productivity, foster autonomy

</v-clicks>

<!-- 
Self-service platforms embody the evolution of DevEx by **empowering developers** to independently provision resources, deploy applications, and manage their lifecycles without waiting for operational support. These platforms **leverage automation, templates, and predefined policies** to ensure compliance and governance, while offering the agility needed for rapid development cycles. By providing developers with the tools to perform tasks that were traditionally in the domain of IT operations, self-service platforms **accelerate development, enhance productivity, and foster a culture of autonomy and innovation**.
-->

---
layout: image
image: /images/slides/42-devex-devops-convergence.jpg
backgroundSize: contain
---

<!-- 
### Bringing DevOps and DevEx Together
When organizations prioritize DevEx, they ensure that devs have access to tools and processes that not only streamline their workflow but also facilitate a smoother transition of code from development to production. This alignment encourages both teams to work closely from the outset of projects, sharing insights, feedback, and responsibilities, which enhances the efficiency of the development lifecycle and leads to higher quality outcomes. Which strenghtens the implementation of DevOps culture and practices.
-->

---
layout: image-left
image: /images/slides/better-practices.jpg
class: my-cool-content-on-the-right
backgroundSize: contain
---

## Better Practices for leveling up DevEx

<v-clicks>

- Empower with the right tools

- Encourage Cross-functional Teams

- Implement Feedback Loops

- Focus on Automation

- Invest in Training and Development

</v-clicks>

<!-- 
Some of the better practices to keep in mind when leveling up with DevEx are:
**Equip teams** with integrated, user-friendly tools that support automation, collaboration, and real-time communication. Choose the tools which align with both Dev and Ops needs. Get their input in the decision. Just because your buddy's IT startup says they offer 10x developer productivity doesn't mean it works for your teams, much less that it works at all.
**Put in place cross-functional teams** that include roles with diverse expertise (e.g., development, operations, quality assurance) to foster a shared understanding and responsibility from project inception through to deployment and maintenance.  
**Establishing robust feedback mechanisms** allow for continuous learning and improvement. Conduct regular retrospectives, incorporate user feedback into development cycles, and use monitoring tools to gather insights on performance and user experience.  
Reduce toil and free up team members to focus on more strategic activities by **automating repetitive and manual tasks wherever possible.** This includes automating testing, deployments, and infrastructure provisioning.  
**Ensure that team members have opportunities to learn and grow** their skills in both development and operations domains. This helps in building empathy between teams and equips individuals with the knowledge to understand and contribute to different stages of the development lifecycle.
-->

---
layout: section
---

# Strategies for Improving DevEx
<!--

-->

---

## DevEx reflects an organizational culture

<Tweet id="1750563607266410692" />

<!-- 
The level of investment that a company invests in DevEx can be a reflection of a company's values towards its employees, especially its developers. A strong focus on DevEx shows a commitment to employee well-being and efficiency. And prioritizing DevEx helps foster a culture of excellence and innovation. When developers are provided with the right tools, support, and environment, they are more likely to produce high-quality work and push the boundaries of what's possible.
-->

---
layout: center
---

# Strategies for Improving DevEx

## Improving DevEx in your organization

**DevEx initiatives should be modeled from Leadership _FIRST_**{style="color: red; font-size: 1.25em; font-weight: bolder;"}

---

## Improving DevEx in your organization

1. Foster a positive culture

2. Streamline the workflow(s)

<!--
I generally break the process of improving DevEx in an organization into two steps

Foster a positive culture
Streamline the workflow(s)
-->

---
layout: image-left
image: /images/slides/clear-concise-docs.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
---

## Improving DevEx
### Foster a positive culture

1. Clear and concise documentation

  - Encourage knowledge sharing
  - Create easily accessible resources to reduce toil + empower

<!--
Fostering a Positive Development Culture
Invest in clear and concise documentation: Encourage knowledge sharing, create easily accessible resources to reduce context switching and empower developers.

-->

---
layout: image-left
image: /images/slides/promote-collab-comms.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
---

## Improving DevEx
### Foster a positive culture

1. Clear and concise documentation

2. Promote collaboration and communication

  - Facilitate code reviews
  - Implement comms to foster teamwork + problem solving


<!--
Promote collaboration and communication: Facilitate code reviews, knowledge-sharing platforms, and communication channels to foster teamwork and problem-solving.
-->

---
layout: image-left
image: /images/slides/champion-growth.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
---

## Improving DevEx
### Foster a positive culture

1. Clear and concise documentation

2. Promote collaboration and communication

3. Champion well-being and growth

  - Encourage feedback, up and down
  - Recognize achievements
  - Create a sense of belonging


<!--
Champion developer well-being and growth: Encourage feedback, recognize achievements, create a sense of belonging to boost morale and developer satisfaction.

-->

---
layout: image-left
image: /images/slides/streamline-workflows.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
---

## Improving DevEx
### Streamline the workflow

1. Tools and Automation

  - Explore tools which are highly regarded in your field
  - Automate repetitive tasks wherever possible

<!--
Streamlining the Development Workflow
This approach focuses on making the development process itself smoother and more efficient. Here are some key strategies:
Focus on tools and automation: Explore options for code editors, version control systems, CI/CD pipelines etc. to automate repetitive tasks and improve development efficiency.

--> 

---
layout: image-left
image: /images/slides/standard-env-setup.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
---

## Improving DevEx
### Streamline the workflow

1. Tools and Automation

2. Standardize environment setup

- Use config management tools
- Streamline onboarding for all team members

<v-click>

**Examples:**

<div class="flex items-center gap-3" style="padding-top:10px;">
  <div><img src="/images/slides/jfrog-artifactory.png"></div>
  <div><img src="/images/slides/jfrog-pipelines.png"></div>
  <div><img src="/images/slides/atlassian-logo.png"></div>
  <div><img src="/images/slides/github-cat.png"></div>
  <div><img src="/images/slides/gitlab-logo.png"></div>
  <div><img src="/images/slides/ansible-logo.png"></div>
</div>

</v-click>

<!--
Standardize development environment setup: Use configuration management tools and streamline onboarding processes to ensure a consistent and efficient development environment for all team members.
Some examples: JFrog’s Artifactory provides that centralized repo for all artifact types, making it easy for deves to find the resources they need; JFrog’s Pipelines provides a CI/CD platform for automating the build, test, deployment process. There’s also JFrog’s new collaboration with GitHub announced today. Atlassian provides a suite of tools which integration collaboration, communication, and knowledge sharing. GitHub and Gitlab provide version control and collaboration. Ansible helps to quickly and consistently set up development environments, saving time and reducing the risk of configuration errors.
--> 

---
layout: statement
---

# DevEx is...

>### "ruthlessly eliminating barriers (and blockers) that keep your practitioners from being successful"


<!-- 
I'll leave you with this, that DevEx is ruthlessly eliminating barriers (and blockers) that keep your practitioners from being successful.
-->

---
layout: two-cols
---


<div class="flex items-center gap-3" style="padding-top:10px;">

## Thank you!

</div>

::right::

<p><img src="/images/bluesky-logo.svg" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px;">@jerdog.dev</p>
<p><img src="/images/linkedin.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px;">/in/jeremymeiss</p>
<p><img src="/images/devto.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px;">@jerdog</p>
<p><img src="/images/mastodon.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px;">@jerdog@hachyderm.io</p>
<p><img src="/images/twitter.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px;">@IAmJerdog</p>


<!-- 

-->

---
layout: end
---


<!-- 

-->

