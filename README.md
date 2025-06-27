<h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/152699296-73cb8002-9a24-47f8-9941-519afacd2195.png">
  <br />
 Self Hosting Guide
</h1>

 <a href="https://github.com/mikeroyal?tab=followers">
         <img alt="followers" title="Follow me on Github for Updates" src="https://custom-icon-badges.demolab.com/github/followers/mikeroyal?color=236ad3&labelColor=1155ba&style=for-the-badge&logo=person-add&label=Follow&logoColor=white"/></a> 	

![Maintenance](https://img.shields.io/maintenance/yes/2024?style=for-the-badge)
![Last-Commit](https://img.shields.io/github/last-commit/mikeroyal/self-hosting-guide?style=for-the-badge)

 #### A guide for getting started with Self Hosting devices including software and hardware that will make you a better and more efficient Self Hosting.
 
 **Note: You can easily convert this markdown file to a PDF in [VSCode](https://code.visualstudio.com/) using this handy extension [Markdown PDF](https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf).**
 
 **Note 2: This guide will constantly be updated with new info as becomes available and please feel to make an [issue](https://github.com/mikeroyal/Self-Hosting-Guide/issues) if you think something should be added.**
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/152699307-1c4ebfcd-a2b0-456c-9a84-01ac255e3782.png">
  <br />
</p>
 
# Table of Contents

1. [Getting Started with Self-Hosting](https://github.com/mikeroyal/Self-Hosting-Guide#getting-started-with-self-hosting)
 
    - [Tools for Self-Hosting](https://github.com/mikeroyal/Self-Hosting-Guide#tools-for-self-hosting)
       * [Containers](https://github.com/mikeroyal/Self-Hosting-Guide#containers)
       * [CI/CD](https://github.com/mikeroyal/Self-Hosting-Guide#cicd)
       * [Development](https://github.com/mikeroyal/Self-Hosting-Guide#development)
       * [Web servers](#web-servers)
       * [Large language models (LLMs)](#llms)
       * [ChatGPT Chatbots](#chatgpt)
       * [Automation](#automation)
       * [Configuration Management](#Configuration-Management)
       * [Cloud Storage](#cloud-storage)
       * [Cloud](https://github.com/mikeroyal/Self-Hosting-Guide#Cloud)
        * [Linode](#Linode)
	* [Nextcloud](#Nextcloud)
	* [DigitalOcean](#DigitalOcean)
        * [Back4app Web Deployment](#back4app-web-deployment)
	* [MinIO Object Storage](#MinIO-Object-Storage)
       * [Databases](#Databases)
         - [SQL](#SQL)
         - [NoSQL](#NoSQL)
       * [Remote Access](https://github.com/mikeroyal/Self-Hosting-Guide#Remote-Access)
       * [Virtualization](https://github.com/mikeroyal/Self-Hosting-Guide#Virtualization)
       * [Password Management](https://github.com/mikeroyal/Self-Hosting-Guide#password-management)
       * [SSH](#ssh)
       * [VPN](#vpn)
       * [LDAP(Lightweight Directory Access Protocol)](#ldap)
       * [Log Management](#log-management)
       * [DNS](#dns)
       * [Network Tools](https://github.com/mikeroyal/Self-Hosting-Guide#network-tools)
       * [Service Discovery](#service-discovery)
       * [Security](#security)
       * [Troubleshooting](#troubleshooting)
       * [Monitoring](https://github.com/mikeroyal/Self-Hosting-Guide#monitoring)
       * [Dashboards](#Dashboards)
       * [Analytics](#Analytics)
       * [Search](#Search)
       * [Notifications](#Notifications)
       * [RSS](#RSS)
       * [Websites/Blogs](#WebsitesBlogs)
       * [Social](#Social)
       * [Nostr](#nostr)
       * [iMessage](#imessage)
       * [Communications](https://github.com/mikeroyal/Self-Hosting-Guide#communications)
       * [Business Management](https://github.com/mikeroyal/Self-Hosting-Guide#business-management)
       * [Collaboration & Synchronization](https://github.com/mikeroyal/Self-Hosting-Guide#Collaboration--Synchronization)
       * [Encryption](#Encryption)
       * [Backups](https://github.com/mikeroyal/Self-Hosting-Guide#backups)
       * [Snapshots Management/System Recovery](snapshots-managementsystem-recovery)
       * [Archiving](#archiving)
       * [Home Server](https://github.com/mikeroyal/Self-Hosting-Guide#home-server)
       * [Media Server](https://github.com/mikeroyal/Self-Hosting-Guide#media-server)
       * [Smart Home Automation](#Smart-Home-Automation)
       * [Voice Assistants](#Voice-Assistants)
       * [Video Surveillance](#Video-Surveillance)
       * [Text-To-Speech Synthesis (TTS)](#Text-To-Speech-Synthesis-TTS)
       * [Video and Audio Processing](#Video-and-Audio-Processing)
       * [Podcasting](#Podcasting)
       * [Audiobooks](#Audiobooks)
       * [Health](#Health)
       * [Gardening](#gardening)
       * [Maps](https://github.com/mikeroyal/Self-Hosting-Guide#maps)
       * [Bookmarks](#Bookmarks)
       * [Photos](https://github.com/mikeroyal/Self-Hosting-Guide#photos)
       * [Pastebins](#pastebins)
       * [Note-Taking](#Note-Taking)
       * [Time Monitoring](#time-monitoring)
       * [Wikis](#wikis)
       * [Gaming](https://github.com/mikeroyal/Self-Hosting-Guide#gaming)
       * [Foundations/Projects](https://github.com/mikeroyal/Self-Hosting-Guide#foundationsprojects)
    
    - [System Hardware](#System-Hardware)
    - [Operating Systems](#Operating-Systems)
    - [Storage](https://github.com/mikeroyal/Self-Hosting-Guide#storage)
    - [File systems](https://github.com/mikeroyal/Self-Hosting-Guide#file-systems)
    - [Books](https://github.com/mikeroyal/Self-Hosting-Guide#books)
    - [Podcasts](https://github.com/mikeroyal/Self-Hosting-Guide#podcasts)
    - [YouTube Channels](https://github.com/mikeroyal/Self-Hosting-Guide#youtube-channels)
    - [Tutorials & Resources](https://github.com/mikeroyal/Self-Hosting-Guide#tutorials--resources)
    - [Useful Subreddits to Follow](https://github.com/mikeroyal/Self-Hosting-Guide#subreddits)

2. [WireGuard](https://github.com/mikeroyal/Self-Hosting-Guide#wireguard)
     * [What is WireGuard?](#what-is-wireguard)
     * [What is Tailscale?](#what-is-tailscale)
     * [What is Netmaker?](#what-is-netmaker)
     * [WireGuard Tools](#wireguard-tools)
     * [Setting up WireGuard with PiVPN](#setting-up-wireguard-with-pivpn)
     * [Setting up WireGuard on Unraid](#setting-up-wireguard-on-unraid)
     * [Setting up WireGuard on pfSense](#setting-up-wireguard-on-pfsense)
     * [Setting up WireGuard on OpenWRT](#setting-up-wireguard-on-openwrt)
     * [Setting up WireGuard on Home Assistant](#setting-up-wireguard-on-home-assistant)

3. [Nextcloud](https://github.com/mikeroyal/Self-Hosting-Guide#nextcloud)

4. [Raspberry Pi](https://github.com/mikeroyal/Self-Hosting-Guide#raspberry-pi)
     
    * [Models of Raspberry Pi boards](#models-of-raspberry-pi-boards)

    * [Raspberry Pi Learning Resources](#raspberry-pi-learning-resources)

    * [Raspberry Pi Operating Systems](#raspberry-pi-operating-systems)

    * [Raspberry Pi Tools](#raspberry-pi-tools)
    
      - [Getting Started with Home Assistant(HA)](#Home-Assistant)
      - [Getting Started with Homebridge](#Homebridge)
      - [Getting Started with ESPHome](#ESPHome)
      - [Turning Raspberry Pi into a Router](#Turning-Raspberry-Pi-into-a-Router)
      - [Setting up Watchdog Time (WDT) on Raspberry Pi](#setting-watchdog-timer-wdt-on-raspberry-pi)

    * [Raspberry Pi Upgrades](#raspberry-pi-upgrades)
    

5. [Grafana](https://github.com/mikeroyal/Self-Hosting-Guide#Grafana)

6. [Networking](https://github.com/mikeroyal/Self-Hosting-Guide#networking)

7. [Docker](https://github.com/mikeroyal/Self-Hosting-Guide#docker)

8. [Kubernetes](https://github.com/mikeroyal/Self-Hosting-Guide#kubernetes)

9. [Ansible](https://github.com/mikeroyal/Self-Hosting-Guide#ansible)

10. [Databases](https://github.com/mikeroyal/Self-Hosting-Guide#databases)

11. [Telco 5G](https://github.com/mikeroyal/Self-Hosting-Guide#telco-5g)

12. [Open Source Security](https://github.com/mikeroyal/Self-Hosting-Guide#open-source-security)

13. [Differential Privacy](https://github.com/mikeroyal/Self-Hosting-Guide#differential-privacy)

14. [Machine Learning](https://github.com/mikeroyal/Self-Hosting-Guide#machine-learning)

15. [IoT Protocols](https://github.com/mikeroyal/Self-Hosting-Guide#iot-protocols)

16. [Operating systems (OS)](https://github.com/mikeroyal/Self-Hosting-Guide#operating-systems)

17. [Middleware](https://github.com/mikeroyal/Self-Hosting-Guide#middleware)

18. [Node Flow editors](https://github.com/mikeroyal/Self-Hosting-Guide#node-flow-editors)

19. [Toolkits](https://github.com/mikeroyal/Self-Hosting-Guide#toolkits)

20. [Data visualization](https://github.com/mikeroyal/Self-Hosting-Guide#data-visualization)
 
21. [Search](https://github.com/mikeroyal/Self-Hosting-Guide#search)

22. [Hardware](https://github.com/mikeroyal/Self-Hosting-Guide#hardware)

23. [In-memory data grids](https://github.com/mikeroyal/Self-Hosting-Guide#in-memory-data-grids)

24. [Home automation](https://github.com/mikeroyal/Self-Hosting-Guide#home-automation)

25. [Robotics](https://github.com/mikeroyal/Self-Hosting-Guide#robotics)

26. [Mesh networks](https://github.com/mikeroyal/Self-Hosting-Guide#mesh-networks)

27. [Blockchain Development](https://github.com/mikeroyal/Self-Hosting-Guide#blockchain-development)

28. [Node.js Development](https://github.com/mikeroyal/Self-Hosting-Guide#nodejs-development)

29. [C/C++ Development](https://github.com/mikeroyal/Self-Hosting-Guide#cc-development)

30. [Java Development](https://github.com/mikeroyal/Self-Hosting-Guide#java-development)

31. [Python Development](https://github.com/mikeroyal/Self-Hosting-Guide#python-development)

32. [Rust Development](https://github.com/mikeroyal/Self-Hosting-Guide#rust-development)

33. [Swift Development](https://github.com/mikeroyal/Self-Hosting-Guide#swift-development)

34. [XML Development](https://github.com/mikeroyal/Self-Hosting-Guide#xml-development)

# Getting Started with Self-Hosting
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

[Self-Hosting](https://www.reddit.com/r/selfhosted/) is the practice of locally hosting(on premises & private web servers) and managing software applications by a person or organization instead of monthly subscriptions from [Software as a service (SaaS) providers](https://azure.microsoft.com/en-us/overview/what-is-saas/).  

Most self-hosted software can be installed using [Docker](https://en.wikipedia.org/wiki/Docker_(software)), a packaging system which allows software to bundle their configuration and dependencies and isolate them from your operating system.  Software using docker can be installed using the command line or via graphical interfaces such as [Portainer](https://github.com/portainer/portainer).  Software is installed with Docker by downloading an image file containing the application, then creating a copy that sets up its own dependencies and configuration within what is called a container.  Without containers you would often need to install different versions of the same programming languages or tools to satisfy the dependencies for the software you want to use which can get complicated.

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/152699308-36691800-8078-4af3-9d5c-711da4e9b26e.png">
  <br />
</p>

## Tools for Self-Hosting
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

### Containers

[Back to the Top](#table-of-contents)

**Container** is a standard unit of software that packages up code and all its dependencies(including CPU, memory, file storage, and network connections) so the application runs quickly and reliably from one computing environment to another. 

  * [Application Container Security Guide | NIST (PDF)](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-190.pdf)

**Container Image** is a lightweight, standalone, executable package of software that includes everything needed to run an application such as the code, runtime, system tools, system libraries, and settings. 

**Best places to get Container Images:**

 * [DockerHub Container Images](https://hub.docker.com/search?image_filter=official&q=&type=image)
 * [LinuxServer.io Container Images](https://fleet.linuxserver.io/)
 * [Quay Container Images](https://quay.io/search)

[Docker Compose](https://github.com/docker/compose) is a tool that was developed to help define and share multi-container applications. With Compose, we can create a YAML file to define the services and with a single command, can spin everything up or tear it all down.

[Docker Include](https://docs.docker.com/compose/compose-file/14-include/) is a Compose application can declare dependency on another Compose application. This is useful if you want to reuse other Compose files. Also, if you need to factor out parts of your application model into separate Compose files so they can be managed separately or shared with others.

[Kompose](https://kompose.io/) is a conversion tool for Docker Compose to container orchestrators such as [Kubernetes](https://kubernetes.io/) or [OpenShift](https://openshift.com/). 

[SwarmKit](https://github.com/moby/swarmkit) is a toolkit for orchestrating distributed systems at any scale. It includes primitives for node discovery, raft-based consensus, task scheduling and more.

[Containerd](https://containerd.io/) is a daemon that manages the complete container lifecycle of its host system, from image transfer and storage to container execution and supervision to low-level storage to network attachments and beyond. It is available for Linux and Windows.

[ContainersSSH](https://containerssh.io/) is an SSH Server that Launches Containers in Kubernetes and Docker on demand.

[Podman](https://podman.io/) is a daemonless, open source, Linux native tool designed to make it easy to find, run, build, share and deploy applications using Open Containers Initiative (OCI) Containers and Container Images. Podman provides a command line interface (CLI) familiar to anyone who has used the Docker Container Engine.

[Lima](https://github.com/lima-vm/lima) is a tool that launches Linux virtual machines with automatic file sharing and port forwarding (similar to WSL2), and [containerd](https://containerd.io/). It's a great free and open-source alternative for [Docker Desktop](https://www.docker.com/products/docker-desktop).

[Colima](https://github.com/abiosoft/colima) is a container runtimes on macOS (and Linux) with minimal setup.

[Portainer Community Edition](https://github.com/portainer/portainer) is a lightweight service delivery platform for containerized applications that can be used to manage Docker, Swarm, Kubernetes and ACI environments. It is designed to be as simple to deploy as it is to use.

[Yacht](https://github.com/SelfhostedPro/Yacht) is a container management UI with a focus on templates and 1-click deployments.

[Kitematic](https://kitematic.com/) is a simple application for managing Docker containers on Mac, Linux and Windows letting you control your app containers from a graphical user interface (GUI).

[HashiCorp Nomad](https://www.nomadproject.io/) is a simple and flexible scheduler and orchestrator to deploy and manage containers and non-containerized applications across on-premises and clouds at scale.

[Open Container Initiative](https://opencontainers.org/about/overview/) is an open governance structure for the express purpose of creating open industry standards around container formats and runtimes.

[OpenNebula](https://opennebula.io/)  is an open source platform delivering a simple but feature-rich and flexible solution to build and manage enterprise clouds for virtualized services, containerized applications and serverless computing. 

[Buildah](https://buildah.io/) is a command line tool to build Open Container Initiative (OCI) images. It can be used with Docker, Podman, Kubernetes.

[Red Hat Universal Base Images (UBI)](https://developers.redhat.com/products/rhel/ubi) is a tool that offers a way to build your container images on a foundation of Red Hat Enterprise Linux software. They are OCI-compliant, container-based, operating system images with complementary runtime languages and packages that are freely redistributable. Easily find UBI images in the Red Hat container catalog, and they are buildable and deployable anywhere. 

[Red Hat Quay](https://quay.io/) is a project that Builds, Stores, and Distributes your Applications and Containers.

[ctop](https://ctop.sh/) is a tool that provides a concise and condensed overview of real-time metrics for multiple containers as well as a [single container view](https://github.com/bcicen/ctop/blob/master/_docs/single.md) for inspecting a specific container. It comes with built-in support for Docker and runC; connectors for other container and cluster systems are planned for future releases.

[runc](https://github.com/opencontainers/runc) is a CLI tool for spawning and running containers on Linux according to the OCI specification.

[container-images](https://github.com/opencontainers/container-images) is a collection of container images used in CI across various opencontainers projects.

[Clair](https://github.com/quay/clair) is an open source project for the static analysis of vulnerabilities in application containers (currently including [OCI](https://github.com/opencontainers/image-spec/blob/master/spec.md) and [Docker](https://github.com/docker/docker/blob/master/image/spec/v1.2.md)).

[Shipwright](https://github.com/SelfhostedPro/Shipwright) is a WebUI to generate templates for Yacht, Portainer, Docker-Compose, and Unraid. 

[Alnoda Workspaces](https://docs.alnoda.org/) is an open-source portable containerized browser-based development environments in Docker containers. You can create your own custom workspace or customize any of the workspaces with your preferred stack of applications without knowing much of the Docker.

[Autoheal](https://hub.docker.com/r/willfarrell/autoheal) monitors and restarts unhealthy docker containers. 

[Dozzle](https://hub.docker.com/r/amir20/dozzle) is a small lightweight application with a web based interface to monitor Docker logs. It doesn’t store any log files. It is for live monitoring of your container logs only. 

[Diun](https://crazymax.dev/diun/) is a tool that receive notifications when a Docker image is updated on a Docker registry. 

[WatchTower](https://hub.docker.com/r/containrrr/watchtower) is a process for automating Docker container base image updates.

[Kasm Workspaces](https://www.kasmweb.com/) is a a highly configurable container streaming platform that enables you to stream and deliver containerized applications over the web. It offers tools that you can use to create desktop workspaces and provide access to virtual desktops to end users. It also ensures data loss prevention as well as secure and private web browsing.

[Nginx Proxy](https://github.com/nginx-proxy/nginx-proxy) is an automation tool that sets up a container running nginx and [docker-gen](https://github.com/nginx-proxy/docker-gen). Docker-gen generates reverse proxy configs for nginx and reloads nginx when containers are started and stopped.

[Visual Studio Code Dev Containers](https://github.com/microsoft/vscode-dev-containers) is an extension that lets you use a [Docker container](https://docker.com/) as a full-featured development environment. It allows you to open any folder inside (or mounted into) a container and take advantage of Visual Studio Code's full feature set. A [devcontainer.json file](https://code.visualstudio.com/docs/devcontainers/containers#_create-a-devcontainerjson-file) in your project tells VS Code how to access (or create) a development container with a well-defined tool and runtime stack. 

### CI/CD

[Back to the Top](#table-of-contents)

 * **CI/CD: Continuous Integration and Continuous Delivery**

[Drone](https://drone.io/) is a Continuous Delivery system built on container technology. Drone uses a simple YAML configuration file, a superset of docker-compose, to define and execute Pipelines inside Docker containers.

[Woodpecker](https://woodpecker-ci.org/) is a CI service, a community fork of Drone.

[Travis CI](https://travis-ci.org/) is a hosted continuous integration service used to build and test software projects hosted at GitHub.

[Circle CI](https://circleci.com/) is a continuous integration and continuous delivery platform that helps software teams work smarter, faster.

[Buddy](https://buddy.works/) is a fully-featured DevOps platform with no learning curve that packs everything you need from a CI/CD tool. 

[Buildbot](https://www.buildbot.net/) is a continuous integration tool which automates the compile or test cycle required to validate changes to the project code base. It queues jobs, executes the jobs when the required resources are available, and reports the results.

### Development

[Back to the Top](#table-of-contents)

[Proxmox VE(Virtual Environment)](https://www.proxmox.com/en/proxmox-ve) is an open-source platform for enterprise virtualization. It has a built-in web interface that you can use to easily manage VMs and containers, software-defined storage and networking, high-availability clustering, and multiple out-of-the-box tools on a single solution.

[Terraform provider plugin for Proxmox](https://github.com/Telmate/terraform-provider-proxmox) is a  Terraform provider for the [Proxmox virtualization platform](https://pve.proxmox.com/pve-docs/) and exposes Terraform resources to provision QEMU VMs and LXC Containers.

[OTF](https://github.com/leg100/otf) is an open source alternative to Terraform Enterprise. Includes SSO, team management, agents, and as many applies as you can throw hardware at.

[Semaphore UI](https://github.com/ansible-semaphore/semaphore) is a modern UI for Ansible. It lets you easily run Ansible playbooks, get notifications about fails, control access to deployment system.

[APITable](https://apitable.com/) is an API-oriented low-code platform for building collaborative apps and better than all other Airtable open-source alternatives. 

[Chisel Kubernetes Operator](https://github.com/FyraLabs/chisel-operator/) is a Kubernetes operator for Chisel. It allows you to use Chisel as a LoadBalancer provider for your Kubernetes cluster, similar to [inlets-operator](https://github.com/inlets/inlets-operator).

[Docker-pgautoupgrade](https://github.com/pgautoupgrade/docker-pgautoupgrade) is a PostgreSQL Docker container that automatically upgrades your database. It's whole purpose in life is to automatically detect the version of PostgreSQL used in the existing PostgreSQL data directory, and automatically upgrade it (if needed) to the required version of PostgreSQL.

[IT-Tools](https://it-tools.tech/) is a collection of handy online tools for developers, with great UX. 

[Lazygit](https://github.com/jesseduffield/lazygit) is a simple terminal UI for git commands, written in Go with the [gocui](https://github.com/jroimartin/gocui) library.

[LazyDocker](https://github.com/jesseduffield/lazydocker) is a  simple terminal UI for both docker and docker-compose, written in Go with the [gocui](https://github.com/jroimartin/gocui) library.

[Code-Server](https://github.com/coder/code-server) is Visual Studio Code running on a remote server, accessible through the browser. 

[Turbopilot](https://github.com/ravenscroftj/turbopilot) is an open source large-language-model based code completion engine that runs locally on your CPU.

[Self-Hosted Sentry nightly](https://develop.sentry.dev/self-hosted/) is an official bootstrap for running your own Sentry with Docker. Sentry, feature-complete and packaged up for low-volume deployments and proofs-of-concept.

[Visual Studio Live Share](https://visualstudio.microsoft.com/services/live-share/) is a service/extension that enables you to collaboratively edit and debug with others in real time, regardless of the programming languages you're using or app types you're building. You can instantly and securely share your current project, start a joint debugging session, share terminal instances, forward localhost web apps, have voice calls, and more.

[GistPad](https://marketplace.visualstudio.com/items?itemName=vsls-contrib.gistfs) is a Visual Studio Code extension that allows you to edit GitHub Gists and repositories from the comfort of your favorite editor. You can open, create, delete, fork and star gists and repositories, and then seamlessly begin editing files as if they were local, without ever cloning, pushing or pulling anything.

[Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) is an extension for Visual Studio Code that launches a development local Server with live reload feature for static & dynamic pages.

[Gitea](https://gittea.dev/) is a community managed painless self-hosted Git service.

[Act](https://github.com/nektos/act) is a a tool to run your GitHub Actions locally.

[Act runner](https://gitea.com/gitea/act_runner) is a runner for Gitea based on [act](https://gitea.com/gitea/act).

[GitLab](https://about.gitlab.com/) is an open source end-to-end software development platform with built-in version control, issue tracking, code review, CI/CD, and more. Self-host GitLab on your own servers, in a container, or on a cloud provider. 

[Bonobo Git Server](https://bonobogitserver.com/) - Set up your own self hosted git server on IIS for Windows. Manage users and have full control over your repositories with a nice user friendly graphical interface. 

[Fossil](https://www.fossil-scm.org/index.html/doc/trunk/www/index.wiki) - Distributed version control system featuring wiki and bug tracker. 

[Gerrit](https://www.gerritcodereview.com/) - A code review and project management tool for Git based projects. 

[Gitblit](https://www.gitblit.com/) - Pure Java stack for managing, viewing, and serving Git repositories. 

[gitbucket](https://gitbucket.github.io/gitbucket-news/) - Easily installable GitHub clone powered by Scala.

[Gitea](https://gitea.io) - Community managed fork of Gogs, lightweight code hosting solution. 

[Gitlist](https://gitlist.org/) - Web-based git repository browser - GitList allows you to browse repositories using your favorite browser, viewing files under different revisions, commit history and diffs. 

[Gitolite](https://gitolite.com/gitolite/index.html) - Gitolite allows you to setup git hosting on a central server, with fine-grained access control and many more powerful features.

[GitPrep](https://github.com/yuki-kimoto/gitprep) - Portable Github clone. 

[Gogs](https://gogs.io/) - Painless self-hosted Git Service written in Go. 

[Kallithea](https://kallithea-scm.org/) - Source code management system that supports two leading version control systems, Mercurial and Git, with a web interface.

[Klaus](https://github.com/jonashaag/klaus) - Simple, easy-to-set-up Git web viewer that Just Works. 

[Lavagna](https://lavagna.io) - Lavagna is an open-source issue/project management tool designed for small teams. Lightweight, pure Java, easy to install, easy to use.

[Leantime](https://leantime.io) - Leantime is a lean project management system for small teams and startups helping to manage projects from ideation through delivery. 

[Taiga](https://taiga.io/) is an open-source project management software for cross-functional teams that work agile across both scrum and kanban frameworks.

[Planka](https://planka.app/) is a realtime kanban board for workgroups built with React and Redux. 

[Microgit](https://github.com/microgit-com/microgit) - Git hosting service made in Crystal and Lucky. `MIT` `Crystal`

[OneDev](https://onedev.io/) - All-In-One DevOps Platform. With Git Management, Issue Tracking, and CI/CD. Simple yet Powerful. 

[OpenProject](https://www.openproject.org) - OpenProject is a web-based project management system. 

[Pagure](https://pagure.io/pagure) - A lightweight, powerful, and flexible git-centric forge with features laying the foundation for federated and decentralized development. 

[Phorge](https://we.phorge.it/) - Phorge is an open source, community driven platform for collaborating, managing, organizing and reviewing software development projects. 

[Redmine](https://www.redmine.org/) - Redmine is a flexible project management web application. ([Demo](http://demo.redmine.org/), 

[RhodeCode](https://rhodecode.com/) - RhodeCode is an open source platform for software development teams. It unifies and simplifies repository management for Git, Subversion, and Mercurial. 

[SCM Manager](https://www.scm-manager.org/) - The easiest way to share and manage your Git, Mercurial and Subversion repositories over http. 

[Taiga](https://www.taiga.io/) - Agile Project Management Tool based on the Kanban and Scrum methods. 

[Titra](https://titra.io/) - Time-tracking solution for freelancers and small teams. 

[Traq](https://traq.io/) - Project management and issue tracking system written in PHP. 

[Tuleap](https://www.tuleap.org/) - Tuleap is a libre suite to plan, track, code and collaborate on software projects. 

[UVDesk](https://www.uvdesk.com/) - UVDesk community is a service oriented, event driven extensible opensource helpdesk system that can be used by your organization to provide efficient support to your clients effortlessly whichever way you imagine. 

[ZenTao](https://www.zentao.pm/) - An agile(scrum) project management system/tool. 

[k3s-ansible](https://github.com/techno-tim/k3s-ansible) is the easiest way to bootstrap a self-hosted High Availability Kubernetes cluster. A fully automated HA k3s etcd install with [kube-vip](https://kube-vip.chipzoller.dev/), [MetalLB](https://metallb.universe.tf/installation/), and more.

[Soft Serve](https://github.com/charmbracelet/soft-serve) is a tasty, self-hostable Git server for the command line.

[Coolify](https://coolify.io/) is an open-source & self-hostable Heroku/Netlify alternative. 

[Corosync Cluster Engine](https://corosync.github.io/corosync/) is a Group Communication System with additional features for implementing high availability within applications. 

[Glow](https://github.com/charmbracelet/glow) is a terminal based markdown reader designed from the ground up to bring out the beauty—and power—of the CLI.  It's used to discover markdown files, read documentation directly on the command line and stash markdown files to your own private collection, so you can read them anywhere. 

[Deep Lake](https://github.com/activeloopai/deeplake) is a data lake for deep learning applications. Our open-source dataset format is optimized for rapid streaming and querying of data while training models at scale, and it includes a simple API for creating, storing, and collaborating on AI datasets of any size. It can be deployed locally or in the cloud, and it enables you to store all of your data in one place, ranging from simple annotations to large videos.

[Node-Red](https://nodered.org/) is a low-code programming for event-driven applications.

[krunvm](https://github.com/containers/krunvm) is a CLI-based utility for creating microVMs from OCI images, using [libkrun](https://github.com/containers/libkrun) and [buildah](https://github.com/containers/buildah).

[Zeal](https://zealdocs.org/) is an offline documentation browser for software developers inspired by [Dash](https://kapeli.com/dash).

### Web servers

[Back to The Top](#table-of-contents)

**Web servers**

[Apache](https://httpd.apache.org/) - Most popular web server.

[OpenResty Manager](https://om.uusec.com/) - The easiest using, powerful and beautiful OpenResty Manager(Nginx Enhanced Version), open source alternative to OpenResty Edge.

[Beakon](https://github.com/RealDudePerson/beakon) - A self-host location sharing webserver. Beakon aims to leak as little data as possible and uses mostly self-contained libraries and local database files. Where possible, it will reference local files and not reach out over any network. 

[Caddy](https://caddyserver.com/) - The HTTP/2 Web Server with Fully Managed TLS.

[Cherokee](https://cherokee-project.com/) - Lightweight, high-performance web server/reverse proxy.

[Lighttpd](https://www.lighttpd.net/) - Web server more optimized for speed-critical environments.

[Nginx](https://nginx.org/) - Reverse proxy, load balancer, HTTP cache, and web server.

[uWSGI](https://github.com/unbit/uwsgi/) - The uWSGI project aims at developing a full stack for building hosting services.

**Web Performance**

[HAProxy](https://www.haproxy.org/) - Software based load Balancing, SSL offloading and performance optimization, compression, and general web routing.

[Squid](https://www.squid-cache.org/) - Caching proxy for the web supporting HTTP, HTTPS, FTP, and more.

[Traefik](https://traefik.io/) - Taefik is a modern HTTP reverse proxy and load balancer made to deploy microservices with ease.

[Varnish](https://www.varnish-cache.org/) - HTTP based web application accelerator focusing on optimizing caching and compression.

### LLMs

[Back to the Top](#table-of-contents)

**Large Language Models (LLMs)** is a language model that uses artificial neural networks to generate text (AI chatbots/search engines). Some notable ones are GPT-3, GPT-4, BLOOM, and LLaMA.

 * [A comprehensive guide to running Llama 2 locally](https://replicate.com/blog/run-llama-locally)
 * [Leaderboard by lmsys.org](https://chat.lmsys.org/?leaderboard)
 * [LLM-Leaderboard](https://github.com/LudwigStumpp/llm-leaderboard)
 * [Open LLM Leaderboard by Hugging Face](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)
 * [Holistic Evaluation of Language Models (HELM)](https://crfm.stanford.edu/helm/latest/?groups=1)

[llama.cpp](https://github.com/ggerganov/llama.cpp) is a Port of Facebook's LLaMA model in C/C++.

[ollama](https://ollama.ai/) is a tool to get up and running with Llama 2 and other large language models locally.

[LocalAI](https://localai.io/) is a self-hosted, community-driven, local OpenAI-compatible API. Drop-in replacement for OpenAI running LLMs on consumer-grade hardware with no GPU required. It's an API to run ggml compatible models: llama, gpt4all, rwkv, whisper, vicuna, koala, gpt4all-j, cerebras, falcon, dolly, starcoder, and many others.
 
[Serge](https://github.com/serge-chat/serge) is a web interface for chatting with Alpaca through llama.cpp. Fully self-hosted & dockerized, with an easy to use API. 

[OpenLLM](https://github.com/bentoml/OpenLLM) is an open platform for operating large language models (LLMs) in production. Fine-tune, serve, deploy, and monitor any LLMs with ease.

[Llama-gpt](https://github.com/getumbrel/llama-gpt) is a self-hosted, offline, ChatGPT-like chatbot. Powered by Llama 2. 100% private, with no data leaving your device. 

[Llama2 webui](https://github.com/liltom-eth/llama2-webui) is a tool to run any Llama 2 locally with gradio UI on GPU or CPU from anywhere (Linux/Windows/Mac). Use `llama2-wrapper` as your local llama2 backend for Generative Agents/Apps. 

[Llama2.c](https://github.com/karpathy/llama2.c) is a tool to Train the Llama 2 LLM architecture in PyTorch then inference it with one simple 700-line C file ([run.c](https://github.com/karpathy/llama2.c/blob/master/run.c)).

[Alpaca.cpp](https://github.com/antimatter15/alpaca.cpp) is a fast ChatGPT-like model locally on your device. It combines the [LLaMA foundation model](https://github.com/facebookresearch/llama) with an [open reproduction](https://github.com/tloen/alpaca-lora) of [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) a fine-tuning of the base model to obey instructions (akin to the [RLHF](https://huggingface.co/blog/rlhf) used to train ChatGPT) and a set of modifications to [llama.cpp](https://github.com/ggerganov/llama.cpp) to add a chat interface.

[GPT4All](https://github.com/nomic-ai/gpt4all) is an ecosystem of open-source chatbots trained on a massive collections of clean assistant data including code, stories and dialogue based on [LLaMa](https://github.com/facebookresearch/llama).

[MiniGPT-4](https://minigpt-4.github.io/) is an enhancing Vision-language Understanding with Advanced Large Language Models

[LoLLMS WebUI](https://github.com/ParisNeo/lollms-webui) is a the hub for LLM (Large Language Model) models. It aims to provide a user-friendly interface to access and utilize various LLM models for a wide range of tasks. Whether you need help with writing, coding, organizing data, generating images, or seeking answers to your questions.

[LM Studio](https://lmstudio.ai/) is a tool to Discover, download, and run local LLMs.

[Ava PLS](https://lmstudio.ai/) small, all-in-one desktop app to run LLMs locally.

[Gradio Web UI](https://github.com/oobabooga/text-generation-webui) is a tool for Large Language Models. Supports transformers, GPTQ, llama.cpp (ggml/gguf), Llama models. 

[OpenPlayground](https://github.com/nat/openplayground) is a playfround for running ChatGPT-like models locally on your device.

[Vicuna](https://vicuna.lmsys.org/) is an open source chatbot trained by fine tuning LLaMA. It apparently achieves more than 90% quality of chatgpt and costs $300 to train.

[Yeagar ai](https://github.com/yeagerai/yeagerai-agent) is a Langchain Agent creator designed to help you build, prototype, and deploy AI-powered agents with ease.

[KoboldCpp](https://github.com/LostRuins/koboldcpp) is an easy-to-use AI text-generation software for GGML models. It's a single self contained distributable from Concedo, that builds off llama.cpp, and adds a versatile Kobold API endpoint, additional format support, backward compatibility, as well as a fancy UI with persistent stories, editing tools, save formats, memory, world info, author's note, characters, and scenarios.

[Minima](https://github.com/dmayboroda/minima) is a configurable conversational RAG system that runs LLM locally and on-premises using containers.

### ChatGPT 

[Back to the Top](#table-of-contents)

**Chatbot UI for ChatGPT**

[Chatbot UI by mckaywrigley](https://github.com/mckaywrigley/chatbot-ui) is an advanced chatbot kit for OpenAI's chat models built on top of Chatbot UI Lite using Next.js, TypeScript, and Tailwind CSS. This version of ChatBot UI supports both GPT-3.5 and GPT-4 models. Conversations are stored locally within your browser. You can export and import conversations to safeguard against data loss. See a [demo](https://twitter.com/mckaywrigley/status/1636103188733640704).

[Chatbot UI Lite by mckaywrigley](https://github.com/mckaywrigley/chatbot-ui-lite) is a simple chatbot starter kit for OpenAI's chat model using Next.js, TypeScript, and Tailwind CSS. See a [demo](https://twitter.com/mckaywrigley/status/1636103188733640704).

**Build locally with Docker:**

```shell
docker build -t chatgpt-ui .
docker run -e OPENAI_API_KEY=xxxxxxxx -p 3000:3000 chatgpt-ui
```

### Running Locally on Windows, MacOS, and Linux:

**1. Clone Project Repo**

```bash
git clone https://github.com/mckaywrigley/chatbot-ui.git
```

**2. Install Dependencies**

```bash
npm i
```

**3. Provide OpenAI API Key**

Create a .env.local file in the root of the repo with your **[OpenAI API Key](https://platform.openai.com/account/api-keys)**:

```bash
OPENAI_API_KEY=YOUR_KEY
```

* **You can set `OPENAI_API_HOST` where access to the official OpenAI host is restricted or unavailable, allowing users to configure an alternative host for their specific needs.**

* **Additionally, if you have multiple OpenAI Organizations, you can set `OPENAI_ORGANIZATION` to specify one.**

**4. Run App**

```bash
npm run dev
```

**You done you should be able to start chatting with ChatGPT!**

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/230762358-a51124d1-9ee4-4d42-b83b-0dab95b7a93f.png">
  <br />
  Chatbot UI
</p>

[MiniGPT-4](https://minigpt-4.github.io/) is an enhancing Vision-language Understanding with Advanced Large Language Models

**Launching Demo Locally**

Try out the demo [demo.py](https://github.com/Vision-CAIR/MiniGPT-4/blob/main/demo.py) on your local machine by running

```python demo.py --cfg-path eval_configs/minigpt4_eval.yaml  --gpu-id 0```

Here, the demo loads Vicuna as 8 bit by default to save some GPU memory usage. Besides, the default beam search width is 1. Under this setting, the **demo cost about 23G GPU memory**. If you have a more powerful GPU with larger GPU memory, you can run the model in 16 bit by setting low_resource to False in the config file [minigpt4_eval.yaml](https://github.com/Vision-CAIR/MiniGPT-4/blob/main/eval_configs/minigpt4_eval.yaml) and use a larger beam search width.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/233298431-db46ccd6-c0c8-48db-9d9f-c142776de51f.png">
  <br />
  MiniGPT-4 Demo
</p>

[GPT4All](https://github.com/nomic-ai/gpt4all) is an ecosystem of open-source chatbots trained on a massive collections of clean assistant data including code, stories and dialogue based on [LLaMa](https://github.com/facebookresearch/llama).

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/232368422-447387b2-5d7b-4aec-872d-7b711a313b4f.gif">
</p>

[GPT4All UI](https://github.com/nomic-ai/gpt4all-ui) is a Flask web application that provides a chat UI for interacting with the GPT4All chatbot. 

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/232368426-2b555ca6-e620-4d18-bfb8-fa71e4eed64e.png">
</p>

[Alpaca.cpp](https://github.com/antimatter15/alpaca.cpp) is a fast ChatGPT-like model locally on your device. It combines the [LLaMA foundation model](https://github.com/facebookresearch/llama) with an [open reproduction](https://github.com/tloen/alpaca-lora) of [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) a fine-tuning of the base model to obey instructions (akin to the [RLHF](https://huggingface.co/blog/rlhf) used to train ChatGPT) and a set of modifications to [llama.cpp](https://github.com/ggerganov/llama.cpp) to add a chat interface.

[llama.cpp](https://github.com/ggerganov/llama.cpp) is a Port of Facebook's LLaMA model in C/C++.

[Serge](https://github.com/serge-chat/serge) is a web interface for chatting with Alpaca through llama.cpp. Fully self-hosted & dockerized, with an easy to use API. 

[OpenPlayground](https://github.com/nat/openplayground) is a playfround for running ChatGPT-like models locally on your device.

[Vicuna](https://vicuna.lmsys.org/) is an open source chatbot trained by fine tuning LLaMA. It apparently achieves more than 90% quality of chatgpt and costs $300 to train.

[Yeagar ai](https://github.com/yeagerai/yeagerai-agent) is a Langchain Agent creator designed to help you build, prototype, and deploy AI-powered agents with ease.

[LocalAI](https://localai.io/) is a self-hosted, community-driven, local OpenAI-compatible API. Drop-in replacement for OpenAI running LLMs on consumer-grade hardware with no GPU required. It's an API to run ggml compatible models: llama, gpt4all, rwkv, whisper, vicuna, koala, gpt4all-j, cerebras, falcon, dolly, starcoder, and many others.

[DoctorGPT](https://github.com/ingyamilmolinar/doctorgpt) is a lightweight self-contained binary that monitors your application logs for problems and diagnoses them.

[HttpGPT](https://github.com/lucoiso/UEHttpGPT/releases) is an Unreal Engine 5 plugin that facilitates integration with OpenAI's GPT based services (ChatGPT and DALL-E) through asynchronous REST requests, making it easy for developers to communicate with these services. It also includes Editor Tools to integrate Chat GPT and DALL-E image generation directly in the Engine.


### Automation

[Back to the Top](#table-of-contents)

[Accelerated Text](https://github.com/accelerated-text/accelerated-text) - Automatically generate multiple natural language descriptions of your data varying in wording and structure. 

[Activepieces](https://www.activepieces.com) - No-code business automation tool like Zapier or Tray. For example, you can send a Slack notification for each new Trello card. 

[ActiveWorkflow](https://github.com/automaticmode/active_workflow) - An intelligent process and workflow automation platform based on software agents. 

[Alltube](https://github.com/Rudloff/alltube) - Web GUI for youtube-dl, a program to download videos and audio from more than 100 websites.

[AmIUnique](https://amiunique.org/) - Learn how identifiable you are on the Internet (browser fingerprinting tool). 

[Automatisch](https://automatisch.io) - Business automation tool that lets you connect different services like Twitter, Slack, and more to automate your business processes (Open source Zapier alternative). 

[Baserow](https://baserow.io/) - Open source online database tool and Airtable alternative. Create your own database without technical experience. 

[betanin](https://github.com/sentriz/betanin) - Music organization man-in-the-middle of your torrent client and music player. Based on beets.io, similar to Sonarr and Radarr.

[ChiefOnboarding](https://chiefonboarding.com) - Employee onboarding platform that allows you to provision user accounts and create sequences with todo items, resources, text/email/Slack messages, and more! Available as a web portal and Slack bot. 

[Datasette](https://datasette.io/) - An open source multi-tool for exploring and publishing data, easy import and export and database management. 

[Eonza](https://www.eonza.org) - Eonza is used to create scripts and automate tasks on servers or VPS hosting. Manage your servers from any browser on any device. 

[Exadel CompreFace](https://exadel.com/solutions/compreface/) - Face recognition system that provides REST API for face recognition, face detection, and other face services, and is easily deployed with docker. There are SDKs for Python and JavaScript languages. Can be used without prior machine learning skills. 

[feed2toot](https://feed2toot.readthedocs.io/en/latest/) - Feed2toot parses a RSS feed, extracts the last entries and sends them to Mastodon.

[feedmixer](https://github.com/cristoper/feedmixer) - FeedMixer is a WSGI (Python3) micro web service which takes a list of feed URLs and returns a new feed consisting of the most recent n entries from each given feed(Returns Atom, RSS, or JSON).

[Headphones](https://github.com/rembo10/headphones) - Automated music downloader for NZB and Torrent, written in Python. It supports SABnzbd, NZBget, Transmission, µTorrent, Deluge and Blackhole. 

[Healthchecks](https://healthchecks.io/) - Django app which listens for pings and sends alerts when pings are late. 

[HRConvert2](https://github.com/zelon88/HRConvert2) - Drag-and-drop file conversion server with session based authentication, automatic temporary file maintenance, and logging capability. 

[Huginn](https://github.com/huginn/huginn) - Allows you to build agents that monitor and act on your behalf. 

[Kibitzr](https://kibitzr.github.io) - Lightweight personal web assistant with powerful integrations. 

[Krayin](https://krayincrm.com/) - Free and Opensource Laravel CRM Application. 

[Leon](https://getleon.ai) - Open-source personal assistant who can live on your server. 

[Lidarr](https://lidarr.audio/) - Lidarr is a music collection manager for Usenet and BitTorrent users. 

[Matchering](https://github.com/sergree/matchering) - A containerized web app for automated music mastering. An open-source alternative to LANDR, eMastered, and MajorDecibel.

[Medusa](https://pymedusa.com/) - Automatic Video Library Manager for TV Shows. It watches for new episodes of your favorite shows, and when they are posted it does its magic. ([Source Code](https://github.com/pymedusa/Medusa)) `GPL-3.0` `Python`

[MeTube](https://github.com/alexta69/metube) - Web GUI for youtube-dl, with playlist support. Allows downloading videos from dozens of websites. `AGPL-3.0` `Python/Nodejs/Docker`

[Nautobot](https://github.com/nautobot/nautobot) is a Network Source of Truth and Network Automation Platform built as a web application atop the Django Python framework with a PostgreSQL or MySQL database.

[nefarious](https://github.com/lardbit/nefarious) - Web application that automates downloading Movies and TV Shows. 

[NocoDB](https://www.nocodb.com/) - No-code platform that turns any database into a smart spreadsheet. It can be considered as an Airtable or Smartsheet alternative. 

[OliveTin](https://github.com/OliveTin/OliveTin) - OliveTin is a web interface for running Linux shell commands.

[Patrowl](https://github.com/Patrowl/PatrowlManager) - Open Source, Smart and Scalable Security Operations Orchestration Platform. 

[Podgrab](https://github.com/akhilrex/podgrab) - Lightweight podcast manager and automatic podcast episode downloader. It will monitor podcasts for your and download them automatically whenever a new episode goes live. 

[pyLoad](https://pyload.net/) - Lightweight, customizable and remotely manageable downloader for 1-click-hosting sites like rapidshare.com or uploaded.to. 

[Radarr](https://radarr.video/) - Radarr is an independent fork of Sonarr reworked for automatically downloading movies via Usenet and BitTorrent, à la Couchpotato. 

[SickRage](https://www.sickrage.ca) - SickRage is an automatic Video Library Manager for TV Shows. Automatic torrent/nzb searching, downloading, and processing at the qualities you want. 

[SiteInspector](https://www.getsiteinspector.com/) - Web-based tool for catching spelling errors, grammatical errors, broken links, and other errors on websites. 

[Sonarr](https://sonarr.tv/) - Automatic TV Shows downloader and manager for Usenet and BitTorrent. It can grab, sort and rename new episodes and automatically upgrade the quality of files already downloaded when a better quality format becomes available. 

[StackStorm](https://stackstorm.com) - StackStorm (aka _IFTTT for Ops_) is event-driven automation for auto-remediation, security responses, troubleshooting, deployments, and more. Includes rules engine, workflow, 160 integration packs with 6000+ actions and ChatOps.

[µTask](https://github.com/ovh/utask) - Automation engine that models and executes business processes declared in yaml. 

### Configuration Management

[Back to The Top](#table-of-contents)

[Ansible](https://www.ansible.com/) -  is a tool  is a powerful, agentless tool that works everywhere and with everything. When you add in proven enterprise engineering and support from Red Hat that's written in Python.

[Ansible.Ai](https://ansible.ai/) is an AI for Ansible Content Development tool to automate in your IT infrastructure and it will generate syntactically correct playbook to help you get there.

[CFEngine](https://cfengine.com/) - is a Lightweight agent system where the configuration state is specified via a declarative language.

[mgmt](https://github.com/purpleidea/mgmt) - is a next generation config management written in Go.

[Pallet](https://palletops.com/) - is a Infrastructure definition, configuration and management via a Clojure DSL.

[Puppet](https://puppetlabs.com/) - is an automated administrative engine for your Linux, Unix, and Windows systems, performs administrative tasks (such as adding users, installing packages, and updating server configurations) based on a centralized specification.

[Chef](https://www.opscode.com/chef/) - is a powerful automation platform that transforms infrastructure into code automating how infrastructure is configured, deployed and managed across any environment.

[(R)?ex](https://www.rexify.org/) - is a friendly automation framework to any combinations of local and remote execution, push and pull style of management, or imperative and declarative approach. 

[Salt](https://www.saltstack.com/) -  is an event-driven automation tool and framework to deploy, configure, and manage complex IT systems. It automates common infrastructure administration tasks and ensure that all the components of your infrastructure are operating in a consistent desired state.

[Fleek](https://getfleek.dev/) is an all-in-one management system for everything you need to be productive on your computer. 

### Cloud Storage

[Back to The Top](#table-of-contents)

[Swift](https://docs.openstack.org/developer/swift/) - A highly available, distributed, eventually consistent object/blob store.

[Syncthing](https://syncthing.net/) - Open Source system for private, encrypted and authenticated distribution of data.

[git-annex assistant](https://git-annex.branchable.com/assistant/) - A synchronized folder on each of your MacOS and Linux computers, Android devices, removable drives, NAS appliances, and cloud services.

[NextCloud](https://nextcloud.com) - Provides access to your files via the web.

[ownCloud](https://owncloud.org) - Provides universal access to your files via the web, your computer or your mobile devices.

[Seafile](https://seafile.com) - Another Open Source Cloud Storage solution.

[SparkleShare](https://sparkleshare.org/) - Provides cloud storage and file synchronization services. By default, it uses Git as a storage backend.

### Cloud

[Back to the Top](#table-of-contents)

#### Linode

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/131386177-004d86df-a21b-4257-a502-0fe6c1e0ff4c.png">
  <br />

</p>

[Linode](https://www.linode.com/) is a cloud hosting company that provides virtual private servers and variety of other cloud services.

  * [Linode Documentation](https://www.linode.com/docs)

  * [Linode Guides & Tutorials ](https://www.linode.com/docs/guides/)

  * [Linode API Guides](https://developers.linode.com/guides/)
  
  * [Linode Marketplace](https://www.linode.com/marketplace/apps/)
  
  * [Self-Hosting the vaultwarden Password Manager](https://www.linode.com/docs/guides/how-to-self-host-the-vaultwarden-password-manager/)

  * [Linode Cloud Community](https://www.linode.com/community/)

  * [Linode Developer Portal](https://www.linode.com/developers/)

  * [Linode Content Resources](https://www.linode.com/content/)
 
**Linode Tools**

[Linode Cloud Manager](https://www.linode.com/products/cloud-manager/) is a user- and mobile-friendly interface to deploy and manage virtual machines, configure networking, and control user accounts.

[Linode API](https://developers.linode.com/api/v4/) is a tool that makes easy to configure, manage, and deploy user management, billing, support tickets, and more with programmatic access to Linode products and services.

[Linode CLI](https://www.linode.com/docs/cli/) is a tool to deploy and manage Linux servers from Linode without leaving the command line.

[Linode Images](https://www.linode.com/products/images/) is a service to capture, store, and deploy your custom images across Linodes or data centers. Easily create your own raw disk image and upload a compressed .gz image file (up to 5 GB) using the Cloud Manager or API to easily deploy to the Linode size and data center you need.

[Linode Integrations](https://www.linode.com/products/integrations/) is a collection of integrations lets you connect infrastructure and dev tools to the Linode platform. That let's you manage your Linode resources using the tools you know and love.

[StackScripts](https://www.linode.com/products/stackscripts/) is a tool to automatically configure new Linode instances using simple scripts. Create [your own StackScript](https://www.linode.com/docs/platform/stackscripts/) or browse the community StackScript library.

[Linode Bare Metal](https://www.linode.com/products/bare-metal/) is the single-tenant solution for applications and organizations with security, compliance, and performance needs. Bare Metal combines direct hardware access and the flexibility of a virtual machine.

#### Nextcloud

[Back to the Top](#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/150701955-f1f514a8-82e6-462f-9fc9-8926b6b7de3e.png">
  <br />
</p>

[Nextcloud](https://nextcloud.com) is an industry-leading, on-premises content collaboration platform for file sync & share and communication server. It is fully open source and you can host it yourself or pay a company to do it for you. Also checkout the following links below:

   - [Nextcloud App Store](https://apps.nextcloud.com)

   - [Nextcloud GitHub](https://github.com/nextcloud)

   - [Nextcloud Developer Program](https://nextcloud.com/developer)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/150701961-ac8be115-34c1-4012-bd69-d1f22a10e48c.png">
  <br />
Nexcloud login screen
</p>

[Nextcloud Hub](https://nextcloud.com/hub/) is a tool that allows you to share and collaborate on documents, send and receive email, manage your calendar and have video chats without data leaks. As fully on-premises solution, Nextcloud Hub provides the benefits of online collaboration without the compliance and security risks.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/150701964-df1dd8d9-1d3a-4376-81e8-f49439fb4356.png">
  <br />
Nexcloud Hub
</p>

[Nextcloud AIO (All In One)](https://github.com/nextcloud/all-in-one) is a tool that provides easy deployment and maintenance with most features included in this one Nextcloud instance. 

[Nextcloud Desktop Client](https://nextcloud.com/install/#install-clients) is a tool to synchronize files from Nextcloud Server with your computer.

[Nextcloud Deck](https://apps.nextcloud.com/apps/deck) is a kanban style organization tool aimed at personal planning and project organization for teams integrated with Nextcloud.

[Nextcloud Files](https://nextcloud.com/files/) is a tool tool that allows your employees have easy access to their files, photos and documents to work and can share and collaborate with team members, customers and partners. So IT knows nobody besides those they shared with has access to those files.

[Nextcloud Talk](https://nextcloud.com/talk/) is a tool that protects your communication better than other team collaboration platforms like Microsoft Teams or Slack, making sure your data stays on your servers. It also goes further than other encrypted communication technologies by keeping even metadata from leaking.

[Nextcloud Home](https://nextcloud.com/athome/) is a tool that allows you store your documents, calendar, contacts and photos on your server at home, at one of at one Nextcloud's providers or in a data center you trust.

[Nextcloud Enterprise](https://nextcloud.com/enterprise/) is a service that gives professional organizations software optimized and tested for mission critical environments.

[Nextcloud Outlook Integration](https://nextcloud.com/outlook/) is a tool that automatically upload files to replace large attachments or integrate Calendars and Contacts in Microsoft Outlook.

[Collabora Online in Nextcloud](https://nextcloud.com/collaboraonline/) is a powerful LibreOffice-based online office suite with collaborative editing, which supports all major document, spreadsheet and presentation file formats and works in all modern browsers.

[ONLYOFFICE integration in Nextcloud](https://nextcloud.com/onlyoffice/) is a service that empowers your users to collaborate on office documents with team members in real time. It has compatibility with Microsoft Office formats means perfect documents, every time.

[Nextcloud VM(virtual machine appliance)](https://download.nextcloudvm.com/) is a set of carefully crafted family of [*nix](https://bit.ly/2UaCC7b) scripts, which interactively guide you through a quality-controlled installation of a Nextcloud instance for Home/SME Server and scripts for Raspberry Pi 4. It is Community developed and maintained.

[LibreSign](https://libresign.github.io/) is a Libre digital signature app for Nextcloud. 

#### DigitalOcean

[Back to the Top](#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/117214946-5bbf9c00-adb2-11eb-96cc-fef7d13d4d06.png">
  <br />
</p>

[DigitalOcean](https://www.digitalocean.com/) is a cloud infrastructure provider that provides developers cloud services that help to deploy and scale applications that run simultaneously on multiple computers with data centers worldwide. 

  * [DigitalOcean Pricing](https://www.digitalocean.com/pricing/)

  * [DigitalOcean GitHub](https://github.com/digitalocean)

  * [DigitalOcean Tutorials](https://www.digitalocean.com/community/tutorials)
  
**DigitalOcean Tools**

[DigitalOcean API](https://developers.digitalocean.com/documentation/v2/) is a service that manages your DigitalOcean infrastructure with our RESTful API.

[DigitalOcean Client libraries](https://developers.digitalocean.com/libraries/) is a collection of libraries lets you use the DigitalOcean API in a variety of programming languages.

[DigitalOcean CLI](https://github.com/digitalocean/doctl) is a service that manages your DigitalOcean infrastructure through your terminal with our open source Command Line Interface (CLI).

[Terraform provider](https://www.terraform.io/docs/providers/do/index.html) is a service that allows the user treat their DigitalOcean infrastructure like code with [Terraform](https://www.terraform.io/).

[DigitalOcean Custom images](https://www.digitalocean.com/docs/images/custom-images/) is a service that quickly builds your environment in the cloud by provisioning servers with your own custom image, or choose from various Linux distributions.

[Container Registry](https://www.digitalocean.com/products/container-registry/) is a service that easily stores, manages, and protects private container images.

### Back4app Web Deployment

[Back4app Web Deployment](https://www.back4app.com/web-deployment-platform) is a Container as a Service (CaaS) provider platform that allows the dev teams to build and deploy containerized applications with no downtime. You can simply connect it to a GitHub repository and publish the code within seconds. 

  * [Back4app Web Deployment Platform Pricing](https://www.back4app.com/pricing/container-as-a-service)

  * [Back4app GitHub](https://github.com/back4app)

  * [Back4app Tutorials](https://www.back4app.com/tutorials)

### MinIO Object Storage

[Back to the Top](#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/219937490-da874c4e-cf91-4f2e-b009-77b7929383ba.png">

</p>

[MinIO](https://min.io/download) is a High Performance Object Storage released under GNU Affero General Public License v3.0. It is API compatible with [Amazon S3 cloud storage service](https://aws.amazon.com/s3/). Use MinIO to build high performance infrastructure for machine learning, analytics and application data workloads. It's one of the fastest object storage platforms globally, with a read/write speed of **183GB/s-171GB/s** if you use standard hardware. It can function as the main storage tier for many workloads like **Spark, TensorFlow, Presto, Hadoop HDFS, and H2O.**

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/219937492-d47107b5-d2c3-4746-a133-cbdac97fa379.png">
</br>
MinIO UI
</p>

**Run the following command to run the latest stable image of MinIO as a container using an ephemeral data volume:**

## Podman

```
podman run -p 9000:9000 -p 9001:9001 \
  quay.io/minio/minio server /data --console-address ":9001"
```

## Docker

```
#docker run -p 9000:9000 --name minio -d minio/minio server /export
```
**If you're using an SSD mounted at /mnt/sdd, then we can run the following to use it instead:**

```
# docker run -v /mnt/ssd:/export -p 9000:9000 --name minio -d minio/minio server /export
```

## MacOS

```
brew install minio/stable/minio
minio server /data
```

## Binary Download for MacOS

```
wget https://dl.min.io/server/minio/release/darwin-amd64/minio
chmod +x minio
./minio server /data
```

## Linux

```
wget https://dl.min.io/server/minio/release/linux-amd64/minio
chmod +x minio
./minio server /data
```

|Architecture |	URL|
|--- | --- | 
|64-bit Intel/AMD |https://dl.min.io/server/minio/release/linux-amd64/minio|
|64-bit ARM |https://dl.min.io/server/minio/release/linux-arm64/minio|
|64-bit PowerPC LE (ppc64le) |https://dl.min.io/server/minio/release/linux-ppc64le/minio|
|IBM Z-Series (S390X) |	https://dl.min.io/server/minio/release/linux-s390x/minio|

## Windows

To run MinIO on 64-bit Windows hosts, download the MinIO executable from the following URL:

```https://dl.min.io/server/minio/release/windows-amd64/minio.exe```

Use the following command to run a standalone MinIO server on the Windows host. Replace D:\ with the path to the drive or directory in which you want MinIO to store data. You must change the terminal or powershell directory to the location of the minio.exe executable, or add the path to that directory to the system $PATH:

```minio.exe server D:\```

## Install from Source

Use the following commands to compile and run a standalone MinIO server from source. Source installation is only intended for developers and advanced users. If you do not have a working Golang environment, please follow [How to install Golang](https://golang.org/doc/install). The minimum version required is [go1.19](https://golang.org/dl/#stable).

```go install github.com/minio/minio@latest```

**After you install MinIO:**

The MinIO deployment starts using default root credentials ```minioadmin:minioadmin```. You can test the deployment using the MinIO Console, an embedded web-based object browser built into MinIO Server. Point a web browser running on the host machine to ```http://127.0.0.1:9000``` and log in with the root credentials. You can use the Browser to create buckets, upload objects, and browse the contents of the MinIO server.


When you run Minio you will be issued a key and a secret. These are used by the client or the web front-end to connect securely. I found my codes by typing in ```docker logs minio```.

```
Created minio configuration file at /root/.minio

Endpoint:  http://172.17.0.2:9000  http://127.0.0.1:9000
AccessKey: accessCode
SecretKey: secretCode
Region:    us-west-1
SQS ARNs:  <none>

Browser Access:
   http://172.17.0.2:9000  http://127.0.0.1:9000

Command-line Access: https://docs.minio.io/docs/minio-client-quickstart-guide
   $ mc config host add myminio http://172.17.0.2:9000 accessCode secretCode

Object API (Amazon S3 compatible):
   Go:         https://docs.minio.io/docs/golang-client-quickstart-guide
   Java:       https://docs.minio.io/docs/java-client-quickstart-guide
   Python:     https://docs.minio.io/docs/python-client-quickstart-guide
   JavaScript: https://docs.minio.io/docs/javascript-client-quickstart-guide

Drive Capacity: 50 GiB Free, 70 GiB Total
```

If you'd like to learn more then most of the Minio client commands support a help flag or give info on the command line:

```
NAME:
  mc - Minio Client for cloud storage and filesystems.

USAGE:
  mc [FLAGS] COMMAND [COMMAND FLAGS | -h] [ARGUMENTS...]

COMMANDS:
  ls       List files and folders.
  mb       Make a bucket or a folder.
  cat      Display file and object contents.
  pipe     Redirect STDIN to an object or file or STDOUT.
  share    Generate URL for sharing.
  cp       Copy files and objects.
  mirror   Mirror buckets and folders.
  diff     Show differences between two folders or buckets.
  rm       Remove files and objects.
  events   Manage object notifications.
  watch    Watch for files and objects events.
  policy   Manage anonymous access to objects.
  session  Manage saved sessions for cp and mirror commands.
  config   Manage mc configuration file.
  update   Check for new mc update.
  version  Print version info.
  help, h  Shows a list of commands or help for one command
```

### Advanced options

You can have your client point to multiple Minio servers, which is really neat especially if you're working on a distributed team.

Minio's test-server called "play" is already configured in the default client, you can see all the servers you have configured with mc config host list.

**To upload the photo to Minio's "play" S3 server just type in:**

```# mc mb play/somebucketname```

```# mc cp ~/Downloads/IMG_2016120-25.jpg play/somebucketname```

**Recursive uploads:**

**If you want to test something larger out you could try uploading your entire Downloads photo, and then you should use the --recursive flag to make sure nothing's missed:**

```# mc cp --recursive ~/Downloads/IMG_2016120-25.jpg myminio/photos```

### Databases

[Back to the Top](#table-of-contents)

#### SQL 

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/169607509-ba5e092f-c566-4014-86a1-258bf75266d0.png">
  <br />
</p>

**[SQL](https://en.wikipedia.org/wiki/SQL)** is a standard language for storing, manipulating and retrieving data in relational databases.

[Coolify](https://coolify.io/) is an open-source & self-hostable Heroku/Netlify alternative. 

[MySQL](https://www.mysql.com/) is a fully managed database service to deploy cloud-native applications using the world's most popular open source database. 

[PostgreSQL](https://www.postgresql.org/) is a powerful, open source object-relational database system with over 30 years of active development that has earned it a strong reputation for reliability, feature robustness, and performance.

[PostgREST](https://github.com/PostgREST/postgrest) is a tool that serves a fully RESTful API from any existing PostgreSQL database. It provides a cleaner, more standards-compliant, faster API than you are likely to write from scratch.

[NocoDB](https://www.nocodb.com/) is an open source #NoCode platform that turns any database into a smart spreadsheet. It turns any MySQL, PostgreSQL, SQL Server, SQLite & MariaDB into a smart-spreadsheet. 

[DBeaver](https://dbeaver.io/) is a free multi-platform database tool for developers, database administrators, analysts and all people who need to work with databases. Supports all popular databases: MySQL, PostgreSQL, SQLite, Oracle, DB2, SQL Server, Sybase, MS Access, Teradata, Firebird, Apache Hive, Phoenix, Presto, etc.

[OmniDB](https://github.com/OmniDB/OmniDB) is a web-based tool for database management.

[Navicat](https://www.navicat.com/) is a series of graphical database management and development software produced by CyberTech Ltd. for MySQL, MariaDB, MongoDB, Oracle, SQLite, PostgreSQL and Microsoft SQL Server. 

[HeidiSQL](https://www.heidisql.com/) is free software, and has the aim to be easy to learn. It lets you see and edit data and structures from computers running one of the database systems MariaDB, MySQL, Microsoft SQL, PostgreSQL and SQLite. 
 
[Beekeeper Studio](https://www.beekeeperstudio.io/) is a cross-platform SQL editor and database manager(MySQL, Postgres, SQLite, SQL Server, and more.) available for Linux, Mac, and Windows. 
 
[UI Bakery](https://uibakery.io/) is a web-based low-code internal tool builder. It can visualize the data pulled from PostgreSQL, MongoDB, MySQL, MicrosoftSQL, Redis.

[IBM DB2](https://www.ibm.com/analytics/db2) is a collection of hybrid data management products offering a complete suite of AI-empowered capabilities designed to help you manage both structured and unstructured data on premises as well as in private and public cloud environments. Db2 is built on an intelligent common SQL engine designed for scalability and flexibility.

[OracleDB](https://www.oracle.com/database/) is a powerful fully managed database helps developers manage business-critical data with the highest availability, reliability, and security.

[MariaDB](https://mariadb.com/) is an enterprise open source database solution for modern, mission-critical applications.

[EventQL](https://eventql.io/documentation/) is a distributed, analytical database. It allows you to store massive amounts of structured data and explore it using SQL and other programmatic query facilities.

[CockroachDB](https://www.cockroachlabs.com/docs/stable/) is the SQL database for building global, scalable cloud services that survive disasters. 

[SQLite](https://sqlite.org/index.html) is a C-language library that implements a small, fast, self-contained, high-reliability, full-featured, SQL database engine.SQLite is the most used database engine in the world. SQLite is built into all mobile phones and most computers and comes bundled inside countless other applications that people use every day.

[SQLite Database Browser](https://sqlitebrowser.org/) is an open source SQL tool that allows users to create, design and edits SQLite database files. It lets users show a log of all the SQL commands that have been issued by them and by the application itself. 

[TimescaleDB](https://github.com/timescale/timescaledb) is an open-source database designed to make SQL scalable for time-series data. It is engineered up from PostgreSQL and packaged as a PostgreSQL extension, providing automatic partitioning across time and space (partitioning key), as well as full SQL support.

[InfluxDB](https://www.influxdata.com/) is an open source time series platform.  This includes APIs for storing and querying data, processing it in the background for [ETL](https://docs.microsoft.com/en-us/azure/architecture/data-guide/relational-data/etl) or monitoring and alerting purposes, user dashboards, Internet of Things sensor data, and visualizing and exploring the data and more. It also has support for processing data from [Graphite](http://graphiteapp.org/).

[Atlas](https://github.com/Netflix/atlas) is an in-memory dimensional [time series database](https://en.wikipedia.org/wiki/Time_series_database).

[dbWatch](https://www.dbwatch.com/) is a complete database monitoring/management solution for SQL Server, Oracle, PostgreSQL, Sybase, MySQL and Azure. Designed for proactive management and automation of routine maintenance in large scale on-premise, hybrid/cloud database environments.

[Adminer](https://www.adminer.org/) is an SQL management client tool for managing databases, tables, relations, indexes, users. Adminer has support for all the popular database management systems such as MySQL, MariaDB, PostgreSQL, SQLite, MS SQL, Oracle, Firebird, SimpleDB, Elasticsearch and MongoDB.

[Knex](https://github.com/knex/knex) is a query builder for PostgreSQL, MySQL, CockroachDB, SQL Server, SQLite3 and Oracle, designed to be flexible, portable, and fun to use. 

[rqlite](https://github.com/rqlite/rqlite) is an easy-to-use, lightweight, distributed relational database, which uses [SQLite](https://www.sqlite.org/) as its storage engine.

[osquery](https://github.com/osquery/osquery) is a SQL powered operating system instrumentation, monitoring, and analytics framework. 

[SQLModel](https://github.com/tiangolo/sqlmodel) is a library for interacting with SQL databases from Python code, with Python objects. It is designed to be intuitive, easy to use, highly compatible, and robust.

[Citus](https://github.com/citusdata/citus) is a [PostgreSQL extension](https://www.citusdata.com/blog/2017/10/25/what-it-means-to-be-a-postgresql-extension/) that transforms Postgres into a distributed database—so you can achieve high performance at any scale.

[DbVisualizer](https://dbvis.com/) is a SQL management tool that allows users to manage a wide range of databases such as Oracle, Sybase, SQL Server, MySQL, H3, and SQLite.

[AppDynamics Database](https://www.appdynamics.com/supported-technologies/database) is a management product for Microsoft SQL Server. With AppDynamics you can monitor and trend key performance metrics such as resource consumption, database objects, schema statistics and more, allowing you to proactively tune and fix issues in a High-Volume Production Environment.

[Toad](https://www.quest.com/toad/) is a SQL Server DBMS toolset developed by Quest. It increases productivity by using extensive automation, intuitive workflows, and built-in expertise. This SQL management tool resolve issues, manage change and promote the highest levels of code quality for both relational and non-relational databases.

[Lepide SQL Server](https://www.lepide.com/sql-storage-manager/) is an open source storage manager utility to analyse the performance of SQL Servers. It provides a complete overview of all configuration and permission changes being made to your SQL Server environment through an easy-to-use, graphical user interface.

[Sequel Pro](https://sequelpro.com/) is a fast MacOS database management tool for working with MySQL. This SQL management tool helpful for interacting with your database by easily to adding new databases, new tables, and new rows.

[ElasticSearch](https://www.elastic.co/) is a search engine based on the Lucene library. It provides a distributed, multitenant-capable full-text search engine with an HTTP web interface and schema-free JSON documents. Elasticsearch is developed in Java.

[Logstash](https://www.elastic.co/products/logstash) is a tool for managing events and logs. When used generically, the term encompasses a larger system of log collection, processing, storage and searching activities.

[Kibana](https://www.elastic.co/products/kibana) is an open source data visualization plugin for Elasticsearch. It provides visualization capabilities on top of the content indexed on an Elasticsearch cluster. Users can create bar, line and scatter plots, or pie charts and maps on top of large volumes of data.

[Trino](https://trino.io/) is a Distributed SQL query engine for big data. It is able to tremendously speed up [ETL processes](https://docs.microsoft.com/en-us/azure/architecture/data-guide/relational-data/etl), allow them all to use standard SQL statement, and work with numerous data sources and targets all in the same system.

[Tableau](https://www.tableau.com/) is a Data Visualization software used in relational databases, cloud databases, and spreadsheets. Tableau was acquired by [Salesforce in August 2019](https://investor.salesforce.com/press-releases/press-release-details/2019/Salesforce-Completes-Acquisition-of-Tableau/default.aspx).

[DataGrip](https://www.jetbrains.com/datagrip/) is a professional DataBase IDE developed by Jet Brains that provides context-sensitive code completion, helping you to write SQL code faster. Completion is aware of the tables structure, foreign keys, and even database objects created in code you're editing.

[RStudio](https://rstudio.com/) is an integrated development environment for R and Python, with a console, syntax-highlighting editor that supports direct code execution, and tools for plotting, history, debugging and workspace management.

#### NoSQL 

[Back to the Top](#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/169607515-65629e5a-83e1-4578-9eb5-afe915f0fad9.png">
  <br />
</p>

**[NoSQL](https://www.ibm.com/cloud/blog/sql-vs-nosql)** is a database that is interchangeably referred to as "nonrelational, or "non-SQL" to highlight that the database can handle huge volumes of rapidly changing, unstructured data in different ways than a relational (SQL-based) database with rows and tables.

[Scylla](https://github.com/scylladb/scylla) is the real-time big data database that is API-compatible with Apache Cassandra and Amazon DynamoDB. 

[Apache Cassandra™](https://cassandra.apache.org/) is an open source NoSQL distributed database trusted by thousands of companies for scalability and high availability without compromising performance. Cassandra provides linear scalability and proven fault-tolerance on commodity hardware or cloud infrastructure make it the perfect platform for mission-critical data.

[Apache HBase™](https://hbase.apache.org/) is an open-source, NoSQL, distributed big data store. It enables random, strictly consistent, real-time access to petabytes of data. HBase is very effective for handling large, sparse datasets. HBase serves as a direct input and output to the Apache MapReduce framework for Hadoop, and works with Apache Phoenix to enable SQL-like queries over HBase tables.

[Hadoop Distributed File System (HDFS)](https://www.ibm.com/analytics/hadoop/hdfs) is a distributed file system that handles large data sets running on commodity hardware. It is used to scale a single Apache Hadoop cluster to hundreds (and even thousands) of nodes. HDFS is one of the major components of Apache Hadoop, the others being [MapReduce](https://www.ibm.com/analytics/hadoop/mapreduce) and [YARN](https://hadoop.apache.org/docs/current/hadoop-yarn/hadoop-yarn-site/YARN.html).

[Redis(REmote DIctionary Server)](https://redis.io/) is an open source (BSD licensed), in-memory data structure store, used as a database, cache, and message broker. It provides data structures such as strings, hashes, lists, sets, sorted sets with range queries, bitmaps, hyperloglogs, geospatial indexes, and streams.

[FoundationDB](https://www.foundationdb.org/) is an open source distributed database designed to handle large volumes of structured data across clusters of commodity servers. It organizes data as an ordered key-value store and employs ACID transactions for all operations. It is especially well-suited for read/write workloads but also has excellent performance for write-intensive workloads. FoundationDB was acquired by [Apple in 2015](https://techcrunch.com/2015/03/24/apple-acquires-durable-database-company-foundationdb/).

[CouchbaseDB](https://www.couchbase.com/) is an open source distributed [multi-model NoSQL document-oriented database](https://en.wikipedia.org/wiki/Multi-model_database). It creates a key-value store with managed cache for sub-millisecond data operations, with purpose-built indexers for efficient queries and a powerful query engine for executing SQL queries.

[MongoDB](https://www.mongodb.com/) is a document database meaning it stores data in JSON-like documents. 

[NoSQLBooster](https://www.nosqlbooster.com/) is a cross-platform IDE for [MongoDB v2.6-5.0](https://www.mongodb.com/download-center/community/releases), which provides a build-in MongoDB script debugger, SQL query, server monitoring tools, chaining fluent query, query code generator, task scheduling, ES2020 support, and advanced IntelliSense experience.

[ClickHouse®](https://github.com/ClickHouse/ClickHouse) is an open-source column-oriented database management system that allows generating analytical data reports in real-time.

[Neo4j](https://neo4j.com/) is a graph database management system that provides an array of tools, libraries, and frameworks to make development faster and easier. 

### Remote Access

[Back to the Top](#table-of-contents)

[FreeRDP](https://github.com/FreeRDP/FreeRDP) is a free remote desktop protocol library and clients.

[Rustdesk](https://rustdesk.com/) is an open source virtual/remote desktop infrastructure for everyone. Display and control your PC (Windows, macOS, and Linux) and Android devices.

[TinyPilot](https://tinypilotkvm.com/) is a tool that enables KVM over IP letting you control any computer remotely.

[X2Go](https://wiki.x2go.org/) is open source remote desktop software for Linux that uses a modified NX 3 protocol. It gives remote access to a Linux system's GUI.

[Apache Guacamole](https://guacamole.apache.org/) is a clientless remote desktop gateway. It supports standard protocols like VNC, RDP, and SSH.

[Remmina](https://remmina.org/) is a Remote access screen and file sharing to your desktop. It has Remote Access Protocol Plugins for [RDP](https://remmina.org/remmina-rdp/), [SSH](https://remmina.org/remmina-ssh/), [SPICE](https://remmina.org/remmina-spice/), [VNC](https://remmina.org/remmina-vnc/), [X2Go](https://remmina.org/remmina-x2go/), [HTTP/HTTPS](https://remmina.org/remmina-www/).

[Remotely](https://github.com/immense/Remotely) is a  remote control and remote scripting solution, built with .NET 6, Blazor, SignalR Core, and WebRTC. 

[P2P Remote Desktop](https://github.com/miroslavpejic85/p2p) is a portable, no configuration or installation needed remote desktop tool.

[Cloudflare Tunnel](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/install-and-setup/tunnel-guide) is a tunneling daemon that proxies traffic from the Cloudflare network to your origins. This daemon sits between Cloudflare network and your origin (a webserver). This attracts client requests and sends them to you via this daemon, without requiring you to poke holes on your firewall and your origin(webserver) can remain as closed as possible. 

[WireGuard®](https://www.wireguard.com/) is a straight-forward, fast and modern VPN that utilizes state-of-the-art cryptography. It aims to be faster, simpler, leaner, and more useful than IPsec while avoiding the massive headache. WireGuard is designed as a general-purpose VPN for running on embedded interfaces and super computers alike, fit for many circumstances. It's cross-platform (Windows, macOS, BSD, iOS, Android) and widely deployable.

[NetBird](https://netbird.io/) is an open-source VPN management platform built on top of WireGuard® making it easy to create secure private networks for your organization or home.

[Tailscale](https://github.com/tailscale) is a WireGuard-based app that makes secure, private networks easy for teams of any scale. It works like an overlay network between the computers of your networks using all kinds of NAT traversal sorcery.

[Headscale](https://github.com/juanfont/headscale) is an open source, self-hosted implementation of the Tailscale coordination server.

[MeshCentral](https://meshcentral.com/) is a full computer management web site. It can run your own web server to remotely manage and control computers on a local network or anywhere on the internet. Once you get the server started, create device group and download and install an agent on each computer you want to manage. 

[VNC Viewer](https://www.realvnc.com/en/connect/download/viewer/) is a free remote desktop application that use can use on your iPhone, iPad, Mac, Windows and Linux computers from anywhere in the world.

[TightVNC](https://www.tightvnc.com/) is a free remote desktop application. It can see the desktop of a remote machine and control it with your local mouse and keyboard, just like you would do it sitting in the front of that computer.

[KRDC](https://apps.kde.org/krdc/) is a client application that allows you to view or even control the desktop session on another machine that is running a compatible server. VNC and RDP is supported.

[Krfb Desktop Sharing](https://apps.kde.org/krfb/) is a server application that allows you to share your current session with a user on another machine, who can use a VNC client to view or even control the desktop.

[wayvnc](https://github.com/any1/wayvnc) is a VNC server for wlroots-based Wayland compositors (no_entry Gnome, KDE and Weston are not supported). It attaches to a running Wayland session, creates virtual input devices, and exposes a single display via the RFB protocol. 

[Waypipe](https://gitlab.freedesktop.org/mstoeckl/waypipe/) is a proxy for Wayland clients. It forwards Wayland messages and serializes changes to shared memory buffers over a single socket. 

### Virtualization

[Back to the Top](#table-of-contents)

[HVM (Hardware Virtual Machine)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/virtualization_types.html) is a virtualization type that provides the ability to run an operating system directly on top of a virtual machine without any modification, as if it were run on the bare-metal hardware.

[PV(ParaVirtualization)](https://wiki.xenproject.org/wiki/Paravirtualization_(PV)) is an efficient and lightweight virtualization technique introduced by the Xen Project team, later adopted by other virtualization solutions. PV does not require virtualization extensions from the host CPU and thus enables virtualization on hardware architectures that do not support Hardware-assisted virtualization.

[Network functions virtualization (NFV)](https://www.vmware.com/topics/glossary/content/network-functions-virtualization-nfv) is the replacement of network appliance hardware with virtual machines. The virtual machines use a hypervisor to run networking software and processes such as routing and load balancing. NFV allows for the separation of communication services from dedicated hardware, such as routers and firewalls. This separation means network operations can provide new services dynamically and without installing new hardware. Deploying network components with network functions virtualization only takes hours compared to months like with traditional networking solutions.

[Software Defined Networking (SDN)](https://www.vmware.com/topics/glossary/content/software-defined-networking) is an approach to networking that uses software-based controllers or application programming interfaces (APIs) to communicate with underlying hardware infrastructure and direct traffic on a network. This model differs from that of traditional networks, which use dedicated hardware devices (routers and switches) to control network traffic.

[Virtualized Infrastructure Manager (VIM)](https://www.cisco.com/c/en/us/td/docs/net_mgmt/network_function_virtualization_Infrastructure/3_2_2/install_guide/Cisco_VIM_Install_Guide_3_2_2/Cisco_VIM_Install_Guide_3_2_2_chapter_00.html) is a service delivery and reduce costs with high performance lifecycle management Manage the full lifecycle of the software and hardware comprising your NFV infrastructure (NFVI), and maintaining a live inventory and allocation plan of both physical and virtual resources.

[Management and Orchestration(MANO)](https://www.etsi.org/technologies/open-source-mano) is an ETSI-hosted initiative to develop an Open Source NFV Management and Orchestration (MANO) software stack aligned with ETSI NFV. Two of the key components of the ETSI NFV architectural framework are the NFV Orchestrator and VNF Manager, known as NFV MANO.

[Magma](https://www.magmacore.org/) is an open source software platform that gives network operators an open, flexible and extendable mobile core network solution. Their mission is to connect the world to a faster network by enabling service providers to build cost-effective and extensible carrier-grade networks. Magma is 3GPP generation (2G, 3G, 4G or upcoming 5G networks) and access network agnostic (cellular or WiFi). It can flexibly support a radio access network with minimal development and deployment effort.

[OpenRAN](https://open-ran.org/) is an intelligent Radio Access Network(RAN) integrated on general purpose platforms with open interface between software defined functions. Open RANecosystem enables enormous flexibility and interoperability with a complete openess to multi-vendor deployments.

[Open vSwitch(OVS)](https://www.openvswitch.org/)is an open source production quality, multilayer virtual switch licensed under the open source Apache 2.0 license. It is designed to enable massive network automation through programmatic extension, while still supporting standard management interfaces and protocols (NetFlow, sFlow, IPFIX, RSPAN, CLI, LACP, 802.1ag).

[Edge](https://www.ibm.com/cloud/what-is-edge-computing) is a distributed computing framework that brings enterprise applications closer to data sources such as IoT devices or local edge servers. This proximity to data at its source can deliver strong business benefits, including faster insights, improved response times and better bandwidth availability.

[Multi-access edge computing (MEC)](https://www.etsi.org/technologies/multi-access-edge-computing) is an Industry Specification Group (ISG) within ETSI to create a standardized, open environment which will allow the efficient and seamless integration of applications from vendors, service providers, and third-parties across multi-vendor Multi-access Edge Computing platforms.

[Virtualized network functions(VNFs)](https://www.juniper.net/documentation/en_US/cso4.1/topics/concept/nsd-vnf-overview.html) is a software application used in a Network Functions Virtualization (NFV) implementation that has well defined interfaces, and provides one or more component networking functions in a defined way. For example, a security VNF provides Network Address Translation (NAT) and firewall component functions.

[Cloud-Native Network Functions(CNF)](https://www.cncf.io/announcements/2020/11/18/cloud-native-network-functions-conformance-launched-by-cncf/) is a network function designed and implemented to run inside containers. CNFs inherit all the cloud native architectural and operational principles including Kubernetes(K8s) lifecycle management, agility, resilience, and observability.

[Physical Network Function(PNF)](https://www.mpirical.com/glossary/pnf-physical-network-function) is a physical network node which has not undergone virtualization. Both PNFs and VNFs (Virtualized Network Functions) can be used to form an overall Network Service.

[Network functions virtualization infrastructure(NFVI)](https://docs.vmware.com/en/VMware-vCloud-NFV/2.0/vmware-vcloud-nfv-reference-architecture-20/GUID-FBEA6C6B-54D8-4A37-87B1-D825F9E0DBC7.html) is the foundation of the overall NFV architecture. It provides the physical compute, storage, and networking hardware that hosts the VNFs. Each NFVI block can be thought of as an NFVI node and many nodes can be deployed and controlled geographically.

[Virtualization-based Security (VBS)](https://docs.microsoft.com/en-us/windows-hardware/design/device-experiences/oem-vbs) is a hardware virtualization feature to create and isolate a secure region of memory from the normal operating system.

[Hypervisor-Enforced Code Integrity (HVCI)](https://docs.microsoft.com/en-us/windows-hardware/drivers/bringup/device-guard-and-credential-guard) is a mechanism whereby a hypervisor, such as Hyper-V, uses hardware virtualization to protect kernel-mode processes against the injection and execution of malicious or unverified code. Code integrity validation is performed in a secure environment that is resistant to attack from malicious software, and page permissions for kernel mode are set and maintained by the hypervisor.

[NVIDIA virtual GPU (vGPU)](https://www.nvidia.com/en-us/data-center/virtual-solutions/) is a software enables powerful GPU performance for workloads ranging from graphics-rich virtual workstations to data science and AI, enabling IT to leverage the management and security benefits of virtualization as well as the performance of NVIDIA GPUs required for modern workloads.

[AMD MxGPU](https://www.amd.com/en/graphics/workstation-virtual-graphics) is a hardware-based virtualized GPU solution, is built on industry standard SR-IOV (Single-Root I/O Virtualization) technology and allows multiple virtualized users per physical GPU to work remotely.

[Proxmox Virtual Environment(VE)](https://www.proxmox.com/en/) is a complete open-source platform for enterprise virtualization. It inlcudes a built-in web interface that you can easily manage VMs and containers, software-defined storage and networking, high-availability clustering, and multiple out-of-the-box tools on a single solution.

[KVM (for Kernel-based Virtual Machine)](https://www.linux-kvm.org/page/Main_Page) is a full virtualization solution for Linux on x86 hardware containing virtualization extensions (Intel VT or AMD-V). It consists of a loadable kernel module, kvm.ko, that provides the core virtualization infrastructure and a processor specific module, kvm-intel.ko or kvm-amd.ko.

[QEMU](https://www.qemu.org) is a fast processor emulator using a portable dynamic translator. QEMU emulates a full system, including a processor and various peripherals. It can be used to launch a different Operating System without rebooting the PC or to debug system code.

[Quickemu](https://github.com/wimpysworld/quickemu) is a program that quickly create and run optimised Windows, macOS and Linux desktop virtual machines.

[Hyper-V](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/) enables running virtualized computer systems on top of a physical host. These virtualized systems can be used and managed just as if they were physical computer systems, however they exist in virtualized and isolated environment. Special software called a hypervisor manages access between the virtual systems and the physical hardware resources. Virtualization enables quick deployment of computer systems, a way to quickly restore systems to a previously known good state, and the ability to migrate systems between physical hosts.

[Cloud Hypervisor](https://github.com/cloud-hypervisor/cloud-hypervisor) is an open source Virtual Machine Monitor (VMM) that runs on top of [KVM](https://www.kernel.org/doc/Documentation/virtual/kvm/api.txt). The project focuses on exclusively running modern, cloud workloads, on top of a limited set of hardware architectures and platforms. Cloud workloads refers to those that are usually run by customers inside a cloud provider. Cloud Hypervisor is implemented in [Rust](https://www.rust-lang.org/) and is based on the [rust-vmm](https://github.com/rust-vmm) crates.

[VirtManager](https://github.com/virt-manager/virt-manager) is a graphical tool for managing virtual machines via libvirt. Most usage is with QEMU/KVM virtual machines, but Xen and libvirt LXC containers are well supported. Common operations for any libvirt driver should work.

[oVirt](https://www.ovirt.org) is an open-source distributed virtualization solution, designed to manage your entire enterprise infrastructure. oVirt uses the trusted KVM hypervisor and is built upon several other community projects, including libvirt, Gluster, PatternFly, and Ansible. Founded by Red Hat as a community project on which Red Hat Enterprise Virtualization is based allowing for centralized management of virtual machines, compute, storage and networking resources, from an easy-to-use web-based front-end with platform independent access.

[Firecracker](http://firecracker-microvm.io/) is an open source virtualization technology that is purpose-built for creating and managing secure, multi-tenant container and function-based services that provide serverless operational models. It runs workloads in lightweight virtual machines, called microVMs, which combine the security and isolation properties provided by hardware virtualization technology with the speed and flexibility of containers.

[Foreman](https://theforeman.org/) is a free open source project that gives you the power to easily automate repetitive tasks, quickly deploy applications, and proactively manage your servers life cycle, on-premises or in the cloud.

[Harvester](https://harvesterhci.io/) is an open source hyper-converged infrastructure (HCI) software built on Kubernetes.

[Anthos](https://cloud.google.com/anthos/docs/concepts/overview) is a modern application management platform that provides a consistent development and operations experience for cloud and on-premises environments.

[OpenNebula](https://opennebula.io/)  is an open source platform delivering a simple but feature-rich and flexible solution to build and manage enterprise clouds for virtualized services, containerized applications and serverless computing. 

[HyperKit](https://github.com/moby/hyperkit) is a toolkit for embedding hypervisor capabilities in your application. It includes a complete hypervisor, based on [xhyve](https://github.com/mist64/xhyve)/[bhyve](https://bhyve.org/), which is optimized for lightweight virtual machines and container deployment. It is designed to be interfaced with higher-level components such as the [VPNKit](https://github.com/moby/vpnkit) and [DataKit](https://github.com/moby/datakit). HyperKit currently only supports macOS using the [Hypervisor.framework](https://developer.apple.com/library/mac/documentation/DriversKernelHardware/Reference/Hypervisor/index.html) making it a core component of Docker Desktop for Mac.

[Intel® Graphics Virtualization Technology (Intel® GVT)](https://github.com/intel/gvt-linux) is a full GPU virtualization solution with mediated pass-through, starting from 4th generation Intel Core (TM) processors with Intel processor graphics(Broadwell and newer). It can be used to virtualize the GPU for multiple guest virtual machines, effectively providing near-native graphics performance in the virtual machine and still letting your host use the virtualized GPU normally.

[Apple Hypervisor](https://developer.apple.com/documentation/hypervisor) is a frameowrk that builds virtualization solutions on top of a lightweight hypervisor, without third-party kernel extensions. Hypervisor provides C APIs so you can interact with virtualization technologies in user space, without writing kernel extensions (KEXTs). As a result, the apps you create using this framework are suitable for distribution on the [Mac App Store](https://www.appstore.com/).

[Apple Virtualization Framework](https://developer.apple.com/documentation/virtualization) is a framework that provides high-level APIs for creating and managing virtual machines on Apple silicon and Intel-based Mac computers. This framework is used to boot and run a Linux-based operating system in a custom environment that you define. It also supports the [Virtio specification](https://www.redhat.com/en/virtio-networking-series), which defines standard interfaces for many device types, including network, socket, serial port, storage, entropy, and memory-balloon devices.

[Apple Paravirtualized Graphics Framework](https://developer.apple.com/documentation/paravirtualizedgraphics) is a framework that implements hardware-accelerated graphics for macOS running in a virtual machine, hereafter known as the guest. The operating system provides a graphics driver that runs inside the guest, communicating with the framework in the host operating system to take advantage of Metal-accelerated graphics.

[Cilicon](https://github.com/traderepublic/Cilicon) is a macOS App that leverages Apple's Virtualization Framework to create, provision and run ephemeral virtual machines with minimal setup or maintenance effort. You should be able to get up and running with your self-hosted CI in less than an hour.

[Xen](https://github.com/xen-project/xen) is focused on advancing virtualization in a number of different commercial and open source applications, including server virtualization, Infrastructure as a Services (IaaS), desktop virtualization, security applications, embedded and hardware appliances, and automotive/aviation.

[Ganeti](https://github.com/ganeti/ganeti) is a virtual machine cluster management tool built on top of existing virtualization technologies such as Xen or KVM and other open source software. Once installed, the tool assumes management of the virtual instances (Xen DomU).

[Packer](https://www.packer.io/) is an open source tool for creating identical machine images for multiple platforms from a single source configuration. Packer is lightweight, runs on every major operating system, and is highly performant, creating machine images for multiple platforms in parallel. Packer does not replace configuration management like Chef or Puppet. In fact, when building images, Packer is able to use tools like Chef or Puppet to install software onto the image.

[Vagrant](https://www.vagrantup.com/) is a tool for building and managing virtual machine environments in a single workflow. With an easy-to-use workflow and focus on automation, Vagrant lowers development environment setup time, increases production parity, and makes the "works on my machine" excuse a relic of the past. It provides easy to configure, reproducible, and portable work environments built on top of industry-standard technology and controlled by a single consistent workflow to help maximize the productivity and flexibility of you and your team.

### Password Management

[Back to the Top](#table-of-contents)

[Bitwarden](https://bitwarden.com/host/) is a free and open-source password management service that stores sensitive information such as website credentials in an encrypted vault. 

[Bitwarden Server](https://github.com/bitwarden/server) is a project contains the APIs, database, and other core infrastructure items needed for the "backend" of all bitwarden client applications. Checkout [Bitwarden's self-hosted release repository](https://github.com/bitwarden/self-host).

[Vaultwarden](https://github.com/dani-garcia/vaultwarden) is an unofficial Bitwarden compatible server written in Rust, formerly known as bitwarden_rs.

[Passbolt](https://www.passbolt.com/) is an open-source/self-hosted password manager for teams. It allows you to securely share and store credentials. For instance, the wifi password of your office, the administrator password of a router or your organization's social media account passwords, all of them can be secured using passbolt. 

[KeePassXC](https://keepassxc.org/) is a modern, secure, and open-source password manager that stores and manages your most sensitive information. You can run KeePassXC on Windows, macOS, and Linux systems. It saves many different types of information, such as usernames, passwords, URLs, attachments, and notes in an offline, encrypted file that can be stored in any location, including private and public cloud solutions.

[AuthPass.app](https://authpass.app/) is an Open-Source Password Manager for mobile and desktop that is Keepass 2.x (kdbx 3.x) compatible.

[pass](https://www.passwordstore.org/) is an open-source unix-based password utilitiy with various [gui clients](https://www.passwordstore.org/#other)

### SSH

[Back to The Top](#table-of-contents)

 * **Secure Shell Protocol (SSH)** is a cryptographic network protocol for operating network services securely over an unsecured network.

[Advanced SSH config](https://pypi.python.org/pypi/advanced-ssh-config/) is a tool that enhances ssh_config file capabilities, completely transparent.

[AutoSSH](https://www.harding.motd.ca/autossh/) is a tool that automatically respawn ssh session after network interruption.

[ContainersSSH](https://containerssh.io/) is an SSH Server that Launches Containers in Kubernetes and Docker on demand.

[Cluster SSH](https://sourceforge.net/projects/clusterssh/) is a tool that controls a number of xterm windows via a single graphical console.

[DSH](https://www.netfort.gr.jp/~dancer/software/dsh.html.en)  is a Dancer's shell / distributed shell - Wrapper for executing multiple remote shell commands from one command line.

[Flightplan](https://github.com/pstadler/flightplan) is a node.js library for streamlining application deployment or systems administration tasks (local and remote hosts).

[Mosh](https://mosh.org/) is a command-line program, like SSH. You can use it inside xterm, gnome-terminal, urxvt, Terminal.app, iTerm, emacs, screen, or tmux.

[Parallel SSH](https://parallel-ssh.org/) is an asynchronous parallel SSH library designed for large scale automation. It differentiates ifself from alternatives, other libraries and higher level frameworks like Ansible or Chef.

[SSH Audit](https://github.com/jtesta/ssh-audit) is a tool for SSH server & client configuration auditing (banner, key exchange, encryption, mac, compression, compatibility, security, etc).

[Sshwifty](https://sshwifty-demo.nirui.org/) is a SSH and Telnet connector made for the Web. It can be deployed on your computer or server to provide SSH and Telnet access interface for any compatible (standard) web browser.

[SSHrc](https://github.com/Russell91/sshrc) is a tool that sources ~/.sshrc on your local computer after logging in remotely.

[StormSSH](https://stormssh.readthedocs.org) is a command line tool to manage SSH connections.

[Tailscale SSH](https://tailscale.com/kb/1193/tailscale-ssh/) is a service that allows Tailscale to manage the authentication and authorization of SSH connections on your tailnet.


### VPN

[Back to The Top](#table-of-contents)

 * **VPN (Virtual Private Network)** is a service that encrypts your internet traffic on unsecured networks to protect your online identity, hide your IP address, and shield your online data from third parties. 

[Wireguard](https://www.wireguard.com/) - New minimal VPN Solution that is very fast.

[OpenVPN](https://community.openvpn.net) - Uses a custom security protocol that utilizes SSL/TLS for key exchange.

[Pritunl](https://pritunl.com/) - OpenVPN based solution that's easy to set up.

[SoftEther](https://www.softether.org/) - Multi-protocol software VPN with advanced features.

[sshuttle](https://github.com/apenwarr/sshuttle) - Poor man's VPN.

[strongSwan](https://www.strongswan.org/) - Complete IPsec implementation for Linux.

[tinc](https://www.tinc-vpn.org/) - Distributed p2p VPN.

### LDAP

[Back to The Top](#table-of-contents)

**LDAP Servers**

[389 Directory Server](https://port389.org) - Developed by Red Hat.

[Apache Directory Server](https://directory.apache.org/) - Apache Software Foundation project written in Java.

[Fusion Directory](https://www.fusiondirectory.org) - Improve the Management of the services and the company directory based on OpenLDAP.
[OpenDJ](https://opendj.forgerock.org/) - Fork of OpenDS.

[OpenDS](https://opends.java.net/) - Another directory server written in Java.

[OpenLDAP](https://openldap.org/) - Developed by the OpenLDAP Project.

**LDAP management**

[Apache Directory Studio](https://directory.apache.org/studio/) - The Eclipse-based LDAP browser and directory client

### Log Management

[Back to The Top](#table-of-contents)

[Echofish](https://echothrust.github.io/echofish/) - A web based real-time event log aggregation, analysis, monitoring and management system.

[Fluentd](https://www.fluentd.org/) - Log Collector and Shipper.

[Flume](https://flume.apache.org/) - Distributed log collection and aggregation system.

[Graylog2](https://graylog2.org/) - Pluggable Log and Event Analysis Server with Alerting options.

[Heka](https://hekad.readthedocs.org/en/latest/) - Stream processing system which may be used for log aggregation.

[Elasticsearch](https://www.elasticsearch.org/) - A Lucene Based Document store mainly used for log indexing, storage and analysis.

[Kibana](https://www.elasticsearch.org/overview/kibana/) - Visualize logs and time-stamped data.

[Logstash](https://logstash.net/) - Tool for managing events and logs.

[Octopussy](https://www.octopussy.pm) - Log Management Solution (Visualize/Alert/Report).

### DNS

[Back to The Top](#table-of-contents)

[Duckdns](https://duckdns.org/) - A free service which will point a DNS (sub domains of duckdns.org) to an IP of your choice. The service is completely free, and doesn't require reactivation or forum posts to maintain its existence.

[dnsmasq](http://www.thekelleys.org.uk/dnsmasq/doc.html) - A lightweight service providing DNS, DHCP and TFTP services to small-scale networks.

[MagicDNS](https://tailscale.com/kb/1081/magicdns/) is a tool that automatically registers DNS names for devices in your network.

[Bind](https://www.isc.org/downloads/bind/) - The most widely used name server software.

[djbdns](http://cr.yp.to/djbdns.html) - A collection of DNS applications, including tinydns.

[Designate](https://wiki.openstack.org/wiki/Designate) - DNS REST API that support several DNS servers as its backend.

[Knot](https://www.knot-dns.cz/) - High performance authoritative-only DNS server.

[Lexicon](https://github.com/AnalogJ/lexicon) is a tool that provides a way to manipulate DNS records on multiple DNS providers in a standardized way.

[NSD](http://www.nlnetlabs.nl/projects/nsd/) - Authoritative only, high performance, simple name server.

[PowerDNS](https://www.powerdns.com/) - DNS server with a variety of data storage back-ends and load balancing features.

[CoreDNS](https://coredns.io/) is a DNS server/forwarder, written in Go, that chains [plugins](https://coredns.io/plugins). Each plugin performs a (DNS) function.

[Unbound](http://unbound.net/) - Validating, recursive, and caching DNS resolver.

[Yadifa](http://yadifa.eu/) - Lightweight authoritative Name Server with DNSSEC capabilities powering the .eu top-level domain.

### Network Tools

[Back to the Top](#table-of-contents)

[MQTT](https://mqtt.org/) is an [OASIS standard](https://www.oasis-open.org/standards/) messaging protocol for the Internet of Things (IoT). It is designed as an extremely lightweight publish/subscribe messaging transport that is ideal for connecting remote devices with a small code footprint and minimal network bandwidth.

[Mongoose](https://github.com/cesanta/mongoose) is a networking library for C/C++. It implements event-driven non-blocking APIs for TCP, UDP, HTTP, WebSocket, MQTT. It is designed for connecting devices and bringing them online.

[Nautobot](https://github.com/nautobot/nautobot) is a Network Source of Truth and Network Automation Platform built as a web application atop the Django Python framework with a PostgreSQL or MySQL database.

[Eclipse Mosquitto](https://github.com/eclipse/mosquitto) is an open source implementation of a server for version 5.0, 3.1.1, and 3.1 of the [MQTT](https://mqtt.org/) protocol. 

[Ejabberd](https://ejabberd.im/) is an open-source, robust, scalable and extensible realtime platform built using [Erlang/OTP](https://www.erlang.org/), that includes [XMPP](https://xmpp.org/) Server, [MQTT](https://mqtt.org/) Broker and [SIP](https://en.wikipedia.org/wiki/Session_Initiation_Protocol) Service.

[Nebula](https://github.com/slackhq/nebula) is a scalable overlay networking tool with a focus on performance, simplicity and security. It lets you seamlessly connect computers anywhere in the world. Nebula is portable, and runs on Linux, OSX, Windows, iOS, and Android. It can be used to connect a small number of computers, but is also able to connect tens of thousands of computers.

[LibreSpeed](https://librespeed.org/) is a network speed test tool that can be run on your LAN or hosted in the cloud.

[SmokePing](https://oss.oetiker.ch/smokeping/) is a deluxe latency measurement tool. It can measure, store and display latency, latency distribution and packet loss. It uses RRDtool to maintain a longterm data-store and to draw pretty graphs, giving up to the minute information on the state of each network connection.

[Tailnet](https://tailscale.com/kb/1136/tailnet/) is your private network. When you log in for the first time to Tailscale on your phone, laptop, desktop, or cloud VM, a tailnet is created. For personal users, you are a tailnet of many devices and one person. Each device gets a private Tailscale IP address in the [CGNAT](https://tailscale.com/kb/1015/100.x-addresses/) range and every device can talk directly to every other device, wherever they are on the internet.

[Tailscale SSH](https://tailscale.com/kb/1193/tailscale-ssh/) is a service that allows Tailscale to manage the authentication and authorization of SSH connections on your tailnet.

[Tailscale Funnel](https://tailscale.com/kb/1223/tailscale-funnel/) is a feature that allows you to route traffic from the wider internet to one or more of your Tailscale nodes. You can think of this as publicly sharing a node for anyone to access, even if they don’t have Tailscale themselves.

[Cockpit](https://cockpit-project.org/) is a web-based graphical interface for servers, intended for everyone. It uses [your system’s normal user logins and privileges](https://cockpit-project.org/guide/latest/privileges). Network-wide logins are also supported through [single-sign-on](https://cockpit-project.org/guide/latest/sso) and other [authentication](https://cockpit-project.org/guide/latest/authentication) techniques.

[NetBox](https://docs.netbox.dev/) is a leading solution for modeling and documenting modern networks. It combines the traditional disciplines of IP address management (IPAM) and datacenter infrastructure management (DCIM) with powerful APIs and extensions, NetBox provides the ideal "source of truth" to power network automation.

[Network UPS Tools (NUT)](https://networkupstools.org/) is a project that provides support for Power Devices, such as Uninterruptible Power Supplies, Power Distribution Units, Automatic Transfer Switches, Power Supply Units and Solar Controllers. NUT provides a common protocol and set of tools to monitor and manage such devices, and to consistently name equivalent features and data points, across a vast range of vendor-specific protocols and connection media types.

[Dnsmasq](https://dnsmasq.org/) is a tool that provides network infrastructure for small networks: DNS, DHCP, router advertisement and network boot. It is designed to be lightweight and have a small footprint, suitable for resource constrained routers and firewalls. It has also been widely used for tethering on smartphones and portable hotspots, and to support virtual networking in virtualisation frameworks. Supported platforms include Linux (with glibc and uclibc), Android, BSD, and MacOS. 

[Nginx proxy manager (NPM)](https://nginxproxymanager.com/) is a reverse proxy management system running on Docker. It's easy to set up and does not require users to know how to work with Nginx servers or SSL certificates.

[Netdata](https://github.com/netdata/netdata) is high-fidelity infrastructure monitoring and troubleshooting, real-time monitoring Agent collects thousands of metrics from systems, hardware, containers, and applications with zero configuration. It runs permanently on all your physical/virtual servers, containers, cloud deployments, and edge/IoT devices, and is perfectly safe to install on your systems mid-incident without any preparation.

[Pi-hole](https://pi-hole.net/) is a [DNS sinkhole](https://en.wikipedia.org/wiki/DNS_Sinkhole) that protects your devices from unwanted content, without installing any client-side software, intended for use on a private network. It is designed for use on embedded devices with network capability, such as the Raspberry Pi, but it can be used on other machines running Linux and cloud implementations.

[OWASP Amass](https://owasp.org/www-project-amass/) is a tool that performs network mapping of attack surfaces and external asset discovery using open source information gathering and active reconnaissance techniques.

[Smap](https://github.com/s0md3v/Smap) is a port scanner built with shodan.io's free API. It takes same command line arguments as Nmap and produces the same output which makes it a drop-in replacament for Nmap.

[ORY Oathkeeper](https://github.com/ory/oathkeeper) is an Identity & Access Proxy (IAP) and Access Control Decision API that authorizes HTTP requests based on sets of Access Rules.

[Ory Kratos](https://github.com/ory/kratos) is a developer-friendly, security-hardened and battle-test Identity, User Management and Authentication system for the Cloud. The Kratos identity server (similiar to Auth0, Okta, Firebase) with Ory-hardened authentication, MFA, FIDO2, TOTP, WebAuthn, profile management, identity schemas, social sign in, registration, account recovery, passwordless. 

[Ory Hydra](https://github.com/ory/hydra) is a hardened, OpenID Certified OAuth 2.0 Server and OpenID Connect Provider optimized for low-latency, high throughput, and low resource consumption. Ory Hydra is not an identity provider (user sign up, user login, password reset flow), but connects to your existing identity provider through a [login and consent app](https://www.ory.sh/docs/hydra/oauth2#authenticating-users-and-requesting-consent).

[Ory Keto](https://github.com/ory/keto) is an Open Source (Go) implementation of [Zanzibar: Google's Consistent, Global Authorization System](https://research.google/pubs/pub48190/). It ships gRPC, REST APIs, newSQL, and an easy and granular permission language. Supports ACL, RBAC, and other access models. 

[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome) is a DNS relay station with ad/tracker/other blocking, IP address redirections, and DNS-over-HTTPS.

[NetBird](https://netbird.io/) is an open-source VPN management platform built on top of WireGuard® making it easy to create secure private networks for your organization or home.

[Supabase](https://github.com/supabase/supabase) is an open source Firebase alternative. It is building the features of Firebase using enterprise-grade open source tools.

[Plik](https://github.com/root-gg/plik) is a scalable & friendly temporary file upload system (Wetransfer like) in golang.

[Restify](https://github.com/restify/node-restify) is a framework, utilizing [connect](https://github.com/senchalabs/connect) style middleware for building REST APIs. 

[Traefik](https://traefik.io/traefik/) is an open source Edge Router that makes publishing your services a fun and easy experience. It receives requests on behalf of your system and finds out which components are responsible for handling them. What sets Traefik apart, besides its many features, is that it automatically discovers the right configuration for your services.

[Traefik Mesh](https://traefik.io/traefik-mesh) is a simple, yet full-featured service mesh. It is container-native and fits as your de-facto service mesh in your Kubernetes cluster. It supports the latest Service Mesh Interface specification [SMI](https://smi-spec.io/) that facilitates integration with pre-existing solution. 

[DuckDNS](https://www.duckdns.org/) is a free service that allows you to bind your own favorite subdomain under ```duckdns.org``` to the public IP address in use from your router, even though such address is dynamically allocated by your internet service provider and therefore changes over time.

[Trust-DNS](https://github.com/bluejekyll/trust-dns) is a Rust based DNS client, server, and Resolver, built to be safe and secure from the ground up.

[Hugo](https://github.com/gohugoio/hugo) is a static HTML and CSS website generator written in Go. It is optimized for speed, ease of use, and configurability. Hugo takes a directory with content and templates and renders them into a full HTML website.

[sshuttle](https://github.com/sshuttle/sshuttle) is a transparent proxy server that works as a poor man's VPN that forwards connection over ssh. It works with Linux and MacOS and supports DNS tunneling. 

[NetHopper](https://www.nethopper.io/) is a Multi-Cloud Application Network as a Service. The easiest way to visualize, connect, secure, protect, and monitor microservices across any cluster, site, cloud, or network.

[Cypress](https://cypress.io/) is a tool that makes it fast, easy and reliable testing for anything that runs in a browser. 

[Kimchi](https://github.com/kimchi-project/kimchi) is an HTML5 based management tool for KVM. It is designed to make it as easy as possible to get started with KVM and create your first guest.

[ION](https://github.com/pion/ion) is a distributed real-time communication system, the goal is to chat anydevice, anytime, anywhere.

[FreeRDP](https://github.com/FreeRDP/FreeRDP) is a free remote desktop protocol library and clients.

[Pimox](https://github.com/pimox/pimox7) is a port of Proxmox to the Raspberry Pi allowing you to build a Proxmox cluster of Rapberry Pi's or even a hybrid cluster of Pis and x86 hardware.

[PiKVM](https://github.com/pikvm/pikvm) is a very simple and fully functional Raspberry Pi-based KVM over IP.

[Firezone](https://firezone.dev/) is a self-hosted WireGuard®-based VPN server and Linux firewall.

[Monoid](https://github.com/monoid-privacy/monoid) is an open-source suite of tools for automating data privacy.

[Pinecone](https://matrix-org.github.io/pinecone/) is an experimental overlay routing protocol suite which is the foundation of the current P2P Matrix demos. It is designed to provide end-to-end encrypted connectivity between devices at a global scale over any compatible medium (currently TCP, WebSockets, Bluetooth Low Energy etc), allowing multi-hop peer-to-peer connectivity between devices even in places where there is no Internet connectivity. 

### Service Discovery

[Back to The Top](#table-of-contents)

[Consul](http://www.consul.io/)  is a tool for service discovery, monitoring and configuration. [Install Consul on Self-Hosted Kubernetes Clusters](https://github.com/hashicorp/consul/blob/main/website/content/docs/k8s/platforms/self-hosted-kubernetes.mdx).

[Linkerd](https://linkerd.io/) is an ultralight, security-first service mesh for Kubernetes. Linkerd adds critical security, observability, and reliability features to your Kubernetes stack with no code change required.

[Doozerd](https://github.com/ha/doozerd) is a highly-available, completely consistent store for small amounts of extremely important data.

[Admiral](https://github.com/istio-ecosystem/admiral) is a tool for for service discovery that provides automatic configuration and service discovery for multicluster Istio service mesh.

[ScaleCube](https://github.com/scalecube/scalecube-services) is a library that simplifies the development of reactive and distributed applications by providing an embeddable microservices library. It connects distributed microservices in a way that resembles a fabric when viewed collectively. It greatly simplifies and streamlines asynchronous programming and provides a tool-set for managing microservices architecture.

[DPS(dns-proxy-server)](https://github.com/mageddo/dns-proxy-server) is a lightweight end user (Developers, Server Administrators) DNS server tool for service discovery, which make it easy to develop in systems where one hostname can solve to different IPs based on the configured environment, so you can:

 * Solve hostnames from local configuration database.
 * Solve hostnames from docker containers using docker hostname option or HOSTNAMES env.
 * Solve hostnames from a list of configured remote DNS servers(as a proxy) if no answer of two above  .
 * Graphic interface to Create/List/Update/Delete A/CNAME records.
 * Solve host machine IP using host.docker hostname.
 * Access container by its container name / service name.
 * Specify from which network solve container IP.

[ZooKeeper](http://zookeeper.apache.org/)  is a centralized service for maintaining configuration information, naming, providing distributed synchronization, and providing group services.

### Security

[Back to The Top](#table-of-contents)

[Blackbox](https://github.com/StackExchange/blackbox) - Safely store secrets in Git/Mercurial. Provides tooling to automatically encrypt secrets like passwords.

[CrowdSec](https://github.com/crowdsecurity/crowdsec) - Locally scans log files and optionnaly requests, detecting and blocking malicious behaviors. AppSec capabilities to enable virtual-patching and turn your install into a WAF. Share attacks signals and benefit from real time blocklist of the most agressive IPs attacking CrowdSec's network.

[Denyhosts](http://denyhosts.sourceforge.net/) - Thwart SSH dictionary based attacks and brute force attacks.

[Fail2Ban](http://www.fail2ban.org/wiki/index.php/Main_Page) - Scans log files and takes action on IPs that show malicious behavior.

[fwknop](https://www.cipherdyne.org/fwknop/) - Protects ports via Single Packet Authorization in your firewall.

[Glastopf](http://glastopf.org/) - A low-interaction web application honeypot to emulate vulnerabilities and gather attack data.

[Kippo](https://github.com/desaster/kippo) - A medium-interaction SSH honeypot, mostly used as a standalone SSH daemon with a configurable Filesystem sandbox.
[OSSEC](http://ossec.net) - OSSEC is a HIDS that performs log analysis, FIM, rootkit detection, and much more.

[OSQuery](https://osquery.io/) - Query your servers status and info using a SQL like interface.

[OPNsense](https://opnsense.org/) is an open source firewall and routing software developed by Deciso. It offers an integrated Netflow analyser without the need for additional plugins or tools, similar to what you may find in high-end commercial products.

[pfSense](https://www.pfsense.org/) - Firewall and Router FreeBSD distribution.

[Snort](https://www.snort.org/) - Snort is a free and open source network intrusion prevention system (NIPS) and network intrusion detection system (NIDS) created by Martin Roesch in 1998.

[SpamAssassin](https://spamassassin.apache.org/) - A powerful and popular email spam filter employing a variety of detection technique.

[BounCA](https://bounca.org/) - is a personal SSL / Certificate Authority Key management tool. Create self-signed SSL certificates via your browser. 

### Troubleshooting

[Back to The Top](#table-of-contents)

[NETworkManager](https://github.com/BornToBeRoot/NETworkManager) - A powerful tool for managing networks and troubleshoot network problems. It contains features like a WiFi analyzer, IP scanner, port scanner, ping monitor, traceroute, DNS lookup or a LLDP/CDP capture. 

[Wireshark](https://www.wireshark.org/) - The world's foremost network protocol analyzer.

[Selfspy](https://github.com/selfspy/selfspy) is a daemon for Unix/X11, MacOS (thanks to @ljos) and Windows (thanks to @Foxboron), that continuously monitors and stores what you are doing on your computer. This way, you can get all sorts of nifty statistics and reminders on what you have been up to.

[Cilium](https://github.com/cilium/cilium) - A networking, observability, and security solution with an eBPF-based dataplane. It provides a simple flat Layer 3 network with the ability to span multiple clusters in either a native routing or overlay mode.

[Netshoot](https://github.com/nicolaka/netshoot) - A  Docker + Kubernetes network trouble-shooting swiss-army container.

[Kubevious](https://kubevious.io/) - A suite of app-centric assurance, validation, and introspection products for Kubernetes. It helps running modern Kubernetes applications without disasters and costly outages by continuously validating application manifests, cluster state, and configuration. 

[HOMER](https://github.com/sipcapture/homer) - A robust, carrier-grade, scalable Packet and Event capture system and VoiP/RTC Monitoring Application based on the HEP/EEP protocol and ready to process & store insane amounts of signaling, rtc events, logs and statistics with instant search, end-to-end analysis and drill-down capabilities.

[mitmproxy](https://mitmproxy.org/) - A Python tool used for intercepting, viewing and modifying network traffic. Invaluable in troubleshooting certain problems.

[Sysdig](https://www.sysdig.org/) - Capture system state and activity from a running Linux instance, then save, filter and analyze.

[Sysdig Inspect](https://github.com/draios/sysdig-inspect) - A powerful opensource interface for container troubleshooting and security investigation.

### Monitoring

[Back to the Top](#table-of-contents)

[Proxmox Mail Gateway](https://www.proxmox.com/en/proxmox-mail-gateway) is an open-source email security solution protecting your mail server against all email threats from the moment they emerge. 

[M2MLabs MainSpring](http://www.m2mlabs.com/) is an application framework for building machine-to-machine applications like vehicle tracking or machine remote monitoring. In such applications typically a remote device equipped with sensors (e.g. gps, temperature, pressure) and actors communicates with a server application that is running the device communication protocol, device configuration, storage of data sent by the devices as well as the application business logic and the presentation layer. 

[VictoriaMetrics](https://victoriametrics.com/) is a fast and scalable open source time series database and monitoring solution which exists in a Single and in a cluster version. It is compatible with Prometheus pull model and supports a [wide variety of ingestion protocols](https://docs.victoriametrics.com/#prominent-features): Influx, Graphite, Prometheus remote_write, Prometheus exposion format, OpenTSDB put message, JSON line format, Arbitrary CSV data, native binary formant, DataDog agent or DogStatsD; as way as many ways to query data via PromQL or [MetricsQL](https://docs.victoriametrics.com/MetricsQL.html) from Grafana or own [VMUI](https://docs.victoriametrics.com/Single-server-VictoriaMetrics.html#vmui).

[Kestra](https://github.com/kestra-io/kestra) is an infinitely scalable orchestration and scheduling platform, creating, running, scheduling, and monitoring millions of complex pipelines. 

[InfluxDB](https://www.influxdata.com) is an open source time series database, purpose-built by InfluxData for monitoring metrics and events, provides real-time visibility into stacks, sensors, and systems. Use InfluxDB to capture, analyze, and store millions of points per second, meet demanding SLA's, and chart a path to automation.

[Grafana](https://grafana.com/oss/grafana/) is a tool that allows you to query, visualize, alert on and understand your metrics no matter where they are stored. 

[Prometheus](https://prometheus.io/) is a free software application used for event monitoring and alerting. It records real-time metrics in a time series database (allowing for high dimensionality) built using a HTTP pull model, with flexible queries and real-time alerting.

[Loki](https://grafana.com/oss/loki/) is a horizontally-scalable, highly-available, multi-tenant log aggregation system inspired by Prometheus. It is designed to be very cost effective and easy to operate. It does not index the contents of the logs, but rather a set of labels for each log stream.

[Thanos](https://thanos.io/) is a set of components that can be composed into a highly available metric system with unlimited storage capacity, which can be added seamlessly on top of existing Prometheus deployments.

[Wyze](https://wyze.com/) is a great security and monitoring application to live stream HD video from the security cameras from anywhere in the world. 

[Uptime Kuma](https://uptime.kuma.pet/) is a fancy self-hosted monitoring tool.

[Gatus](https://gatus.io/) is a developer-oriented health dashboard that gives you the ability to monitor your services using HTTP, ICMP, TCP, and even DNS queries as well as evaluate the result of said queries by using a list of conditions on values like the status code, the response time, the certificate expiration, the body and many others. 

[Upptime](https://upptime.js.org) is the open-source uptime monitor and status page, powered entirely by GitHub Actions, Issues, and Pages.

[HertzBeat](https://github.com/dromara/hertzbeat) is an open-source, real-time monitoring system with custom-monitor and agentless. It supports web service, database, os, middleware and more.

[Tautulli](https://tautulli.com/) is a python based web application for monitoring, analytics and notifications for [Plex Media Server](https://plex.tv/).

[Flower](https://flower.readthedocs.io/) is a web based tool for monitoring and administrating Celery clusters.

[Weave Scope](https://www.weave.works/oss/scope/) is a tool for Troubleshooting & Monitoring for Docker & Kubernetes. It automatically generates a map of your application, enabling you to intuitively understand, monitor, and control your containerized, microservices-based application.

[Statping (Status Page & Monitoring Server)](https://github.com/statping/statping) is an easy to use Status Page for your websites and applications. Statping will automatically fetch the application and render a beautiful status page with tons of features for you to build an even better status page.

[Vector](https://vector.dev/) is a high-performance, end-to-end (agent & aggregator) observability data pipeline that puts you in control of your observability data. [Collect](https://vector.dev/docs/reference/configuration/sources/), [transform](https://vector.dev/docs/reference/configuration/transforms/), and [route](https://vector.dev/docs/reference/configuration/sinks/) all your logs, metrics, and traces to any vendors you want today and any other vendors you may want tomorrow.

[Open Service Mesh (OSM)](https://openservicemesh.io/) is a lightweight, extensible, cloud native service mesh that allows users to uniformly manage, secure, and get out-of-the-box observability features for highly dynamic microservice environments. 

[Ciao](https://github.com/brotandgames/ciao) is a tool that checks HTTP(S) URL endpoints for a HTTP status code (or errors on the lower TCP stack) and sends a notification on status change via E-Mail or Webhooks.

[Server](https://gotify.net/) is a simple server for sending and receiving messages in real-time per WebSocket. 

[Ngxtop](https://github.com/lebinh/ngxtop) is a real-time metrics for nginx server (and others).

[Blocky](https://github.com/0xERR0R/blocky) is a fast and lightweight DNS proxy as ad-blocker for local network with many features 

[Dashy](https://dashy.to/) is a self-hostable personal dashboard built for you. Includes status-checking, widgets, themes, icon packs, a UI editor and tons more.

[Netdata](https://github.com/netdata/netdata) is high-fidelity infrastructure monitoring and troubleshooting, real-time monitoring Agent collects thousands of metrics from systems, hardware, containers, and applications with zero configuration. It runs permanently on all your physical/virtual servers, containers, cloud deployments, and edge/IoT devices, and is perfectly safe to install on your systems mid-incident without any preparation.

[Restic](https://restic.net/) is a modern backup program that can back up your files: from Linux, BSD, Mac and Windows. To many different storage types, including self-hosted and online services. easily, being a single executable that you can run without a server or complex setup. effectively, only transferring the parts that actually changed in the files you back up.

[Autorestic](https://github.com/cupcakearmy/autorestic) is a wrapper around the amazing restic. While being amazing the restic cli can be a bit overwhelming and difficult to manage if you have many different locations that you want to backup to multiple locations. 

[MinIO](https://min.io/) is a high performance object storage tool that provides the world's fastest object storage server. With READ/WRITE speeds of 325 GiB/s and 165 GiB/s on standard hardware with default parity (EC:4), object storage can operate as the primary storage tier for a diverse set of workloads ranging from Spark, Presto, TensorFlow.

[Greyhole](https://www.greyhole.net/) is a tool that uses Samba to create a storage pool of all your available hard drives (whatever their size, however they are connected), and allows you to create redundant copies of the files you store, in order to prevent data loss when part of your hardware fails.

[Falcon LogScale](https://www.crowdstrike.com/products/observability/falcon-logscale/) is purpose-built to help any organization achieve the benefits of large-scale logging and analysis. Falcon LogScale has virtually no latency, even at ingest volumes of 1PB(Petabyte) per day. 

[Googerteller](https://github.com/berthubert/googerteller) is a tool that makes an audible sound any time your computer sends a packet to a Google tracker or a Google service, which excludes Google Cloud users.

[TeslaMate](https://docs.teslamate.org/) is a powerful, self-hosted data logger for your Tesla.

[OneUptime](https://oneuptime.com/) is an open-source complete SRE and DevOps platform. It monitors your website, dashboards, API's, and more and alerts your team when downtime happens. 

[Parca](https://parca.dev/) is a tool for continuous profiling for analysis of CPU and memory usage, down to the line number and throughout time. Saving infrastructure cost, improving performance, and increasing reliability.

[DeviceHive](https://www.devicehive.com) is a free, highly scalable open-source IoT platform for data collection, processing and analysis, visualization, and device management with the broad range of integration options.

[Distributed Services Architecture (DSA)](https://github.com/IOT-DSA) is an open source IoT platform that facilitates device inter-communication, logic and applications at every layer of the Internet of Things infrastructure. The objective is to unify the disparate devices, services and applications into a structured and adaptable real-time data model.

[IoTivity](https://iotivity.org) is an open source software framework enabling seamless device-to-device connectivity to address the emerging needs of the Internet of Things. 

[Eclipse IoT Project](https://projects.eclipse.org/projects/iot) provides open source technology that will be used to build IoT solutions for industry and consumers.

### Dashboards

[Back to The Top](#table-of-contents)

[Adagios](http://adagios.org/) is a Web based Nagios configuration interface.

[Dash](https://github.com/afaqurk/linux-dash) is a low-overhead monitoring web dashboard for a GNU/Linux machine.

[Thruk](http://www.thruk.org/) is a Multibackend monitoring web interface with support for Naemon, Nagios, Icinga and Shinken.

[Uchiwa](https://uchiwa.io) is a simple dashboard for the Sensu monitoring framework.

[InfluxDB](https://www.influxdata.com) is an open source time series database, purpose-built by InfluxData for monitoring metrics and events, provides real-time visibility into stacks, sensors, and systems. Use InfluxDB to capture, analyze, and store millions of points per second, meet demanding SLA's, and chart a path to automation.

[Grafana](https://grafana.com/oss/grafana/) is a tool that allows you to query, visualize, alert on and understand your metrics no matter where they are stored. 

[Prometheus](https://prometheus.io/) is a free software application used for event monitoring and alerting. It records real-time metrics in a time series database (allowing for high dimensionality) built using a HTTP pull model, with flexible queries and real-time alerting.


### Analytics

[Back to the Top](#table-of-contents)

[Plausible Analytics](https://plausible.io/) - Simple, open-source, lightweight (< 1 KB) and privacy-friendly web analytics.

[PostHog](https://posthog.com) - Product analytics, session recording, feature flagging and a/b testing that you can self-host. 

[Ackee](https://ackee.electerious.com) - Self-hosted analytics tool for those who care about privacy. 

[AWStats](http://www.awstats.org/) - Generate statistics from web, streaming, ftp or mail server logfiles. 

[Chartbrew](https://chartbrew.com) - Web application that can connect directly to databases and APIs and use the data to create beautiful charts. 

[Countly Community Edition](https://count.ly) - Real time mobile and web analytics, crash reporting and push notifications platform.

[Druid](http://druid.io/) - Distributed, column-oriented, real-time analytics data store. 

[EDA](https://eda.jortilles.com/en/jortilles-english/) - Web application for data analysis and visualization. 

[GoAccess](http://goaccess.io/) - Real-time web log analyzer and interactive viewer that runs in a terminal. 

[GoatCounter](https://www.goatcounter.com) - Easy web statistics without tracking of personal data. 

[Metabase](https://metabase.com/) - Easy, open-source way for everyone in your company to ask questions and learn from data. 

[Offen](https://www.offen.dev/) - Fair, lightweight and open web analytics tool. Gain insights while your users have full access to their data. 

[Open Web Analytics](http://www.openwebanalytics.com/) - Web analytics framework that lets you stay in control of how you instrument and analyze the use of your websites and applications. 

[Redash](http://redash.io) - Connect and query your data sources, build dashboards to visualize data and share them with your company. 

[RudderStack](https://rudderstack.com/) - Collect, unify, transform, and store your customer data, and route it to a wide range of common, popular marketing, sales, and product tools. alternative to Segment.

[Shynet](https://github.com/milesmcc/shynet) - Modern, privacy-friendly, and detailed web analytics that works without cookies or JS. 

[Superset](http://superset.apache.org/) - Modern data exploration and visualization platform. 

[Umami](https://umami.is/) - Simple, fast, privacy-focused alternative to Google Analytics.


### Search

[Back to the Top](#table-of-contents)

[Meilisearch](https://github.com/meilisearch/meilisearch) is a lightning-fast search engine that fits effortlessly into your apps, websites, and workflow. 

[Shodan](https://www.shodan.io/) is the world's first search engine for Internet-connected (IoT) devices.

[Whoogle Search](https://github.com/benbusby/whoogle-search) is a self-hosted, ad-free, privacy-respecting metasearch engine.

[SearX](https://github.com/searx/searx) is a Privacy-respecting, hackable [metasearch engine](https://en.wikipedia.org/wiki/Metasearch_engine).

[SearXNG](https://github.com/searxng/searxng) is a free internet metasearch engine which aggregates results from various search services and databases. 

[Sonic](https://github.com/valeriansaliou/sonic) is a fast, lightweight & schema-less search backend. An alternative to Elasticsearch that runs on a few MBs of RAM. 

[Zinc](https://github.com/zinclabs/zinc) is a search engine that does full text indexing. It is a lightweight alternative to Elasticsearch and runs using a fraction of the resources. 

[Cylect.io](https://cylect.io/) is the ultimate searching tool that is here to assist anyone looking for specific information through vast amounts of websites, search engines, and data collectors. 

[Lyra](https://docs.lyrasearch.io/) is a fast, in-memory, typo-tolerant, full-text search engine written in TypeScript. 

[Hugo Lyra](https://github.com/paolomainardi/hugo-lyra) is a  typescript module for creating LyraSearch indexes for static Hugo sites, it comes with server and client libraries. 

[Typesense](https://github.com/typesense/typesense) is a fast, typo-tolerant search engine for building delightful search experiences. 

[Tantivy](https://github.com/quickwit-oss/tantivy) is a full-text search engine library inspired by Apache Lucene and written in Rust.

[Toshi](https://github.com/toshi-search/Toshi) is meant to be a full-text search engine similar to Elasticsearch. Toshi strives to be to Elasticsearch what [Tantivy](https://github.com/tantivy-search/tantivy) is to Lucene.

[FlexSearch](https://github.com/nextapps-de/flexsearch) is a Next-Generation full text search library for Browser and Node.js.

[fd](https://github.com/sharkdp/fd) is a program to find entries in your filesystem. It is a simple, fast and user-friendly alternative to find. 

[k8s at home search](https://nanne.dev/k8s-at-home-search/#/) is a tool that indexs Flux HelmReleases from Github repositories with the ```k8s-at-home topic``` on GitHub. 

[OpenFind](https://open.getfind.app/) is an app to find text in real life. Easily search your entire photo library in split seconds. This runs 100% offline. No servers, nothing weird going on.

### Notifications

[Back to the Top](#table-of-contents)

[Apprise](https://github.com/caronc/apprise) is a tool that allows you to send a notification to almost all of the most popular notification services available to us today such as: Telegram, Discord, Slack, Amazon SNS, Gotify, etc.

[ntfy](https://ntfy.sh/) is a simple HTTP-based pub-sub notification service. It allows you to send notifications to your phone or desktop via scripts from any computer, entirely without signup, cost or setup. It's also open source if you want to run your own.

[Countly](https://github.com/Countly/countly-server) is a product analytics solution and innovation enabler that helps teams track product performance and customer journey and behavior across mobile, web, and desktop applications. [Ensuring privacy by design](https://count.ly/your-data-your-rules), Countly allows you to innovate and enhance your products to provide personalized and customized customer experiences, and meet key business and revenue goals.

[notifiers](https://github.com/liiight/notifiers) is a general wrapper for a variety of 3rd party providers and built in ones (like SMTP) aimed solely at sending notifications.

[Pushover](https://pushover.net/) is a tool that makes it easy to get real-time notifications on your Android, Android Wear, iPhone, iPad, Apple Watch and Desktop.

[Simplepush](https://simplepush.io/) is a tool to send end-to-end encrypted push notifications to your Android and iPhone.

[UnifiedPush](https://unifiedpush.org/) is a set of specifications and tools that lets the user choose how push notifications are delivered. All in a free and open source way.

### RSS

[Back to the Top](#table-of-contents)

[RSS Guard](https://github.com/martinrotter/rssguard) is a simple RSS/ATOM feed reader for Windows, Linux, BSD, OS/2 or macOS which can work with RSS/ATOM/JSON feeds as well as many online feed services:

  * [Feedly](https://feedly.com/)
  * [Gmail](https://developers.google.com/gmail/api)
  * Google Reader API ([Bazqux](https://bazqux.com/), [FreshRSS](https://freshrss.org/), [Inoreader](https://www.inoreader.com/), [Miniflux](https://miniflux.app/), [Reedah](http://reedah.com/), [The Old Reader](https://theoldreader.com/) and more)
  * [Nextcloud News](https://apps.nextcloud.com/apps/news)
  * [Tiny Tiny RSS](https://tt-rss.org/)

[Feedly](https://feedly.com/) is an RSS tool where you can privately organize and research the topics and trends that matter to you. It offers useful integrations with Facebook, Twitter, Evernote, Buffer, OneNote, Pinterest, LinkedIn, IFTTT, and Zapier so that you can easily share stories with your networks and teammates.

[FreshRSS](https://www.freshrss.org/) is a self-hosted RSS and Atom feed aggregator. It is lightweight, easy to work with, powerful, and customizable.

[ArchiveBox](https://archivebox.io/) is a powerful, self-hosted internet archiving solution to collect, save, and view sites you want to preserve offline. It takes URLs/browser history/bookmarks/Pocket/Pinboard/etc., saves HTML, JS, PDFs, media, and more.

[RSSHub](https://github.com/DIYgod/RSSHub) is an open source, easy to use, and extensible RSS feed generator. It's capable of generating RSS feeds from pretty much everything.

[Miniflux V2](https://github.com/miniflux/v2) is a minimalist and opinionated feed reader.

### Websites/Blogs

[Back to the Top](#table-of-contents)

[Hugo](https://github.com/gohugoio/hugo) is a static HTML and CSS website generator written in Go. It is optimized for speed, ease of use, and configurability. Hugo takes a directory with content and templates and renders them into a full HTML website.

[Lyra](https://docs.lyrasearch.io/) is a fast, in-memory, typo-tolerant, full-text search engine written in TypeScript. 

[Hugo Lyra](https://github.com/paolomainardi/hugo-lyra) is a  typescript module for creating LyraSearch indexes for static Hugo sites, it comes with server and client libraries. 

[Kopage](https://www.kopage.com/) is  a self-hosted Website Builder. It's compatible with cPanel and other popular hosting control panels. Compatible with cPanel and other popular hosting control panels.

[Ghost](https://ghost.org/docs/hosting/) is a fully-managed PaaS & self-hosted open source software, and can be installed and maintained relatively easily on just about any VPS hosting provider.

[Cloudron](https://www.cloudron.io/) is a self-hosted immutable infrastructure design allows easy migration of apps across servers. In fact, you can move your entire server along with all its apps to another cloud provider in no time.

[Directus](https://directus.io/) is a real-time API and App dashboard for managing SQL database content.

[Haven](https://havenweb.org/) is a Self-hosted private blog instead of using Facebook.

[Antville](https://antville.org/) is an open source project aimed at the development of a simple site hosting system with many advanced [features](https://github.com/antville/antville/wiki/Features). 

[October](https://octobercms.com/) is a Self-hosted Content Management System (CMS) and web platform whose sole purpose is to make your development workflow simple again. 

[Grav](https://getgrav.org/) is a Fast, Simple, and Flexible, file-based Web-platform. There is Zero installation required. Just extract the ZIP archive, and you are already up and running. It comes with a powerful Package Management System to allow for simple installation and upgrading of plugins and themes, as well as simple updating of Grav itself.

[Orchard](https://github.com/OrchardCMS/Orchard) is a free, open source, community-focused Content Management System built on the ASP.NET MVC platform.

[Netlify CMS](https://www.netlifycms.org/) is a CMS for static site generators. Give users a simple way to edit and add content to any site built with a static site generator.

[Zola](https://www.getzola.org/) is a fast static site generator in a single binary with everything built-in. 

[FlatPress](https://www.flatpress.org/) is a lightweight, easy-to-set-up blogging engine. 

[Chyrp Lite](https://chyrplite.net/) is an ultra-lightweight blogging engine. It provides four beautiful blog themes and a friendly administration console, all fully navigable on a broad range of devices, thanks to the power of responsive HTML5. 

[WriteFreely](https://writefreely.org/) is an open source platform for building a writing space on the web.

[Sandstorm](https://sandstorm.io/) is an open source project built by a community of volunteers with the goal of making it really easy to run open source web applications.

[YunoHost](https://yunohost.org/) is a Debian-based distribution which strives to make it easy to quickly set up a server and host web applications.


### Social

[Back to the Top](#table-of-contents)

[Mattermost](https://mattermost.com/) is a secure, open source platform for communication, collaboration, and workflow orchestration across tools and teams.

[Mastadon](https://joinmastodon.org/) is a a decentralized social media platform that supports audio, video and picture posts, accessibility descriptions, polls, content warnings, animated avatars, custom emojis, thumbnail crop control, and more, to help you express yourself online.

[Telegram](https://telegram.org/) is a cross-platform, cloud-based instant messaging service. It has an open API and source code free for everyone. Telegram also provides end-to-end encrypted video calling, VoIP, file sharing and several other features.

[ActivityPub](https://activitypub.rocks/) is a decentralized social networking protocol based on the ActivityStreams 2.0 data format. It provides a client to server API for creating, updating and deleting content, as well as a federated server to server API for delivering notifications and subscribing to content.

[Lemmy](https://github.com/LemmyNet/lemmy) is similar to sites like Reddit, Lobste.rs, or Hacker News. Where you subscribe to forums you're interested in, post links and discussions, then vote, and comment on them. Behind the scenes, it is very different; anyone can easily run a server, and all these servers are federated, and connected to the same universe, called the Fediverse.

[Lemmy-UI](https://github.com/LemmyNet/lemmy-ui) is the official web app for [Lemmy](https://github.com/LemmyNet/lemmy), written in inferno.

[Mlem](https://github.com/buresdv/Mlem) is a Lemmy client for iOS.

[Jerboa](https://github.com/dessalines/jerboa) is an Android client for Lemmy, a federated reddit alternative.

[GoToSocial](https://gotosocial.org/) is an [ActivityPub](https://activitypub.rocks/) social network server, written in Golang.

[Berty](https://github.com/berty/berty) is a secure peer-to-peer messaging app that works with or without internet access, cellular data or trust in the network.

[Pleroma](https://pleroma.social/) is a free and open communication for everyone. Pleroma is social networking software compatible with other Fediverse software such as Misskey, Pixelfed, Mastodon and many others. 

[Matrix](https://matrix.org/) is a tool that gives you simple HTTP APIs and SDKs (iOS, Android, Web) to create chatrooms, direct chats and chat bots, complete with end-to-end encryption, file transfer, synchronised conversation history, formatted messages, read receipts and more.

[Element](https://element.io/) is a Matrix web client built using the [Matrix React SDK](https://github.com/matrix-org/matrix-react-sdk).

[Nostr(Notes and Other Stuff Transmitted by Relays)](https://github.com/nostr-protocol/nostr) is a truly censorship-resistant alternative to Twitter that has a chance of working.

[Fritter](https://fritter.cc/) is an open source frontend for Twitter on mobile devices, focusing on giving you the best experience and keeping your data private, local and in your hands. 

[Nitter](https://github.com/zedeus/nitter) is a free and open source alternative Twitter front-end focused on privacy and performance. All requests go through the backend, meaning the client never talks to Twitter and prevents Twitter from tracking your IP or JavaScript fingerprint.

[Diaspora](https://diasporafoundation.org/) is a privacy-aware, distributed, open source social network.

[Hubzilla](https://framagit.org/hubzilla/core) is a general purpose communication server integrated with a web publishing system and a decentralised permission system.

[Expanse](https://github.com/jc9108/expanse) is a fully selfhosted multi-user web app for externally storing Reddit items (saved, created, upvoted, downvoted, hidden) to bypass Reddit's 1000-item listing limits.

[Apollo](https://apolloapp.io/) is a beautiful Reddit app built for fast navigation with an incredibly powerful set of features.  

[Infinity](https://github.com/Docile-Alligator/Infinity-For-Reddit) is a Reddit client on Android written in Java. It does not have any ads and it features a clean UI and smooth browsing experience.

[RedReader](https://github.com/QuantumBadger/RedReader) is an unofficial open source Reddit client for Android. 


### Nostr

[Back to the Top](#table-of-contents)

**[Nostr (Notes and Other Stuff Transmitted by Relays)](https://nostr.com/)** is a protocol, designed for simplicity, that aims to create a censorship-resistant global social network. The protocol is based on very simple & flexible event objects (which are passed around as plain JSON) and uses standard elliptic-curve cryptography for keys and signing. 

- [nostr](https://github.com/nostr-protocol/nostr) - overview and FAQ.
- [NIPs](https://github.com/nostr-protocol/nips) - the "**N**ostr **I**mplementation **P**ossibilities" describe the protocol in technical detail.
- [nostr, a basic tour](https://github.com/rajarshimaitra/rust-nostr/blob/main/VISION.md) - an intro to nostr.
- [UseNostr](https://usenostr.org) - A small guide for anyone who wants to learn more about how nostr works and what it can do.
- [nostr.how](https://nostr.how) - Quick-start to onboard desktop users with Alby & Astral.
- [nostr.guide](https://nostr.guide) - A guide to all things nostr.
- [nostr address book](https://github.com/aitechguy/nostr-address-book) - A directory of twitter users accounts and their NOSTR addresses.
- [NNostr](https://github.com/Kukks/NNostr) - a C# relay.
- [nostr-rs-relay](https://sr.ht/~gheartsfield/nostr-rs-relay/) - a minimalistic relay written in Rust that saves data on SQLite.
- [Relayer Basic](https://github.com/fiatjaf/relayer/tree/master/basic) - a simple relay based on _relayer_ backed by Postgres.
- [nodestr](https://github.com/Dolu89/nodestr-relay) - a Node.js implementation.
- [sovereign-stack](https://www.sovereign-stack.org) - a tool that helps you deploy nostr relays and create self-hosted (bitcoin-only) Value4Value websites.
- [expensive relay](https://github.com/fiatjaf/expensive-relay) - a relay that requires payment for registration
- [me.untethr.nostr-relay](https://github.com/atdixon/me.untethr.nostr-relay) - a relay written in Clojure
- [Minds Nostr Relay](https://gitlab.com/minds/infrastructure/nostr-relay) - a relay for [Minds](https://www.minds.com), an open-source social network
  - [Minds Engine - Nostr](https://gitlab.com/minds/engine/-/tree/master/Core/Nostr) - relevant Minds API code for reading/writing Minds posts using Nostr
- [NostrPostr Relay](https://github.com/Giszmo/NostrPostr/tree/master/NostrRelay) - a Kotlin Relay supporting both SQLite and Postgresql
- [nostrpy](https://github.com/monty888/nostrpy) - relay, client, and other tooling in python
- [nostream](https://github.com/Cameri/nostream) - a nostr relay written in Typescript backed by PostgreSQL (renamed from nostr-ts-relay)
- [nostr_relay](https://code.pobblelabs.org/fossil/nostr_relay/) – a nostr relay written in python, backed by SQLite
- [søstr](https://github.com/metasikander/s0str) – a private nostr relay written in rust, saves all notes from one pubkey and publish them to anyone that requests them
- [knostr](https://github.com/lpicanco/knostr) – a nostr relay implemented in Kotlin with support for Postgres and metrics(micrometer).
- [PyRelay](https://github.com/johnny423/pyrelay) – a python implementation of a nostr relay, using asyncio.
- [strfry](https://github.com/hoytech/strfry) – C++ implementation backed by LMDB with efficient syncing of events using merkle trees
- [Astro](https://github.com/Nostrology/astro) – Elixir based implementation built to be performant and highly distributed.
- [Nex](https://github.com/lebrunel/nex) - A powerful and scalable Nostr relay written in Elixir with Postgres DB.
- [gnost-relay](https://github.com/barkyq/gnost-relay) - nostr relay written in go backed by postgresql database.
- [nostring](https://github.com/xbol0/nostring) - A Nostr relay written in Deno.
- [Denostr](https://github.com/guakamoli/denostr) - Deno based, cloud native nostr implemention support by ByteTrade and Revo.
- [nostr-relay-nestjs](https://github.com/CodyTseng/nostr-relay-nestjs)- A Nostr relay implemented using the NestJS framework
- [Ephemerelay](https://gitlab.com/soapbox-pub/ephemerelay) - An in-memory Nostr relay that doesn't store data.
- [Servus](https://github.com/ibz/servus) - A self-contained, single executable, CMS / blogging engine reminiscent of Jekyll which also acts as a personal Nostr relay for your blog posts. Written in Rust.
- [nostr relay registry](https://nostr-registry.netlify.app/) - real-time checking of status of some known relays.
- [nostr.info](https://nostr.info/) - real-time checking of status of some known relays.
- [nostr.watch](https://nostr.watch) - real-time checking of status of some known relays.
- [Astral](https://github.com/monlovesmango/astral) - a branle fork with global feed and UI makeover
- [damus](https://github.com/damus-io/damus) - a twitter-like nostr client for iOS and MacOS.
- [more-speech](https://github.com/unclebob/more-speech) - desktop client for nostr written in Clojure.
- [futr](https://github.com/prolic/futr) - nostr client desktop app written in Haskell.
- [Minds](https://www.minds.com/) - open source social network. Supports reading and creating posts using the Nostr protocol.
- [Jester](https://github.com/jesterui/jesterui)  - Chess over nostr.
  - [Jester instance](https://jesterui.github.io/)
- [Sendstr](https://sendstr.com/) - shared clipboard between devices over nostr.
- [nosbin](https://nosbin.com/) - pastebin over nostr.
- [noscl](https://github.com/fiatjaf/noscl) - a basic command-line client written in Go.
- [loquaz](https://github.com/emeceve/loquaz) - a desktop app written in Rust for direct encrypted chat.
- [nostr console](https://github.com/vishalxl/nostr_console) - a nostr command line client written in Dart. Binaries available for Windows, Linux, and MacOS.
- [ArcadeCity](https://github.com/ArcadeCity/app) - Public group chats and P2P services (WIP) over nostr.
- [second exchange](https://github.com/cynsar-foundation/second.exchange) - an experiment to work out something of like medium, something of creator economy where users are rewarded for engaging in quality discussion and most importantly engaging in governance-related discussion.
- [scalastr](https://github.com/benthecarman/scalastr) - A barebones nostr client written in scala.
- [Nostros](https://github.com/KoalaSat/nostros) - A nostr mobile client for Android.
- [Nostrify.me](https://github.com/lightningorb/nostrify.me) - Nostr client built in SvelteKit.
- [NostrEmitter](https://github.com/cmdruid/nostr-emitter) - Simple E2E encrypted client and EventEmitter object
- [Lightning.Pub](https://github.com/shocknet/Lightning.Pub) - A nostr daemon for Lightning nodes.
- [shockwallet](https://github.com/shocknet/wallet2) - A Lightning wallet that uses nostr and lnurl to connect to nodes.
- [coracle](https://github.com/staab/coracle) - A nostr web client.
- [nostrweb](https://git.qcode.ch/nostr/nostrweb) - another nostr web client in vanilla JS.
  - [nostr.ch](https://nostr.ch/) - live instance
- [Bija](https://github.com/BrightonBTC/bija) - A desktop client written in python. Currently Linux only.
- [Nosky](https://github.com/KotlinGeekDev/Nosky) - A native Android client for Nostr. Still in development.
- [Stackerstan](https://stackerstan.org) - A decentralised organisation built on Bitcoin and Nostr, implemented as a replicated state machine in Golang.
- [nostr-java](https://github.com/tcheeric/nostr-java) - A nostr client API written in java, for generating, signing and publishing events to relays.
- [bolt.fun](https://makers.bolt.fun/feed) - A bitcoin lightning makers community that supports reading and creating comments using Nostr.
- [iris](https://github.com/irislib/iris-messenger) - A nostr web client.
  - [iris.to](https://iris.to) - live instance
  - [Android app](https://play.google.com/store/apps/details?id=to.iris.twa)
- [gossip](https://github.com/mikedilger/gossip) - A desktop client in rust presented with egui.
- [Attached](https://github.com/dyegolara/nostr-attached) - Open-Source ReactNative Expo app for Nostr (iOS, Android). Currently under app stores review.
- [Member](https://github.com/memberapp/memberapp.github.io) - Progressive Web App Client. Works on desktop and mobile.
  - [member.cash](https://member.cash/) - live instance
- [dispute](https://github.com/ethicnology/dispute) - A cross-platform (Linux, Android, iOS, MacOs, Windows and Web) client for NOSTR
- [Snort](https://github.com/v0l/snort) - Nostr UI written in react
- [Hamstr](https://github.com/styppo/hamstr) - A twitter-style web client built with Vue.js
- [Nozzle](https://github.com/kaiwolfram/Nozzle) - A Twitter-like native Android client written with Jetpack Compose
- [electron-nostr](https://github.com/wds4/electron-react-boilerplate-nostr) - A bare-bones desktop nostr client using electron-react-boilerplate. Goal is to be an easy template for people to experiment with different ideas on decentralized ratings, reputation, and web of trust.
- [Nostrid](https://github.com/lapulpeta/Nostrid) - Multi-platform client currently offering binaries for Android, Windows, MacOS and Linux.
  - [Nostrid.Web](https://web.nostrid.app/) - Web version running completely on the browser. It can be installed locally as PWA.
- [nostr-chat-widget-react](https://www.npmjs.com/package/nostr-chat-widget-react?activeTab=readme) - A React component that provides a live-chat widget over nostr that can be embedded into any website.
- [Blockcore Notes](https://github.com/block-core/blockcore-notes)  - Progressive Web App that can be installed on mobile and desktop, organize following in circles and have both public and private following lists. Dynamic interface for different uses, such as optimized for photograph viewing.
- [Noteon](https://github.com/ShawnCN/cinny_nostsr2/tree/dev)- Yet another nostr client focused on private chat and group chat with a simple, elegant and secure interface.
- [emon](https://github.com/sebastiaanwouters/emon) - Encrypted DMs over nostr with lightning payments integrated (WIP).
- [notebin.org](https://notebin.org) - Nostr UI created with NextJS, support for markdown and code highlighting.
- [Daisy](https://github.com/neb-b/daisy) - Mobile client for Android and iOS.
- [Flycat](https://github.com/digi-monkey/flycat-web) - A 2000s old-school style web client which support blogging on Nostr.
- [Amethyst](https://github.com/vitorpamplona/amethyst) - An Android client for nostr written in Kotlin.
- [MeShell](https://github.com/BEEBSDONE/MeShell_Nodejs) - Web, iOS and Android blog type client destined to publish articles and researches for independent journalists.
- [Disgus](https://github.com/carlitoplatanito/disgus) - A comment widget like Disqus, but for Nostr.
- [Tamga](https://github.com/erdaltoprak/tamga) - An offline first nostr contact & profile manager for iOS!
- [nostromat](https://github.com/ekimber/nostromat)- A Twitter-style Nostr web client, written in Clojurescript/React.
- [nostrom.at](https://nostrom.at) - live instance.
- [blogstack.io](https://blogstack.io) - Blogging site for nostr, supports markdown.
- [Votestr](https://votestr.com/) - Poll web app with nostr authentication and blind signature unlinkability.
- [gnost-deflate-client](https://github.com/barkyq/gnost-deflate-client)- A CLI nostr client written in go implementing permessage-deflate websocket compression.
- [algia](https://github.com/mattn/algia) - A cli application for nostr.
- [algia-web](https://github.com/ryogrid/algia-web) - A small resource consumption oriented Nostr web client.
- [Blowater](https://blowater.deno.dev) - A desktop Web client focusing on chat with delightful UX.
- [Written](https://github.com/silencesoft/written) Self hosted blog using nostr long-form content (NIP-23) and it shows only posts by selected authors.
- [Nostr Nests](https://nostrnests.com/) - Nostr Nests is an audio space for chatting, brainstorming, debating, jamming, micro-conferences and more.
- [nblog](https://github.com/jacany/nblog) - a self-host nostr ghost blog
- [Nostribe.com](https://github.com/sepehr-safari/nostribe-web-client) - Nostr client web app built with Next.js 13 and TypeScript.
  - [Nostribe.com](https://nostribe.com/) - Live instance.
- [Nostrtium](https://github.com/pjv/nostrtium) - Post to Nostr directly from within WordPress
- [uBlog](https://github.com/nodetec/ublog) - A minimalist blog on nostr that allows anyone to easily create their own personal micro-blog.
- [Listr](https://github.com/sepehr-safari/listr) - A Nostr Web Client for Making Lists, built with Next.js 13 and TypeScript.  
- [nostr-ruby](https://github.com/dtonon/nostr-ruby) - a Ruby implementation of the nostr protocol.
- [nostr](https://github.com/wilsonsilva/nostr) - a Ruby Nostr gem for use by clients.
- [NNostr.Client](https://github.com/Kukks/NNostr) - a C# Nostr library for use by clients.
- [nostr-tools](https://github.com/fiatjaf/nostr-tools) - a JavaScript client that abstracts the relay management code for use by clients.
- [nostr-relaypool-ts](https://github.com/adamritter/nostr-relaypool-ts) - a TypeScript relay pool library on top of nostr-tools that simplifies handling subscriptions to multiple servers.
- [nostr-react](https://github.com/t4t5/nostr-react) - React Hooks for Nostr.
- [go-nostr](https://github.com/fiatjaf/go-nostr) - a Go library that implements relay management, plus event encoding and signing utils.
- [nostr_rust](https://github.com/0xtlt/nostr_rust) - Functional Rust implementation of the nostr protocol.
- [nostr-js](https://github.com/jb55/nostr-js) - a javascript implementation of the nostr protocol.
- [nostr-rs](https://github.com/futurepaul/nostr-rs) - a Rust implementation of the nostr protocol
- [nostr](https://github.com/rust-nostr/nostr)
  - [nostr](https://github.com/rust-nostr/nostr/tree/master/crates/nostr): Rust implementation of Nostr protocol.
  - [nostr-sdk](https://github.com/rust-nostr/nostr/tree/master/crates/nostr-sdk): High level client library.
  - [bindings](https://github.com/rust-nostr/nostr/tree/master/bindings): UniFFI (Kotlin, Swift, Python, Ruby) bindings.
- [relayer](https://github.com/fiatjaf/relayer) - a server framework for writing custom relays.
- [NostrPostr](https://github.com/Giszmo/NostrPostr) - a Kotlin Nostr library for clients or relays.
- [python-nostr](https://github.com/jeffthibault/python-nostr) - a python library for making clients.
- [nostr-bot](https://github.com/slaninas/nostr-bot) - a Rust library for writing bots.
- [NostrKit](https://github.com/cnixbtc/NostrKit) - a Swift library for interacting with relays.
- [nostr-relay-inspector](https://github.com/dskvr/nostr-relay-inspector) - A library that returns useful information about relays based on nostr-js.
- [schorr_snap](https://github.com/neeboo/schnorr_snap) - A snap plugin for Metamask Flask, supports nostr.
- [nostr-deno](https://github.com/KiPSOFT/nostr-deno) - a client library for Deno javascript runtime.
- [nostr-types](https://github.com/mikedilger/nostr-types) - a rust library defining types useful for the nostr protocol.
- [dart-nostr](https://github.com/ethicnology/dart-nostr) - a Dart library for Flutter.
- [nostr-connect](https://github.com/nostr-connect/connect) - Nostr Connect SDK for TypeScript is a library that allows you to easily integrate Nostr Connect into your web application.
- [pynostr](https://github.com/holgern/pynostr) - a python library for nostr.
- [nostr-php](https://github.com/swentel/nostr-php) - a PHP library for nostr.
- [smtp nostr gateway ](https://github.com/Cameri/smtp-nostr-gateway) - a bridge that forwards emails to pubkeys as encrypted direct messages.
- [matrix-nostr-bridge](https://github.com/8go/matrix-nostr-bridge) - a simple Matrix-to-Nostr or Nostr-to-Matrix bridge.
- [Mostr](https://gitlab.com/soapbox-pub/mostr) - a bridge between Nostr and the Fediverse (Mastodon, ActivityPub, etc.).
- [nostrich.fun](https://nostrich.fun) - A feature-rich directory of nostr projects. A fork of [LightningNetworkStores.com](https://lightningnetworkstores.com)
- [git-nostr-tools](http://git.jb55.com/git-nostr-tools) - A cli tool for sending code patches over nostr.
- [nostr-cln-events](http://git.jb55.com/nostr-cln-events) - A CLN plugin to push clightning node events to nostr.
- [nostr registry](https://codeberg.org/rsbondi/nostr-registry) - a database of known relays with their uptime and NIP support tables
- [nostr-fzf](https://github.com/Cameri/nostr-fzf) - Nostr Directory; a tool for searching usernames and channels.
- [nostr-notify](https://github.com/jb55/nostr-notify) - desktop nostr notifications using libnotify.
- [nostr-launch](https://codeberg.org/rsbondi/nostr-launch) - A tool for launching a bunch of relays and clients locally for development and testing.
- [nostr GitHub Action](https://github.com/theborakompanioni/nostr-action) - send events from GitHub Actions.
- [nostrefresh](https://github.com/melvincarvalho/nostrefresh) -  A simple refresh function for nostr web pages.
- [anonroom](https://github.com/vinliao/anonroom) - anonymous chat room inside nostr.
- [nostril](https://github.com/jb55/nostril) - A C cli tool for creating nostr events.
- [nostr-rs-relay-compose](https://github.com/vdo/nostr-rs-relay-compose) - A Docker compose deployment for nostr-rs-relay with SSL support based on Traefik.
- [nostr.guru](https://nostr.guru/) - a nostr web gateway for viewing events by their ID.
- [nostrandom.netlify.app](https://nostrandom.netlify.app/) - generate publish-able Nostr event with random keys.
- [nashboard](https://github.com/vinliao/nashboard) - A Nostr network dashboard with network statistics, reachable [here](https://nashboard.space/).
- [ndxstr](https://github.com/ArcadeCity/ndxstr) - nostr's layer 2 indexing nodes, with more advanced querying capability than currently supported by relays.
- [nostrillery](https://github.com/Cameri/nostrillery) - A tool for running performance tests against Nostr relays.
- [nostr-terminal](https://github.com/cmdruid/nostr-terminal) - A SSH-like access to your machine via web terminal, powered by Nostr.
- [nostreq](https://github.com/blakejakopovic/nostreq) - A Nostr relay event request generator.
- [nostr.io](https://nostr.io/) - A network statistics with last published notes, top 50 publishers, and top 50 followed users.
- [nostr-commander](https://github.com/8go/nostr-commander-rs) - A simple but convenient CLI-based Nostr app for following users, sending DMs, etc.
- [nostr.directory](https://github.com/pseudozach/nostr.directory) - A searchable database of nostr users and their other social media links.
- [nostr-tool](https://github.com/0xtrr/nostr-tool) - A Rust CLI tool to generate and publish events.
- [frostr](https://github.com/nickfarrow/frostr) - Create joint nostr identities and require t-of-n signatures to post.
- [nostr.rest](https://nostr.rest) - Mine proof of work public keys with user specified prefixes.
- [lnpass](https://lnpass.github.io) - A key manager for Lightning and nostr.
- [sb.nostr.band](https://sb.nostr.band) - Search bots that you can create and follow to receive new posts matching a keyword right into your feed.
- [rss.nostr.band](https://rss.nostr.band) - Create custom RSS feeds with posts matching your keywords and consume using your favorite RSS reader.
- [nostrview](https://nostrview.com) - A nostr search engine. Search by content, tags, events or pub keys.
- [nostr-bulk-dms](https://github.com/leesalminen/nostr-bulk-dm) - A tool that allows you to send DMs over nostr to many recipients in bulk.
- [nostrify](https://github.com/joelklabo/nostrify) - A Core Lightning plugin that sends events (forwards, connect, disconnect, etc.) to nostr.
- [nip06-web](https://github.com/jaonoctus/nip06-web) - a website to generate or restore NIP-06 seed phrases
- [nip06-cli](https://github.com/jaonoctus/nip06-cli) - a Node.js CLI to generate or restore NIP-06 seed phrases.
- [nostr-broadcast](https://github.com/leesalminen/nostr-broadcast) - A tool lets you take your events from some relays and broadcast them to another relay. Could be helpful for backing up your notes to a private relay.
- [nostr-follow-bundler](https://github.com/leesalminen/nostr-follow-bundler) - A tool lets you create lists of profiles that other users can then see and follow themselves.
- [nostr-proxy](https://github.com/dolu89/nostr-proxy) - Push and get events to your Proxy, get results from multiple Nostr relays.
- [nostrends](https://github.com/akiomik/nostrends) - Trending on Nostr, like Twitter trends. Live at [nostrends.vercel.app](https://nostrends.vercel.app).
- [homebrew-nostr](https://github.com/0xbabo/homebrew-nostr) - Homebrew tap for Nostr software.
- [heyxynip5](https://github.com/bennyhodl/hexynip5) - A CLI helper for converting nostr npub/nsec to their hex format for NIP-05 verification.
- [http-nostr-publisher](https://github.com/getAlby/http-nostr-publisher) - A Cloudflare worker to publish Nostr events to relays through a non-blocking HTTP interface .
- [blastr](https://github.com/MutinyWallet/blastr) - A nostr cloudflare workers proxy relay that publishes to all known relays.
- [keystr-rs](https://github.com/keystr/keystr-rs) - An application for managing Nostr keys. Written in Rust, with simple UI (Iced).
- [nostr_simple_publish](https://www.drupal.org/project/nostr_simple_publish/) - Drupal module to publish content to Nostr.
- [nostr-spam-detection](https://github.com/blakejakopovic/nostr-spam-detection) - An experiment in building a machine learning model to label Nostr spam content for filtering and relay rejection.
- [blogsync](https://github.com/canostrical/blogsync) - Self-host blog articles from long-form notes e.g. via Caddy server.
- [NostrFlu](https://heguro.github.io/nostr-following-list-util/) - A tool to collect and resend following lists from relays. You can also check badges.
- [nkcli](https://github.com/mdzz-club/nkcli) - A CLI tool for nostr key manage and serve NIP-46.
- [git-nostr](https://github.com/colealbon/git-nostr)- A tool to enhance git cli with nostr communications.
- [nostr-wtf](https://github.com/LightningK0ala/nostr-wtf) - A set of nostr tools available and deployed on a web app including a [pubkey converter](https://lightningk0ala.github.io/nostr-wtf/) and [relay query tool](https://lightningk0ala.github.io/nostr-wtf/query).
- [strfry policies](https://gitlab.com/soapbox-pub/strfry-policies)- A collection of moderation & antispam policies for the strfry relay developed in TypeScript/Deno.
- [nostrum](https://github.com/nostr-connect/nostrum) - Nostrum it's a mobile app that allows you to sign transactions and messages with your Nostr keys. Nostrum is the reference implementation for a remote signer app (ie. Wallet) of the Nostr Connect protocol.
- [nostr-signing-device](https://github.com/lnbits/nostr-signing-device) - Signing device for Nostr built on ESP32.

### iMessage

[Back to the Top](#table-of-contents)

 * [Beeper HitHub](https://github.com/beeper)
 * [iMessage - Getting Started Guide - Beeper](https://help.beeper.com/chat-networks/imessage)
 
[iMessage-exporter](https://github.com/ReagentX/imessage-exporter) is a binary exports iMessage data to txt or html formats. It can also run diagnostics to find problems with the iMessage database.

[pypush](https://github.com/JJTech0130/pypush) is a POC demo of my recent iMessage reverse-engineering. It can currently register as a new device on an Apple ID, set up encryption keys, and send and receive iMessages!

[Self-Host Beeper](https://github.com/beeper/self-host) is a self-hosted universal chat app that can chat with your friends on iMessage from your Android device using your phone number. You can also join iMessage Group Chats with your phone number and blue bubbles, and share full-resolution images, videos, and audio. 

[Beeper Mini](https://help.beeper.com/beeper-mini/beeper-mini-getting-started-guide-site) is an Andorid app that can chat with your friends on iMessage from your Android device using your phone number. You can also join iMessage Group Chats with your phone number and blue bubbles, and share full-resolution images, videos, and audio.

[Beeper Bridge Manager](https://github.com/beeper/bridge-manager) is a tool for running self-hosted bridges with the Beeper Matrix server. 

[Matrix Ansible and Docker Deploy](https://github.com/spantaleev/matrix-docker-ansible-deploy) is a Matrix (An open network for secure, decentralized communication) server setup using Ansible and Docker.

### Communications

[Back to the Top](#table-of-contents)

[Matrix](https://matrix.org/) is a tool that gives you simple HTTP APIs and SDKs (iOS, Android, Web) to create chatrooms, direct chats and chat bots, complete with end-to-end encryption, file transfer, synchronised conversation history, formatted messages, read receipts and more.

[Postmoogle](https://gitlab.com/etke.cc/postmoogle) is an actual SMTP server that allows you to send and receive emails on your matrix server. It can't be used with arbitrary email providers, because it acts as an actual email provider itself, so you can use it to send emails from your apps and scripts as well.

[SimpleX](https://simplex.chat/) is a privacy redefined messenger without user IDs. Other apps have user IDs: **Signal, Matrix, Session, Briar, Jami, Cwtch, etc.** SimpleX does not, not even random numbers.

[Element](https://element.io/) is a Matrix web client built using the [Matrix React SDK](https://github.com/matrix-org/matrix-react-sdk).

[Mattermost](https://mattermost.com/) is a secure, open source platform for communication, collaboration, and workflow orchestration across tools and teams.

[Mastadon](https://joinmastodon.org/) is a a decentralized social media platform that supports audio, video and picture posts, accessibility descriptions, polls, content warnings, animated avatars, custom emojis, thumbnail crop control, and more, to help you express yourself online.

[Telegram](https://telegram.org/) is a cross-platform, cloud-based instant messaging service. It has an open API and source code free for everyone. Telegram also provides end-to-end encrypted video calling, VoIP, file sharing and several other features.

[Berty](https://github.com/berty/berty) is a secure peer-to-peer messaging app that works with or without internet access, cellular data or trust in the network.

[Pleroma](https://pleroma.social/) is a free and open communication for everyone. Pleroma is social networking software compatible with other Fediverse software such as Misskey, Pixelfed, Mastodon and many others. 

[ffsend](https://gitlab.com/timvisee/ffsend) is a easily and securely share files from the command line. A fully featured Firefox Send client. 

[Nostr(Notes and Other Stuff Transmitted by Relays)](https://github.com/nostr-protocol/nostr) is a truly censorship-resistant alternative to Twitter that has a chance of working.

[Diaspora](https://diasporafoundation.org/) is a privacy-aware, distributed, open source social network.

[Hubzilla](https://framagit.org/hubzilla/core) is a general purpose communication server integrated with a web publishing system and a decentralised permission system.

[Expanse](https://github.com/jc9108/expanse) is a fully selfhosted multi-user web app for externally storing Reddit items (saved, created, upvoted, downvoted, hidden) to bypass Reddit's 1000-item listing limits.

[giscus](https://giscus.app/) is a comments system powered by GitHub Discussions. Let visitors leave comments and reactions on your website via GitHub.

[Mailroute](https://mailroute.net/) is a great tool that provides the best email filtering & security( CMMC, NIST 800-171, DFARS, DISA, HIPPA). It protects your inbox, stop spam, viruses, ransomware, security threats & more with email filtering services. With an easy setup on Office 365, Google & more.

[Docker Mailserver](https://github.com/docker-mailserver/docker-mailserver) is a production-ready fullstack but simple mail server (SMTP, IMAP, LDAP, Antispam, Antivirus, etc.) running inside a container. Only configuration files, no SQL database. 

[Diun](https://github.com/crazy-max/diun) is a CLI application written in Go and delivered as a single executable (and a Docker image) to receive notifications when a Docker image is updated on a Docker registry.

[iRedMail](https://www.iredmail.org/) is a self-hosted email server.

[iRedMail Easy](https://www.iredmail.org/easy.html) is a web-based deployment platform, it offers an easy to use web interface to help you deploy iRedMail server, keep your server up to date, also get fast and professional technical support from iRedMail team.

[Spider Email Archiver](https://spiderd.io/) is  an On-Premises Email Archiving Software.

[MailCow](https://github.com/mailcow/mailcow-dockerized) is a self-hosted email server.

[Nextcloud Talk](https://nextcloud.com/talk/) is a on-premises, private audio/video conferencing and text chat through browser and mobile interfaces with integrated screen sharing and SIP integration.

[Poste.io Email Server](https://poste.io/) is self-hosted SMTP + IMAP + POP3 + Antispam + Antivirus Web administration + Web email. It is easy setup with a [DNS guide]((https://poste.io/doc/configuring-dns)) for protect from spam.

### Business Management

[Back to the Top](#table-of-contents)

[Nextcloud](http://nextcloud.com/) is a suite of enterprise client-server software for creating and using file hosting services. It offers an on-premise Universal File Access and sync platform with powerful collaboration capabilities and desktop, mobile and web interfaces. 

[Odoo](https://www.odoo.com/) is a suite of open source business apps that cover all your company needs: CRM, eCommerce, accounting, inventory, point of sale, project management, etc.

[Kanboard](https://kanboard.org/) is project management software that focuses on the Kanban methodology.

[Eden Workplace](https://www.edenworkplace.com/products) is a complete workplace management platform that lets you achieve more. Desk Booking Software to make desk reservations easier for your team, including assigning permanent and hybrid desks, providing wayfinding solutions for employees.

[Matomo](https://matomo.org/) is an ethical alternative where you won't make privacy sacrifices or compromise your site. Matomo is the Google Analytics alternative that protects your data and your customer's privacy. 

[Plausible Analytics](https://plausible.io/) is a simple, lightweight (< 1 KB), open-source and privacy-friendly alternative to Google Analytics. It doesn’t use cookies and is fully compliant with GDPR, CCPA and PECR. You can self-host Plausible or have us run it for you in the Cloud. 

[Mailroute](https://mailroute.net/) is a great tool that provides the best email filtering & security( CMMC, NIST 800-171, DFARS, DISA, HIPPA). It protects your inbox, stop spam, viruses, ransomware, security threats & more with email filtering services. With an easy setup on Office 365, Google & more.

[InvoicePlane](https://www.invoiceplane.com/) is a self-hosted open source application for managing your quotes, invoices, clients and payments.

### Collaboration & Synchronization

[Back to the Top](#table-of-contents)

[Syncthing](https://syncthing.net/) is a continuous file synchronization program. It synchronizes files between two or more computers in real time.

[Synology](https://www.synology.com/) is a tool that allows you to easily access and manage files in your Synology Drive on the go. Apart from common file types, such as documents, images, videos and music, you can also open Synology Office document, spreadsheets and slides in the user-friendly viewer provided by Drive.

[Nextcloud](http://nextcloud.com/) is a suite of client-server software for creating and using file hosting services. It offers an on-premise Universal File Access and sync platform with powerful collaboration capabilities and desktop, mobile and web interfaces. 

[Lsyncd (Live Syncing Mirror Daemon)](https://github.com/lsyncd/lsyncd) is a tool used in Linux systems to keep directories synchronized. These directories can be found locally, within the same machine, or remotely, on different machines. For remote synchronization, this article focuses on using SSH to accomplish it.

[FileRun](https://hub.docker.com/r/filerun/filerun) is a self-hosted Google Drive alternative. It is a full featured web based file manager with an easy to use user interface.

[FileBrowser](https://hub.docker.com/r/filebrowser/filebrowser) provides a file managing interface within a specified directory and it can be used to upload, delete, preview, rename and edit your files. It allows the creation of multiple users and each user can have its own directory.

[Rsync](https://rsync.samba.org/) is a utility in the command line which enables users to transfer and synchronize files efficiently between a computer and an external hard drive in the entire connected network.

[Warpinator](https://github.com/linuxmint/warpinator) is a free, open-source tool for sending and receiving files between computers that are on the same network. 

[LocalSend](https://localsend.org/) is a free and open-source tool that allows you to send files and messages over the local LAN network to nearby devices. Everything is sent securely over HTTPS. The TLS/SSL certificate is generated on the fly on each device. It's avilable on Windows, macOS, Linux, iOS, and Android.

[FileZilla Client](https://filezilla-project.org/) is a fast and reliable cross-platform FTP, FTPS and SFTP client with lots of useful features and an intuitive graphical user interface. 

[Dragit](https://github.com/sireliah/dragit) is an application for intuitive file sharing between devices. It's useful for when you want to send file from one computer to another with minimal effort. Dragit automatically detects devices in the local network with help of mDNS protocol and allows you to send file immediately. 

[WinFsp](https://github.com/winfsp/winfsp) is a set of software components for Windows computers that allows the creation of user mode file systems. In this sense it is similar to FUSE (Filesystem in Userspace), which provides the same functionality on UNIX-like computers.

[SSHFS-Win](https://github.com/winfsp/sshfs-win) is a minimal port of SSHFS to Windows. Looking under the hood it uses Cygwin for the POSIX environment and WinFsp for the FUSE (Filesystem in Userspace) functionality.

[RiftShare](https://riftshare.app) is a cross platform (Windows, MacOS, Linux) file sharing tool that supports fully encrypted transfers both on the local network and off network using a simple passphrase. RiftShare uses [magic-wormhole](https://github.com/magic-wormhole/magic-wormhole) under the hood and is compatible with other magic-wormhole clients. It is also fully open source and licensed under the GPLv3. 

[Usermode FTP Server](https://gitlab.com/ergoithz/umftpd) is a tool that let's you start an FTP server as user and transfer files with any FTP client. Allowing you to access your files directly with many file browsers' builtin FTP support: Windows File Explorer, Thunar, Gnome Files, Dolphin and many more. 

[TagSpaces](https://www.tagspaces.org/) is a free, no vendor lock-in, open source application for organizing, annotating and managing local files with the help of tags. It features advanced note taking functionalities and some capabilities of to-do apps. It's available for Windows, Linux, Mac OS and Android. 

[Listmonk](https://listmonk.app/) is a standalone, self-hosted, newsletter and mailing list manager. It is fast, feature-rich, and packed into a single binary. 

### Encryption

[Back to the Top](#table-of-contents)

[VeraCrypt](https://www.veracrypt.fr/code/VeraCrypt/) is free open-source disk encryption software for Windows, Mac OS X and Linux. The file encryption, data encryption performed by VeraCrypt is real-time (on-the-fly), automatic, transparent, needs very little memory, and does not involve temporary unencrypted files.   
[AxCrypt](https://axcrypt.net/) is an inexpensive and effective encryption tool for Windows, macOS, iOS, and Android.

[AESCrypt](https://www.aescrypt.com/) is an advanced file encryption utility that integrates with the Windows shell or runs from the Linux command prompt to provide a simple, yet powerful, tool for encrypting files using the Advanced Encryption Standard (AES). It is available for Windows, MacOS, and Linux.

[Linux Unified Key Setup (LUKS)](https://www.redhat.com/sysadmin/disk-encryption-luks) is a disk encryption specification created by Clemens Fruhwirth in 2004 and was originally intended for Linux. It uses device mapper crypt ( dm-crypt) as a kernel module to handle encryption on the block device level.

[GNU Privacy Guard (GnuPG)](https://gnupg.org/) is a complete and free implementation of the OpenPGP standard as defined by RFC4880 (also known as PGP ). It allows you to encrypt and sign your data and communications; it features a versatile key management system, along with access modules for all kinds of public key directories.

[Pretty Good Privacy (PGP)](https://en.wikipedia.org/wiki/Pretty_Good_Privacy) is an encryption program that provides cryptographic privacy and authentication for data communication. It's used for signing, encrypting, and decrypting texts, e-mails, files, directories, and whole disk partitions and to increase the security of e-mail communications. 

[Deadbolt](https://github.com/alichtman/deadbolt) is a Dead-simple file encryption for any OS.

[Infisical](https://infisical.com/) is an open-source, end-to-end encrypted platform to sync secrets and configs across your team and infrastructure. 

[Hemmelig.app](https://github.com/HemmeligOrg/Hemmelig.app) is a tool that keeps your sensitive information out of chat logs, emails, and more with encrypted secrets. 

 **How Encryption Keys work**
 
 <p align="center">
<img src="https://user-images.githubusercontent.com/45159366/196625534-1cebcd35-7654-41cc-bbb2-33913a391a53.png">
  <br />
</p>
 
  * **Symmetric** is a data encryption method whereby the same private key is used to encode and decode information.
  
  * **Asymmetric** is a data encryption method that allows users to encrypt information using shared keys. For example, if you need to send a message across the internet, but you don't want anyone but the intended recipient to see what you've written.
 
 **Types of Encryption**
 
  * **Triple DES (Triple Data Encryption Algorithm)** is a symmetric-key block cipher, which applies the DES cipher algorithm three times to each data block(contains 64 bits of data).
  
  * **AES (Advanced Encryption Standard)** is an algorithm that encrypts and decrypts data in blocks of 128 bits. It can do this using 128-bit, 192-bit, or 256-bit keys.
  
  * **RSA (Rivest–Shamir–Adleman)** is a type of public-key cryptography used for secure data transmission of e-mail and other digital transactions over the Internet. 
  
   * **Twofish**  is a symmetric key block cipher with a block size of 128 bits and key sizes up to 256 bits. It is an advanced version of Blowfish encryption.
  
  * **Format Preserving Encryption (FPE)** is a valid encryption algorithm to be used for compliance with NIST standards. It is mostly used in on-premise encryption and tokenization solutions.
 
 **Application Level Encryption**
 
  * **Hashes** is a function that converts an input of letters and numbers into an encrypted output of a fixed length. For example, algorithms such as [MD5 (Message Digest 5)](https://en.wikipedia.org/wiki/MD5) or [SHA (Secure Hash Algorithm)](https://en.wikipedia.org/wiki/Secure_hash_algorithms).
  
  * **Digital Certificates** is a file that verifies the identity of a device or user and enables encrypted connections. A digital signature is a hashing approach that uses a numeric string to provide authenticity and validate identity. Digital certificates are typically issued by a **certificate authority (CA)**, which is a trusted third-party entity that issues digital certificates for use by other parties.

### Backups

[Back to the Top](#table-of-contents)

[Proxmox Backup Server](https://www.proxmox.com/en/proxmox-backup-server) is an enterprise backup solution for backing up and restoring VMs, containers, and physical hosts. The open-source solution supports incremental backups, deduplication, Zstandard compression, and authenticated encryption.

[BackupPC](https://github.com/backuppc/backuppc) is a high-performance, enterprise-grade system for backing up Linux, Windows and macOS PCs and laptops to a server's disk. BackupPC is highly configurable and easy to install and maintain.

[BorgWarehouse](https://borgwarehouse.com/) is a  fast and modern WebUI for a BorgBackup's central repository server.

[Emborg](https://emborg.readthedocs.io/en/latest/) is a simple command line utility to orchestrate backups. It is built as a front-end to Borg, a powerful and fast de-duplicating backup program. 

[Borgmatic](https://github.com/modem7/docker-borgmatic) is a simple, configuration-driven backup software for servers and workstations. It protects your files with client-side encryption. Backup your databases too. Monitor it all with integrated third-party services. 

[Vorta](https://vorta.borgbase.com/) is a backup client for macOS and Linux desktops. It integrates the mighty Borg Backup with your favorite desktop environment to protect your data from disk failure, ransomware and theft. 

[UrBackup](https://www.urbackup.org/) is an easy to setup Open Source client/server backup system, that through a combination of image and file backups accomplishes both data safety and a fast restoration time. File and image backups are made while the system is running without interrupting current processes. Available for Windows, macOS, and Linux. 

[Kopia](https://kopia.io/) is a user-friendly desktop app for Windows, macOS, and Linux which allows you to create snapshots, define policies, and restore files quickly with Fast and Encrypted Backups.

[Clonezilla](https://clonezilla.org/) is a partition and disk imaging/cloning program. It helps you to do system deployment, bare metal backup and recovery. Three types of Clonezilla are available, Clonezilla live, Clonezilla lite server, and Clonezilla SE (server edition).

[rsnapshot](https://rsnapshot.org/) is a filesystem snapshot utility based on rsync. This makes it easy to make periodic snapshots of local machines, and remote machines over ssh.

[Duplicity](https://duplicity.us/) is a tool that backs directories by producing encrypted tar-format volumes and uploading them to a remote or local file server. Because duplicity uses [librsync](https://github.com/librsync/librsync), the incremental archives are space efficient and only record the parts of files that have changed since the last backup. 

[ZnapZend](https://www.znapzend.org/) is a high performance open source ZFS backup with mbuffer and ssh support. It uses the built-in snapshot functionality of ZFS for fully consistent backups. For each fileset, a pre- and post-snapshot command can be configured to quiet down any software writing to the fileset prior to snapshotting.

[SnapRAID](https://github.com/amadvance/snapraid) is a folder-based backup tool that behaves like a software or hardware RAID5/6 disk raid, but is not a disk raid itself. There is no realtime recovery, free space between disks cannot be combined and manual excution of backup is needed. 

[rsync.net](https://rsync.net/) is a Cloud Storage for Offsite Backup that give you an empty UNIX filesystem to access with any SSH tool. Built on ZFS for data security and fault tolerance with support for rsync/sftp/scp/borg/rclone/restic/git-annex.

### Snapshots Management/System Recovery

[Back to the Top](#table-of-contents)

[rsnapshot](https://rsnapshot.org/) is a filesystem snapshot utility based on rsync. This makes it easy to make periodic snapshots of local machines, and remote machines over ssh.

[rsync.net](https://rsync.net/) is a Cloud Storage for Offsite Backup that give you an empty UNIX filesystem to access with any SSH tool. Built on ZFS for data security and fault tolerance with support for rsync/sftp/scp/borg/rclone/restic/git-annex.

[ZnapZend](https://www.znapzend.org/) is a high performance open source ZFS backup with mbuffer and ssh support. It uses the built-in snapshot functionality of ZFS for fully consistent backups. For each fileset, a pre- and post-snapshot command can be configured to quiet down any software writing to the fileset prior to snapshotting.

[Sanoid](https://github.com/jimsalterjrs/sanoid) is a policy-driven snapshot management tool for ZFS filesystems.

[ZFSBootMenu](https://zfsbootmenu.org/) is a Linux bootloader that attempts to provide an experience similar to FreeBSD's. This allows a user to have multiple "boot environments" (with different distributions, for example), manipulate snapshots before booting, and, for the adventurous user, even bootstrap a system installation via ```zfs recv```.

[Btrfs maintenance toolbox](https://github.com/kdave/btrfsmaintenance) is a set of scripts supplementing the btrfs filesystem and aims to automate a few maintenance tasks. This means the scrub, balance, snapshots, trim or defragmentation.

[Btrbk](https://github.com/digint/btrbk) is a backup tool for btrfs subvolumes, taking advantage of btrfs specific capabilities to create atomic snapshots and transfer them incrementally to your backup locations.

[ksync](https://github.com/ksync/ksync) is a toool that sync files between your local system and a kubernetes cluster. It transparently updates containers running on the cluster from your local checkout. 

[Verify](https://github.com/VerifyTests/Verify) is a snapshot tool that simplifies the assertion of complex data models and documents.

[Timeshift](https://github.com/linuxmint/timeshift) is a Linux application for providing functionality to restore your system just like Windows System Restore tool. Timeshift makes snapshots of your system in regular intervals which are further used at the time of restoration or undo all changes in the system.

[CRIU (Checkpoint and Restore in Userspace)](https://github.com/checkpoint-restore/criu) is a utility to checkpoint/restore Linux tasks. Using this tool, you can freeze a running application (or part of it) and checkpoint it to a hard drive as a collection of files. You can then use the files to restore and run the application from the point it was frozen at. 

[Rsync time backup](https://github.com/laurent22/rsync-time-backup) is a Time Machine style backup with rsync. It creates incremental backups of files and directories to the destination of your choice. The backups are structured in a way that makes it easy to recover any file at any point in time. It works on Linux, macOS and Windows (via WSL).

[rdiff-backup](https://rdiff-backup.net/) is a simple backup tool which can be used locally and remotely, on Linux and Windows, and even cross-platform between both. Users have reported using it successfully on FreeBSD and MacOS.

[Mainframer](https://github.com/buildfoundation/mainframer) is a tool that executes a command on a remote machine while syncing files back and forth. The process is known as remote execution (in general) and remote build (in particular cases).

### Archiving

[Back to the Top](#table-of-contents)

[Access to Memory (AtoM)](https://www.accesstomemory.org/) - Web-based, open source application for standards-based archival description and access in a multilingual, multi-repository environment. 

[ArchiveBox](https://archivebox.io/) - Self-hosted _wayback machine_ that creates HTML & screenshot archives of sites from your bookmarks, browsing history, RSS feeds, or other sources. 

[Archivematica](https://www.archivematica.org/en/) - Mature digital preservation system designed to maintain standards-based, long-term access to collections of digital objects.

[ArchivesSpace](https://archivesspace.org/) - Archives information management application for managing and providing Web access to archives, manuscripts and digital objects. 

[CKAN](https://ckan.org) - CKAN is a tool for making open data websites. 

[Collective Access - Providence](https://collectiveaccess.org/) - Highly configurable Web-based framework for management, description, and discovery of digital and physical collections supporting a variety of metadata standards, data types, and media formats. 

[Omeka S](https://omeka.org/s/) - Omeka S is a web publication system for universities, galleries, libraries, archives, and museums. It consists of a local network of independently curated exhibits sharing a collaboratively built pool of items, media, and their metadata.

[Wayback](https://github.com/wabarc/wayback) - A self-hosted toolkit for archiving webpages to the Internet Archive, archive.today, IPFS, and local file systems. 

### Home Server

[Back to the Top](#table-of-contents)

[Home Assistant](https://www.home-assistant.io/) is an open source home automation that puts local control and privacy first. Home Assistant is powered by a worldwide community of tinkerers and DIY enthusiasts that runs great on Raspberry Pi. 

[Homebridge](https://homebridge.io/) is a software framework that allows you to integrate with smart home devices that do not natively support [HomeKit](https://www.apple.com/shop/accessories/all/homekit). There are over 2,000 Homebridge plugins supporting thousands of different smart accessories. 

[Homebridge UI](https://github.com/oznu/homebridge-config-ui-x) is a tool that provides an easy to use interface to manage your Homebridge plugins, configuration and accessories.

   - Install and configure Homebridge plugins.
   - Monitor your Homebridge server via a fully customisable widget-based dashboard.
   - View and control Homebridge accessories.
   - Backup and Restore your Homebridge instance.

[ESPHome](https://esphome.io/) is a system to control your ESP8266/ESP32 by simple yet powerful configuration files and control them remotely through Home Automation systems.

[Shelly Cloud](https://shelly.cloud/) is a Smart home control tool that has been perfected and provides precise monitoring of your Shelly devices no matter where you are. Shelly devices are compatible with Alexa, Google Home, Android, and iOS. 

[Zigbee](https://csa-iot.org/all-solutions/zigbee/) is the full-stack, secure, reliable, and market-proven solution used by a majority of large smart home ecosystem providers, such as Amazon's Echo Plus, Samsung SmartThings, Signify (Philips Hue), and more.

[openHAB](https://github.com/openhab) is a cross-platform software with the aim to integrate all kinds of Smart Home technologies, devices, etc. 

[Z-Wave](https://www.z-wave.com/) is the leading wireless communications protocol behind many of the secure, trusted brands that are working to make everyone's home smarter and safer.

[Homey](https://homey.app/) is an applciation to control, automate and monitor your entire smart home from your phone, tablet or desktop. 

[Caddy](https://caddyserver.com/) is the only web server to use HTTPS automatically and by default. Caddy obtains and renews TLS certificates for your sites automatically.

[Bazarr](https://hub.docker.com/r/linuxserver/bazarr) is a companion application to Sonarr and Radarr. It can manage and download subtitles based on your requirements. You define your preferences by TV show or movie and Bazarr takes care of everything for you. 

[Sonarr](https://github.com/Sonarr/Sonarr) is a PVR for Usenet and BitTorrent users. It can monitor multiple RSS feeds for new episodes of your favorite shows and will grab, sort and rename them. 

[Homarr](https://github.com/ajnart/homarr) is a customizable browser's home page to interact with your homeserver's Docker containers (e.g. Sonarr/Radarr)

[Midarr](https://github.com/midarrlabs/midarr-server) is a free and open source (and always will be), Midarr aims to provide a tailored experience for you and your users:

   * Beautifully crafted user interface.
   * Real-time online statuses.
   * Simple and easy invite system.
   * Integrates with your existing services, Radarr and Sonarr.

[Rustdesk](https://rustdesk.com/) is an open source virtual/remote desktop infrastructure for everyone. Display and control your PC (Windows, macOS, and Linux) and Android devices. 

[TinyPilot](https://tinypilotkvm.com/) is a tool that enables KVM over IP letting you control any computer remotely.

[PM2](https://github.com/Unitech/pm2) is a production process manager for Node.js applications with a built-in load balancer. It allows you to keep applications alive forever, to reload them without downtime and to facilitate common system admin tasks.

[authentik](https://github.com/goauthentik/authentik) is an open-source Identity Provider focused on flexibility and versatility. You can use authentik in an existing environment to add support for new protocols. authentik is also a great solution for implementing signup/recovery/etc in your application, so you don't have to deal with it.

[ESPHome Remote](https://github.com/landonr/esphome-remote) IS a WI-FI smart home remote with display that runs on ESPHome. It uses Lilygo T-Display or M5Stack Fire.

[Tdarr](https://tdarr.io/) is a distributed transcode automation application using FFmpeg/HandBrake + Audio/Video library analytics + video health checking (Windows, macOS, Linux & Docker). A common use for Tdarr is to simply convert video files from h264 to h265 (hevc), saving 40%-50% in size.

[AppFlowy](https://www.appflowy.io/) is an open-source alternative to Notion where you're in charge of your data and customizations. 

[deemix](https://deemix.app/) is a barebone [deezer](https://www.deezer.com/) downloader library built from the ashes of Deezloader Remix.

[Neko](https://github.com/m1k1o/neko/) is a self hosted virtual browser that runs in docker and uses WebRTC.

[QNAP Switch System (QSS)](https://www.qnap.com/) is a configuration interface for QNAP's managed switch series. Enable management functions such as link aggregation, VLAN, and RSTP, to take care of your network topology with ease.

[ASUSTOR](https://www.asustor.com/) is a subsidiary of ASUS and a leading provider of network attached storage (NAS). It specializes in the development and integration of storage, backup, multimedia, video surveillance and mobile applications for home and enterprise users.

[Seafile](https://www.seafile.com/) is an open-source, cross-platform file-hosting software system. Seafile organize files into libraries stored on a central server. Each library can be synced into any desktop computer(Windows, Mac and Linux) and mobile devices through apps. 

[SnapRAID](http://www.snapraid.it/) is a folder-based backup tool that behaves like a software or hardware RAID5/6 disk raid, but is not a disk raid itself. There is no realtime recovery, free space between disks cannot be combined and manual excution of backup is needed. 

[FreeNAS](https://www.truenas.com/freenas/) is an Open Source Storage Platform and supports sharing across Windows, Apple, and UNIX-like systems. This includes ZFS (high storage capacities and integrates file systems and volume management into a single piece of software). It supports UPS, CIFS/SMB, FTP, NFS, RSYNC, SSH, AFP, Unison, UPnP, Webserver, iSCSI protocols, local and MS AD authentication, and disk enctyption.

[Gladys Assistant](https://github.com/gladysassistant/gladys) is a  privacy-first, open-source home assistant and runs great on Raspberry Pi.

[Audiobookshelf](https://github.com/advplyr/audiobookshelf) is a self-hosted audiobook and podcast server.

[Mistborn](https://gitlab.com/cyber5k/mistborn) is a secure platform for easily standing up and managing your own cloud services: including firewall, ad-blocking, and multi-factor WireGuard VPN access.


### Media Server

[Back to the Top](#table-of-contents)

[Overseerr](https://overseerr.dev/) is a free and open source software application for managing requests for your media library. It integrates with your existing services, such as [Sonarr](https://sonarr.tv/), [Radarr](https://radarr.video/), and [Plex](https://www.plex.tv/).

[Jellyfin](https://jellyfin.org/) is a Free Software Media System that puts you in control of managing and streaming your media. It is an alternative to the proprietary Emby and Plex, to provide media from a dedicated server to end-user devices via multiple apps.

[Swiftfin](https://github.com/jellyfin/Swiftfin) is a modern video client for the Jellyfin media server. Redesigned in Swift to maximize direct play with the power of VLC and look native on all classes of Apple devices.

[Intro Skipper](https://github.com/ConfusedPolarBear/intro-skipper) is a tool that analyzes the audio of television episodes to detect and skip over intro sequences in Jellyfin.

[Jellyseerr](https://github.com/Fallenbagel/jellyseerr) is a free and open source software application for managing requests for your media library. It is a a fork of Overseerr built to bring support for Jellyfin & Emby media servers.

[Midarr](https://github.com/midarrlabs/midarr-server) is a free and open source (and always will be), Midarr aims to provide a tailored experience for you and your users:

   * Beautifully crafted user interface.
   * Real-time online statuses.
   * Simple and easy invite system.
   * Integrates with your existing services, Radarr and Sonarr.
   
[Kirino Media Server](https://kirino.io/) is a lightweight, modular alternative to Plex and Jellyfin.

[Emby](https://emby.media/) is a home media server built on top of other popular open source technologies such as Service Stack, jQuery, jQuery mobile, and Mono. It features a REST-based API with built-in documention to facilitate client development. 

[OpenMediaVault](https://www.openmediavault.org/) is a next generation network attached storage (NAS) solution based on Debian Linux. It contains services like SSH, (S)FTP, SMB/CIFS, AFS, UPnP media server, DAAP media server, RSync, BitTorrent client and many more.

[MediaElch](https://github.com/Komet/MediaElch) is a MediaManager for Kodi. Information about Movies, TV Shows, Concerts and Music are stored as NFO files.

[tinyMediaManager](https://www.tinymediamanager.org/) is a media management tool written in Java/Swing. It is written to provide metadata for the Kodi Media Center (formerly known as XBMC), MediaPortal and Plex media server. 

[FileBot](https://www.filebot.net/) is the ultimate tool for renaming and organizing your movies, TV shows and Anime. Match and rename media files against online databases, download artwork and cover images, fetch subtitles, write metadata, and more, all at once in matter of seconds.

[Plex media server](https://www.plex.tv/) is a application that gives you the power to add, access and share all the entertainment that matters to you, on almost any device. With 50,000+ on demand titles and hundreds of channels of live TV, plus your own personal media collection, using one powerful app.

[Tautulli](https://tautulli.com/) is a 3rd party application that you can run alongside your Plex Media Server to monitor activity and track various statistics.

[Plex DupeFinder](https://github.com/l3uddz/plex_dupefinder) is a python script that finds duplicate versions of media (TV episodes and movies) in your Plex Library and tells Plex to remove the lowest rated files/versions (based on user-specified scoring) to leave behind a single file/version.

[Prometheus Exporter for Plex](https://github.com/jsclayton/prometheus-plex-exporter) is an expose library playback, storage, and host metrics in a Prometheus format.

[Infuse](https://firecore.com/) is a Video Player for iOS, Apple TV, and Mac. It plays every video file ever created to avoid wasting hours converting and transcoding files.

[InfuseSync](https://github.com/firecore/InfuseSync) is a plugin for Emby and Jellyfin media servers that tracks all media changes to decrease sync times with Infuse clients. 

[InvidTUI](https://darkhz.github.io/invidtui/) is an invidious client, which fetches data from invidious instances and displays a user interface in the terminal, and allows for selecting and playing Youtube audio and video.

[Polaris](https://github.com/agersant/polaris) is a music streaming application, designed to let you enjoy your music collection from any computer or mobile device. Polaris works by streaming music directly from your computer (or cloud server), without uploading it to a third-party.

[AirSonic](https://hub.docker.com/r/airsonic/airsonic) is a free, web-based media streamer, providing ubiquitous access to your music.

[TubeSync](https://github.com/meeb/tubesync) is a PVR (personal video recorder) for YouTube. Or, like Sonarr but for YouTube (with a built-in download client). It is designed to synchronize channels and playlists from YouTube to local directories and update your media server once media is downloaded.

[yt-fts](https://github.com/NotJoeMartinez/yt-fts) is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.

[Tube Archivist](https://github.com/tubearchivist/tubearchivist) is a self hosted YouTube media server.

[PeerTube](https://joinpeertube.org/) is an ActivityPub-federated video streaming platform using P2P directly in your web browser.

[Ant Media Server](https://github.com/ant-media/Ant-Media-Server) is a streaming engine software that provides adaptive, ultra low latency streaming by using WebRTC technology with ~0.5 seconds latency. 

[Castopod](https://code.castopod.org/adaures/castopod) is an open-source hosting platform made for podcasters who want engage and interact with their audience. 

[Festival](https://festival.pm/) is a music player for local album collections.

[HD HomeRun Scribe 4K](https://www.silicondust.com/product/hdhomerun-scribe-4k/) is a free local live TV with DVR with 4 tuners and 150 hours of recording storage all-in-one amazing box for watching and recording free TV all around your home.

[RuneAudio](https://www.runeaudio.com/) is a free and open source software that turns embedded hardware into Hi-Fi music players.

[Volumio (The Audiophile Music Player)](https://volumio.com/) is a very powerful and convenient music aggregator, now Volumio can also be used with great results in all sorts of different situations.

[Snapcast](https://github.com/badaix/snapcast) is a multiroom client-server audio player, where all clients are time synchronized with the server to play perfectly synced audio. It's not a standalone player, but an extension that turns your existing audio player into a Sonos-like multiroom solution.

[SonoBus](https://sonobus.net) is an easy to use application for streaming high-quality, low-latency peer-to-peer audio between devices over the internet or a local network.

[MythTV](https://www.mythtv.org/) is a Free Open Source software digital video recorder (DVR) project distributed under the terms of the GNU GPL. 

### Smart Home Automation

[Back to the Top](#table-of-contents)

**Smart home** is a process that allows homeowners to control appliances, thermostats, lights, and other smart devices remotely using a smartphone or tablet through an internet connection.

Most **smart devices** have their own [Virtual Local Area Network (VLAN)](https://en.wikipedia.org/wiki/VLAN) with little to no internet access with broadcasts forwarding to LAN [Subnet aka Subnetwork](https://www.cloudflare.com/learning/network-layer/what-is-a-subnet/) for discovery. Using software such as **Home Assistant, Homebridge, ESPHome, etc.** help simplify the process of controlling and automating all your smart devices.

[Matter](https://buildwithmatter.com/) is an open standard for smart home technology that lets your device work with any Matter-certified ecosystem using a single protocol. Matter comes from the [Connectivity Standards Alliance](https://csa-iot.org/), an organization of hundreds of companies(Amazon, Apple, Google, Comcast, Zigbee Alliance, and Connectivity Standards Alliance (CSA) creating products for the smart home.

**Proprietary Smart Devices**

 * [Amazon Alexa](https://alexa.amazon.com/) is a smart virtual assistant software to manage Alexa-enabled devices, control music playback, view shopping lists on the go, keep track of upcoming reminders, check on active timers and much more. 

 * [Google Assistant](https://assistant.google.com/) is a smart virtual assistant software on mobile and home automation devices.

 * [Apple HomeKit](https://www.apple.com/shop/accessories/all/homekit) is a software framework that enables your app to coordinate and control home automation accessories from multiple vendors to present a coherent, user-focused interface. Using HomeKit, your app can: Discover HomeKit-compatible automation accessories and add them to a persistent, cross-device home configuration database.

 * [Samsung SmartThings](https://www.smartthings.com/) is a sofwtare framework that you can connect, monitor and control multiple smart home devices quicker and easier. Connect your Samsung smart TVs, smart appliances, smart speakers and brands like Ring, Nest and Philips Hue all from one app.

 * [Philips Hue](https://www.philips-hue.com) is  a smart lighting system. The smart lights, Hue Bridge, and smart controls will forever change the way you experience light.

 * [Sonos](https://www.sonos.com) is the wireless home sound system that fills as many rooms as you want with great-sounding music, movies, and TV. 
 
**------------------------------------------------------------------**

[Home Assistant](https://www.home-assistant.io/) is an open source home automation that puts local control and privacy first. Home Assistant is powered by a worldwide community of tinkerers and DIY enthusiasts that runs great on Raspberry Pi. [$13 USD voice assistant remote for Home Assistant](https://www.home-assistant.io/voice_control/thirteen-usd-voice-remote/)

_Add-ons are additional applications and services, that can be run alongside
Home Assistant. The Home Assistant OS and Supervised installations types,
provide the Supervisor, which is capable of running and managing these add-ons._

**Home Assistant Official Add-ons**

_Addons created and maintained by the Home Assistant team._

* [DuckDNS](https://github.com/home-assistant/hassio-addons/blob/master/duckdns/DOCS.md) - This updates your Duck DNS IP address and generate SSL using Let's Encrypt.
* [Almond](https://github.com/home-assistant/hassio-addons/blob/master/almond/DOCS.md) - An Open, Privacy-Preserving Virtual Assistant.
* [HomeMatic](https://github.com/home-assistant/hassio-addons/blob/master/homematic/DOCS.md) - HomeMatic central based on OCCU.
* [Let's Encrypt](https://github.com/home-assistant/hassio-addons/blob/master/letsencrypt/DOCS.md) - Get a free SSL certificate from Let's Encrypt; an open and automated certificate authority (CA).
* [MariaDB](https://github.com/home-assistant/hassio-addons/blob/master/mariadb/DOCS.md) - An open source relational database (fork of MySQL).
* [File editor](https://github.com/home-assistant/hassio-addons/blob/master/configurator/DOCS.md) - Browser-based configuration file editor.
* [Mosquitto](https://github.com/home-assistant/hassio-addons/blob/master/mosquitto/DOCS.md) - Fast and reliable MQTT broker.
* [Terminal & SSH](https://github.com/home-assistant/hassio-addons/blob/master/ssh/DOCS.md) - Allows logging in remotely to using a web terminal or SSH client.
* [Samba](https://github.com/home-assistant/hassio-addons/blob/master/samba/DOCS.md) - Access your configuration files using Windows network shares.
* [NGINX SSL proxy](https://github.com/home-assistant/hassio-addons/blob/master/nginx_proxy/DOCS.md) - Reverse proxy with SSL termination.
* [deCONZ](https://github.com/home-assistant/hassio-addons/blob/master/deconz/DOCS.md) - Control a ZigBee network using ConBee or RaspBee hardware by Dresden Elektronik.
* [TellStick](https://github.com/home-assistant/hassio-addons/blob/master/tellstick/DOCS.md) - Run a TellStick and TellStick Duo service.
* [Ada](https://github.com/home-assistant/hassio-addons/blob/master/ada/DOCS.md) - Ada is voice assistant powered by Almond which is open and privacy-preserving.
* [Fully Kiosk Browser](https://www.home-assistant.io/integrations/fully_kiosk/) is a powerful kiosk browser for Android devices. It provides a number of features for monitoring and controlling your Android device. This integration gives you access to control your device and view the status in Home Assistant.

**Home Assistant Third Party Add-ons**

_Add-ons created by the community._

* [Dasshio](https://github.com/danimtb/dasshio) - Easily use your Amazon Dash Buttons.
* [InfluxDB](https://github.com/hassio-addons/addon-influxdb) - Scalable datastore for metrics, events, and real-time analytics.
* [Grafana](https://github.com/hassio-addons/addon-grafana) - Open platform for beautiful analytics and monitoring.
* [Tor](https://github.com/hassio-addons/addon-tor) - Protect your privacy and access your instance via Tor.
* [Spotify Connect](https://github.com/hassio-addons/addon-spotify-connect) - Spotify Connect client for playing music on your Home Assistant device.
* [SSH & Web Terminal](https://github.com/hassio-addons/addon-ssh) - SSH and Web-based terminal with tons of pre-loaded useful tools.
* [UniFi Controller](https://github.com/hassio-addons/addon-unifi) - The UniFi Controller allows you to manage your UniFi network using a web browser.
* [Node-RED](https://github.com/hassio-addons/addon-node-red) - Flow-based programming for the Internet of Things.
* [Plex Media Server](https://github.com/hassio-addons/addon-plex) - Your recorded media beautifully organized and ready to stream.
* [IDE](https://github.com/hassio-addons/addon-ide) - Advanced web-based IDE, based on Cloud9 IDE.
* [zigbee2mqtt](https://github.com/danielwelch/hassio-zigbee2mqtt) - Zigbee to MQTT bridge, get rid of your proprietary Zigbee bridges.
* [Matrix](https://github.com/hassio-addons/addon-matrix) - A secure and decentralized communication platform.
* [AdGuard Home](https://github.com/hassio-addons/addon-adguard-home) - A network-wide ad-and-tracker blocking DNS server with parental control.
* [Traccar](https://github.com/hassio-addons/addon-traccar) - Traccar is modern GPS Tracking Platform.
* [Home Panel](https://github.com/hassio-addons/addon-home-panel) - A touch-compatible web frontend for controlling the home.
* [Hass.io Google Drive Backup](https://github.com/sabeechen/hassio-google-drive-backup) - A complete and easy to configure solution for backing up your snapshots to Google Drive.
* [Grocy](https://github.com/hassio-addons/addon-grocy) - A groceries & household management solution for your home.
* [EmonCMS](https://github.com/inverse/hassio-addon-emoncms) - A powerful open-source web app for processing, logging, and visualizing energy, temperature, and other environmental data.
* [CrowdSec](https://github.com/crowdsecurity/home-assistant-addons) - A next-gen collaborative IPS/IDS to protect you from intrusion.
* [AppDaemon](https://github.com/hassio-addons/addon-appdaemon) - Python Apps and HADashboard.
* [TasmoAdmin](https://github.com/hassio-addons/addon-tasmoadmin) - Centrally manage all your Sonoff-Tasmota devices.
* [Aircast](https://github.com/hassio-addons/addon-aircast) - AirPlay capabilities for your Chromecast players.
* [AirSonos](https://github.com/hassio-addons/addon-airsonos) - AirPlay capabilities for your Sonos players.
* [Log Viewer](https://github.com/hassio-addons/addon-log-viewer) - Browser-based live log viewing utility.
* [Tautulli](https://github.com/hassio-addons/addon-tautulli) - Monitor and get statistics from your Plex server.
* [motionEye](https://github.com/hassio-addons/addon-motioneye) - Simple, elegant and feature-rich CCTV/NVR for your cameras.
* [JupyterLab](https://github.com/hassio-addons/addon-jupyterlab) - Create documents containing live code, equations, visualizations, and explanatory text.
* [Glances](https://github.com/hassio-addons/addon-glances) - A cross-platform system monitoring tool written in Python.

**Home Assistant Custom Cards**

_The Home Assistant Dashboards allows people to build custom cards on top of it, which you can easily add to your instance._

* [Simple Thermostat](https://github.com/nervetattoo/simple-thermostat) - A simpler and more flexible thermostat card.
* [Card Modder](https://github.com/thomasloven/lovelace-card-mod) - Style your Lovelace cards.
* [Bar Card](https://github.com/Gluwc/bar-card) - Customizable animated bar card.
* [forked-daapd Card](https://github.com/kalkih/forked-daapd-card) - Control a forked daapd instance.
* [Dual Gauge Card](https://github.com/Rocka84/dual-gauge-card) - Shows two gauges in one.
* [Atomic Calendar Revive](https://github.com/totaldebug/atomic-calendar-revive) - Calendar card with advanced settings.
* [Simple Weather Card](https://github.com/kalkih/simple-weather-card) - A minimalistic weather card, inspired by Google Material Design.
* [Auto-Entities Card](https://github.com/thomasloven/lovelace-auto-entities) - Dynamically adds entities.
* [Canvas Gauge Card](https://github.com/custom-cards/canvas-gauge-card) - Use awesome gauges from canvas-gauges.com.
* [Big Number Card](https://github.com/custom-cards/bignumber-card) - Display big numbers for sensors, including severity level as background.
- [Animated Weather Card](https://github.com/bramkragten/weather-card) - Nice looking card showing the weather, with subtle animations.
- [Thermostat Card](https://github.com/ciotlosm/lovelace-thermostat-dark-card) - Thermostat control card that looks like a Nest Thermostat.
* [Raspberry Pi Status Card](https://github.com/ironsheep/lovelace-rpi-monitor-card) - Show status of your Raspberry Pis.
* [Mini Media Player](https://github.com/kalkih/mini-media-player) - A minimalistic media player card.
* [Mini Graph Card](https://github.com/kalkih/mini-graph-card) - A minimalistic sensor graph card.
* [Button card](https://github.com/kuuji/button-card) - Button card for your entities.
* [Slider Entity Row](https://github.com/thomasloven/lovelace-slider-entity-row) - Add a slider to adjust, e.g., the brightness of lights in lovelace entity cards.
* [Power Wheel Card](https://github.com/gurbyz/power-wheel-card) - An intuitive way to represent the power that your home is consuming or producing.
* [Home Card](https://github.com/postlund/home-card) - A quick glance of the state of your home.
* [Banner Card](https://github.com/nervetattoo/banner-card) - A fluffy linkable banner with interactive glances to spice up your home dashboards.
* [Spotify Card](https://github.com/custom-cards/spotify-card) - List and select from current available devices and users top playlists on Spotify.
* [Battery Entity](https://github.com/cbulock/lovelace-battery-entity) - Displaying battery levels for battery entities.
* [Multiple Entity Row](https://github.com/benct/lovelace-multiple-entity-row) - Show multiple entity states or attributes on entity rows.
* [Home Feed Card](https://github.com/gadgetchnnel/lovelace-home-feed-card) - Display a combination of persistent notifications, calendar events, and entities in the style of a feed.
* [Config Template Card](https://github.com/custom-cards/config-template-card) - Allow using templates in Lovelace.
* [RGB Light Card](https://github.com/bokub/rgb-light-card) - Colorful buttons to control your RGB Lights.
* [Restriction Card](https://github.com/iantrich/restriction-card) - A card to provide restrictions on Lovelace cards defined within.
* [Vacuum Map Card](https://github.com/PiotrMachowski/Home-Assistant-Lovelace-Xiaomi-Vacuum-Map-card) - This card provides a user-friendly way to fully control Xiaomi (Roborock/Viomi/Dreame/Roidmi) and Neato (+ possibly other) vacuums.
* [Vacuum Card](https://github.com/denysdovhan/vacuum-card) - A card to card for controlling a vacuum cleaner robot.
* [Purifier Card](https://github.com/denysdovhan/purifier-card) - A card for controlling air purifiers.

**Home Assistant Custom Integrations**

_Additional integrations for Home Assistant created by the community._

* [Lutron Caseta Pro](https://github.com/upsert/lutron-caseta-pro) - Integrates Lutron Caseta Smart Bridge PRO / RA2 Select.
* [SmartIR](https://github.com/smartHomeHub/SmartIR) - Integrates devices using Broadlink IR.
* [Alexa Media Player](https://github.com/keatontaylor/alexa_media_player) - Allow control of Amazon Alexa devices.
* [Circadian Lighting](https://github.com/claytonjn/hass-circadian_lighting) - Circadian Lighting slowly synchronizes your color changing lights with the regular naturally occuring color temperature of the sky throughout the day.
* [Volkswagen Carnet](https://github.com/robinostlund/homeassistant-volkswagencarnet) - Integrates Volkswagen Carnet (requires valid Carnet subscription).
* [Untappd](https://github.com/custom-components/sensor.untapped) - Connects with your Untappd account.
* [Elasticsearch](https://github.com/legrego/homeassistant-elasticsearch) - Publishes events to Elasticsearch.
* [HASS Aarlo](https://github.com/twrecked/hass-aarlo) - Asynchronous Arlo integration. Similar to the Arlo web site; monitors events and states for all base stations, cameras and doorbells.
* [Xiaomi Cloud Map Extractor](https://github.com/PiotrMachowski/Home-Assistant-custom-components-Xiaomi-Cloud-Map-Extractor) - Presents a live view of a map for Xiaomi (Roborock/Viomi/Roidmi/Dreame) vacuums without a need for rooting.
* [Xiaomi Hygrothermo](https://github.com/dolezsa/Xiaomi_Hygrothermo) - Sensor platform for Xiaomi Mijia BT Hygrothermo temperature and humidity sensor.
* [WebRTC Camera](https://github.com/AlexxIT/WebRTC) - View RTSP streams from IP Cameras in real-time through WebRTC or MSE with Pan/Zoom controls.
* [Sonoff LAN](https://github.com/AlexxIT/SonoffLAN) - Control Sonoff devices with eWeLink (original) firmware over LAN and/or Cloud.
* [Spotcast](https://github.com/fondberg/spotcast) - Start Spotify playback on an idle Chromecast device as well as control Spotify connect devices.
* [The Watchman](https://github.com/dummylabs/thewatchman) - Keep track of missing entities and services in your config files.

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177719765-602b4658-c8bf-4952-a238-4b986efbb7cb.png">
  <br />
</p>

Home Assistant integrations. Credit: [Home Assistant](https://www.home-assistant.io/integrations/)

[Homebridge](https://homebridge.io/) is a software framework that allows you to integrate with smart home devices that do not natively support [HomeKit](https://www.apple.com/shop/accessories/all/homekit). There are over 2,000 Homebridge plugins supporting thousands of different smart accessories. 

[Homebridge UI](https://github.com/oznu/homebridge-config-ui-x) is a tool that provides an easy to use interface to manage your Homebridge plugins, configuration and accessories.

   - Install and configure Homebridge plugins.
   - Monitor your Homebridge server via a fully customisable widget-based dashboard.
   - View and control Homebridge accessories.
   - Backup and Restore your Homebridge instance.
   
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/202679713-5cc8dede-7e61-42e1-ab71-def824bc70de.png">
  <br />
</p>
   
[Homebridge Raspberry Pi Image](https://github.com/homebridge/homebridge-raspbian-image) is a free Raspbian based Raspberry Pi image with Homebridge and Homebridge Config UI X pre-installed.

[Homebridge Config UI X](https://github.com/oznu/homebridge-config-ui-x) is a web based management tool for [Homebridge](https://github.com/homebridge/homebridge) that allows you to manage all aspects of your Homebridge setup.

[Homebridge webOS TV](https://github.com/merdok/homebridge-webos-tv) is a plugin for homebridge which allows you to control your LG webOS TV from your Home app! It should work with all TVs that support webOS2 and newer.

[Homebridge Unifi Protect](https://github.com/hjdhjd/homebridge-unifi-protect) is a Homebridge plugin that provides HomeKit support to the [UniFi Protect](https://ui.com/camera-security) device ecosystem. UniFi Protect is [Ubiquiti's](https://www.ui.com/) next-generation video security platform, with rich camera, doorbell, and NVR controller hardware options for you to choose from, as well as an app which you can use to view, configure and manage your video camera and doorbells.

[Homebridge Camera FFmpeg](https://github.com/Sunoo/homebridge-camera-ffmpeg) is a Homebridge Plugin Providing [FFmpeg](https://www.ffmpeg.org/)-based Camera Support.

[Homebridge Mi Aqara](https://github.com/YinHangCode/homebridge-mi-aqara) is a homebridge plugin for XiaoMi Aqara plugin.

[Homebridge Camera UI](https://github.com/seydx/homebridge-camera-ui) is a tool that allows you to expose cameras from camera.ui to HomeKit via Homebridge. 

[HOOBS](https://hoobs.org/) is a tool that makes smart accessories(over 2000 options) compatible with your favorite ecosystem. Whether you prefer Apple Homekit, Google Home, or Amazon Alexa, you’re unlikely to find compatible accessories and services that all work together nicely under one roof.

[ESPHome](https://esphome.io/) is a system to control your ESP8266/ESP32 by simple yet powerful configuration files and control them remotely through Home Automation systems.

[Shelly Cloud](https://shelly.cloud/) is a Smart home control tool that has been perfected and provides precise monitoring of your Shelly devices no matter where you are. Shelly devices are compatible with Alexa, Google Home, Android, and iOS.

[Homey](https://homey.app/) is an applciation to control, automate and monitor your entire smart home from your phone, tablet or desktop. 

[Ecobee](https://www.ecobee.com) is a home automation company in Canada that makes thermostats for residential and commercial use.

[Lutron Caséta](https://www.lutron.com/en-US/Products/Pages/SingleRoomControls/CasetaWireless/Overview.aspx) is a smart lighting control system that is a great solution for giving any client smart lighting control. It was purposely built to work in homes of all ages and it works with older wiring as well as new.

[Insteon switches](https://www.insteon.com/) is a Hub for controlling and configuring your home's devices is quick, easy and fun. The setup takes a couple of minutes and a few moments per light switch, sensor, etc. It bridges your devices to 3rd party services like Amazon Alexa and Google Assistant, while being controlled from any smartphone or tablet.

[Jeedom](https://www.jeedom.com/) is an open source software; taht gives you complete access to the software that manages your home automation. It's compatible with various protocols such as, ZigBee, Z-Wave, EnOcean, KNX, LoRaWAN, BACnet, Modbus, etc..

[Beestat](https://github.com/beestat/app) is a tool that connects with your thermostat and provides you with useful charts and analytics so that you can make informed decisions and see how the changes you make lower your energy footprint.

[MQTT](https://mqtt.org/) is an [OASIS standard](https://www.oasis-open.org/standards/) messaging protocol for the Internet of Things (IoT). It is designed as an extremely lightweight publish/subscribe messaging transport that is ideal for connecting remote devices with a small code footprint and minimal network bandwidth.

[Zigbee](https://csa-iot.org/all-solutions/zigbee/) is the full-stack, secure, reliable, and market-proven solution used by a majority of large smart home ecosystem providers, such as Amazon's Echo Plus, Samsung SmartThings, Signify (Philips Hue), and more.

[openHAB](https://github.com/openhab) is a cross-platform software with the aim to integrate all kinds of Smart Home technologies, devices, etc. 

[Z-Wave](https://www.z-wave.com/) is the leading wireless communications protocol behind many of the secure, trusted brands that are working to make everyone's home smarter and safer.

[pfSense](https://www.pfsense.org/) is a firewall/router computer software distribution based on FreeBSD.

[Pi-hole](https://pi-hole.net/) is a [DNS sinkhole](https://en.wikipedia.org/wiki/DNS_Sinkhole) that protects your devices from unwanted content, without installing any client-side software, intended for use on a private network. It is designed for use on embedded devices with network capability, such as the Raspberry Pi, but it can be used on other machines running Linux and cloud implementations.

[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome) is a DNS relay station with ad/tracker/other blocking, IP address redirections, and DNS-over-HTTPS.

[OpenWRT](https://openwrt.org/) is an open-source project for embedded operating systems based on Linux, primarily used on embedded devices to route network traffic.

[ZoneMinder](https://zoneminder.com/) is a full-featured, open source, state-of-the-art video surveillance software system. Monitor your home, office, or wherever you want.

[Plex media server](https://www.plex.tv/) is a application that gives you the power to add, access and share all the entertainment that matters to you, on almost any device. With 50,000+ on demand titles and hundreds of channels of live TV, plus your own personal media collection, using one powerful app.

### Voice Assistants

[Back to the Top](#table-of-contents)

[$13 voice assistant remote for Home Assistant](https://www.home-assistant.io/voice_control/thirteen-usd-voice-remote/)

[Wyoming](https://github.com/rhasspy/wyoming) is a peer-to-peer protocol for voice assistants (basically [JSONL](https://jsonlines.org/) + PCM audio). It's used in [Rhasspy](https://github.com/rhasspy/rhasspy3/) and the [Home Assistant](https://www.home-assistant.io/integrations/wyoming) for communication with voice services.

[Wyoming Faster Whisper](https://github.com/rhasspy/wyoming-faster-whisper) is a Wyoming protocol server for the faster-whisper speech to text system.

[Wyoming Porcupine1](https://github.com/rhasspy/wyoming-porcupine1) is a Wyoming protocol server for the porcupine1 wake word detection system.

[Wyoming Snowboy](https://github.com/rhasspy/wyoming-snowboy) is a Wyoming protocol server for the snowboy wake word detection system.

[faster-whisper](https://github.com/guillaumekln/faster-whisper/) is a reimplementation of OpenAI's Whisper model using [CTranslate2](https://github.com/OpenNMT/CTranslate2/), which is a fast inference engine for Transformer models.

[Porcupine](https://github.com/Picovoice/porcupine) is a highly-accurate and lightweight wake word engine. It enables building always-listening voice-enabled applications. It uses deep neural networks trained in real-world environments.

[Rhasspy](https://github.com/rhasspy/rhasspy3/) is an open source voice assistant toolkit for many human languages.

[openWakeWord](https://github.com/dscripka/openWakeWord) is an open-source wakeword library that can be used to create voice-enabled applications and interfaces. It includes pre-trained models for common words & phrases that work well in real-world environments.

[Conversation](https://www.home-assistant.io/integrations/conversation) is an integration allows you to converse with **Home Assistant.** You can either converse by pressing the microphone in the frontend (supported browsers only (no iOS)) or by calling the ```conversation/process``` service with the transcribed text.

[Piper](https://github.com/rhasspy/piper/) is a fast, local neural text to speech system that sounds great and is optimized for the Raspberry Pi 4.

[Mycroft](https://mycroft.ai/) is an open source voice assistant that is private by default and completely customizable.

[DeepSpeech](https://github.com/mozilla/DeepSpeech) is an open source embedded (offline, on-device) speech-to-text engine which can run in real time on devices ranging from a Raspberry Pi 4 to high power GPU servers.

[Leon](https://github.com/leon-ai/leon) is your open-source personal assistant. 

[Olivia](https://olivia-ai.org/) is an open-source chatbot built in Golang using Machine Learning technologies. Its goal is to provide a free and open-source alternative to big services like DialogFlow.

[Alan SDK](https://github.com/alan-ai/alan-sdk-web) is an voice assistant SDK to build a voice interface for websites and web apps (JavaScript, React, Angular, Vue, Ember, Electron).

[OpenAssistant](https://open-assistant.io/) is a chat-based assistant that understands tasks, can interact with third-party systems, and retrieve information dynamically to do so. 

### Video Surveillance

[Back to the Top](#table-of-contents)

[Frigate](https://frigate.video/) is an open source NVR built around real-time AI object detection. All processing is performed locally on your own hardware, and your camera feeds never leave your home.

[hkcam](https://hochgatterer.me/hkcam/) is an open-source implementation of an HomeKit IP camera. It uses ffmpeg to access the camera stream and publishes the stream to HomeKit using hap. The camera stream can be viewed in a HomeKit app. 

[OpenDataCam](https://opendata.cam/) is an open source tool to quantify the world. It quantifies and tracks moving objects with live video analysis. It is designed to be an accessible, affordable and open-source solution to better understand interactions in urban environments. It never records any photo or video data. The system only saves surveyed meta-data, in particular the path an object moved or number of counted objects at a certain point.

[Viseron](https://github.com/roflcoopter/viseron) is a Self-hosted, local only NVR and AI Computer Vision software. 

[zmninja](http://zmninja.zoneminder.com/) is a high performance, cross platform ionic app for Home/Commerical Security Surveillance using ZoneMinder.

[Moonfire NVR](https://github.com/scottlamb/moonfire-nvr) is a security camera network video recorder.

[Shinobi Pro](https://gitlab.com/Shinobi-Systems/Shinobi) is a Next Generation in Open-Source Video Management Software with support for over 6000 IP and USB Cameras.

[WyzeHacks](https://github.com/HclX/WyzeHacks) is a project contains a set of scripts trying to provide additional features not implemented by the official firmware. Currently, it provides the following functions:

  * Enable telnetd on your camera.
  * Customize the default root password for telnet login.
  * Redirect all the recordings to an NFS share.
  * Redirect console logs into an NFS share.
  * Automatically reboot the camera at certain time.
  * Automatically archive the recordings.

### Text-To-Speech Synthesis (TTS)

[Back to the Top](#table-of-contents)

[whisper.cpp](https://github.com/ggerganov/whisper.cpp) is a high-performance inference of OpenAI's Whisper automatic speech recognition (ASR) model.

[WaaS](https://github.com/schibsted/WAAS) is a Whisper as a Service (GUI and API for OpenAI Whisper).

[Web Whisper](https://codeberg.org/pluja/web-whisper) is a OpenAI's whisper on your web browser. [Demo](https://whisper.r3d.red/)

[Vosk](https://github.com/alphacep/vosk-api) is an offline open source speech recognition toolkit. It enables speech recognition for 20+ languages and dialects.

[Coqui TTS](http://coqui.ai/) is a deep learning toolkit for Text-to-Speech, battle-tested in research and production.

[Mozilla TTS](https://github.com/mozilla/TTS) is a library for advanced Text-to-Speech generation. It's built on the latest research, was designed to achieve the best trade-off among ease-of-training, speed and quality.

[NVIDIA NeMo](https://github.com/NVIDIA/NeMo) is a conversational AI toolkit built for researchers working on automatic speech recognition (ASR), text-to-speech synthesis (TTS), large language models (LLMs), and natural language processing (NLP). 


### Video and Audio Processing

[Back to the Top](#table-of-contents)

[Intel® Quick Sync Video](https://www.intel.com/content/www/us/en/architecture-and-technology/quick-sync-video/quick-sync-video-general.html) is a tools that uses the dedicated media processing capabilities of Intel® Graphics Technology to decode and encode fast, enabling the processor to complete other tasks and improving system responsiveness.

[Intel® QuickAssist Technology (Intel® QAT)](https://www.intel.com/content/www/us/en/architecture-and-technology/intel-quick-assist-technology-overview.html) is a scalable, flexible, and extendable way to accelerate data encryption/decryption and compression for applications from networking to enterprise, cloud to storage, and content delivery to database. 

[FFmpeg](https://ffmpeg.org) is a leading multimedia framework that can decode, encode, transcode, mux, demux, stream, filter and play pretty much anything that humans and machines have created. It supports the most obscure ancient formats up to the cutting edge ones on multiple platforms such as Windows, macOS, and Linux.

[FFmpeg.guide](https://ffmpeg.guide/) is a simple GUI tool to create complex FFmpeg filtergraphs quickly and correctly, without having to mess with the cumbersome filter syntax.

[HandBrake](https://handbrake.fr/) is a tool for transcoding video from almost any format with a selection of widely supported codecs. It is supported on Window, macOS, and Linux.

[Tdarr](https://github.com/HaveAGitGat/Tdarr) is a cross-platform conditional based transcoding application for automating media library transcode/remux management in order to process your media files as required. It can set rules for the required codecs, containers, languages etc that your media should have which helps keeps things organized and can increase compatability with your devices. A common use for Tdarr is to simply convert video files from h264 to h265 (hevc), saving 40%-50% in size.

[SRS](https://github.com/ossrs/srs) is a simple, high efficiency and realtime video server, supports RTMP, WebRTC, HLS, HTTP-FLV, SRT and GB28181.

[obsws-python](https://github.com/aatikturk/obsws-python) is a Python SDK for OBS Studio WebSocket v5.0. 

**Video/Audio Standards**

[AAC(Advanced Audio Coding)](https://mpeg.chiariglione.org/) is an audio coding standard for lossy digital audio compression. It's endorsed by ISO and IEC as MPEG-2 and MPEG-4 standards for video streams.

[H.264(AVC)](https://en.wikipedia.org/wiki/H.264/MPEG-4_AVC) is a video compression standard based on block-oriented and motion-compensated integer-DCT coding that defines multiple profiles (tools) and levels (max bitrates and resolutions) with support up to 8K.

[H.265(HEVC)](https://en.wikipedia.org/wiki/High_Efficiency_Video_Coding) is a video compression standard that is the successor to H.264(AVC). It offers a 25% to 50% better data compression at the same level of video quality, or improved video quality at the same bit-rate.

[HTTP Live Streaming (HLS)](https://developer.apple.com/streaming/) is a communications protocol developed by Apple that sends live and on‐demand audio and video to iPhone, iPad, Mac, Apple Watch, Apple TV, and PC.
 
[Dynamic Adaptive Streaming over HTTP (DASH)](https://developer.mozilla.org/en-US/docs/Web/HTML/DASH_Adaptive_Streaming_for_HTML_5_Video) is an adaptive streaming protocol that allows for a video stream to switch between bit rates on the basis of network performance, in order to keep a video playing.

[OpenMAX™](https://www.khronos.org/openmax/) is a cross-platform API that provides comprehensive streaming media codec and application portability by enabling accelerated multimedia components to be developed, integrated and programmed across multiple operating systems and silicon platforms.

[GStreamer](https://gstreamer.freedesktop.org/) is a library for constructing graphs of media-handling components. The applications it supports range from simple Ogg/Vorbis playback, audio/video streaming to complex audio (mixing) and video (non-linear editing) processing. Applications can take advantage of advances in codec and filter technology transparently.

[Media Source Extensions (MSE)](https://www.w3.org/TR/media-source/) is a [W3C specification](https://github.com/w3c/media-source) that allows JavaScript to send byte streams to media codecs within Web browsers that support HTML5 video and audio. Also, this allows the implementation of client-side prefetching and buffering code for streaming media entirely in JavaScript.

[WebRTC](https://webrtc.org/) is an open-source project that adds real-time communication capabilities to your application that works on top of an open standard. It supports video, voice, and generic data to be sent between peers, allowing developers to build powerful voice- and video-communication solutions.

### Podcasting

[Back to the Top](#table-of-contents)

[Castopod](https://code.castopod.org/adaures/castopod) is an open-source hosting platform made for podcasters who want engage and interact with their audience.

[Sovereign Feeds](https://sovereignfeeds.com/) is a tool to Search for your podcasts and add them to your favorites.

[IPFS Podcasting](https://ipfspodcasting.net/) is a Decentralized Podcast Distribution over IPFS where you can crowd hosting podcast episodes with storage & bandwidth provided by volunteer nodes. 

[Audiobookshelf](https://www.audiobookshelf.org/) is a self-hosted audiobook and podcast server.

[Vod2Pod-RSS](https://github.com/madiele/vod2pod-rss) is a tool that converts a YouTube or Twitch channel into a podcast with ease. It creates a podcast RSS that can be listened to directly inside any podcast client. VODs are transcoded to MP3 on the fly and no server storage is needed.

[Podverse](https://podverse.fm/) is creating an open source podcast app for iOS, Android, F-Droid, and Web.

[Alby](https://getalby.com/) is a Bitcoin Lightning App for your Browser.

[Alby wallet API](https://blog.getalby.com/introducing-the-alby-wallet-api/) is an implemented OAuth an open standard that apps use to provide client applications with secure delegated access. Thus Podverse users create an Alby wallet account or use their existing Alby account to grant specific access rights to their Alby wallet. 

[Blubrry](https://blubrry.com/) is a podcast hosting service for publishing platform, live customer support, stress-free migration, and impactful statistics.

[SATurn](https://saturn.fly.dev/) is a tool that lets you connect your getalby.com Account and see which content resonates most with your audience and recognize your top contributors. 

[AntennaPod](https://antennapod.org/) is a podcast player that is completely open. The app is open-source and you can subscribe to any RSS feed. AntennaPod is built by volunteers without commercial interest, so it respects your privacy while giving you full control.

[Podgrab](https://github.com/akhilrex/podgrab) is a self-hosted podcast manager/downloader/archiver tool to download podcast episodes as soon as they become live with an integrated player.

[Podify](https://github.com/podify-org/podify) is a self-hosted service that allows you to download videos and audio from any source supported by youtube-dl, sort the downloads into feeds, and subscribe to these feeds using your favorite podcast app.

[dir2cast](https://github.com/ben-xo/dir2cast/) is designed to turn a directory of MP3s into a podcast - automatically. Perfect for, say, radio shows - upload the MP3s to a folder, and use dir2cast.php as your PodCast URL.

[Snipd](https://www.snipd.com/) is an AI-powered podcast player. Search for moments in the transcript, get summaries, share clips to social media, and export to your second brain & note taking apps. Discover, save, and share highlights from podcasts. 

[Wave Share](https://ggerganov.github.io/wave-share) is a serverless, peer-to-peer, local file sharing through sound.

[KBD Audio](https://github.com/ggerganov/kbd-audio) is a collection of command-line and GUI tools for capturing and analyzing audio data.

### AudioBooks

[Back to the Top](#table-of-contents)

[Audioserve](https://github.com/izderadicka/audioserve) is a simple personal server to serve audio files from directories. Intended primarily for audio books, but anything with decent directories structure will do. Focus here is on simplicity and minimalist design.

[Audiobookshelf](https://www.audiobookshelf.org/) is a self-hosted audiobook and podcast server.

[Jellyfin Bookshelf Plugin](https://github.com/jellyfin/jellyfin-plugin-bookshelf)

### Health

[Back to the Top](#table-of-contents)

[Connect](https://github.com/nextgenhealthcare/connect) is the swiss army knife of healthcare integration.

[Fasten](https://github.com/fastenhealth/fasten-onprem) is an open-source, self-hosted, personal/family electronic medical record aggregator, designed to integrate with 1000's of insurances/hospitals/clinics 

[ERPNext](https://erpnext.com/) is a Free and Open Source Enterprise Resource Planning (ERP) for managing businesses.

[OpenEMR](https://open-emr.org/) is a Free and Open Source electronic health records and medical practice management application. It features fully integrated electronic health records, practice management, scheduling, electronic billing, internationalization, free support, a vibrant community, and a whole lot more. It runs on Windows, Linux, MacOS, and many other platforms.

[Ryot (Roll Your Own Tracker)](https://ryot.fly.dev/) is a self hosted platform for tracking various facets of your life - media, fitness etc.

### Gardening

[Back to the Top](#table-of-contents)

  * [ESPHome: DIY Irrigation Controller With Internal Scheduler](https://community.home-assistant.io/t/esphome-diy-irrigation-controller-with-internal-scheduler/171844)
 * [Smart WiFi Controlled Irrigation System Using Home Assistant and ESPHome](https://www.instructables.com/Smart-WiFi-Controlled-Irrigation-System-Using-Home/)


[OpenSprinkler](https://opensprinkler.com/product/opensprinkler/) is an open-source, web-based smart sprinkler controller for lawn and plant watering, drip irrigation, farm irrigation, hydroponics etc. The current version is OS 3.2, with built-in WiFi (based on ESP8266) and OLED display. 

[Droplet](https://github.com/PricelessToolkit/Droplet) is an ALL-IN-ONE Irrigation and monitoring system for ESPHome and Home Assistant.

[9 Valve Sprinkler Controller](https://github.com/hwstar/9-Valve-Sprinkler-Controller) is a 9 valve sprinkler controller for use with customized firmware such as ESPHOME.

[GardenBot](https://www.gardenbot.org/howTo/) is an open source garden monitoring system. Their website is a collection of tutorials for how to build things (like a soil moisture sensor), software for running GardenBot, resources, links, and more.

[farmOS](https://farmos.org/) is a web-based application for farm management, planning, and record keeping. It is developed by a community of farmers, developers, researchers, and organizations with the aim of providing a standard platform for agricultural data collection and management.

[OpenFarm](https://openfarm.cc/) is a free and open database and web application for farming and gardening knowledge. One might think of it as the Wikipedia for growing plants, though it functions more like a cooking recipes site.

[Growstuff](http://growstuff.org/) is an open source/open data project for food gardeners. They crowdsource information on what our members are growing and harvesting, aggregate it, and make it available as open data via their API.

[Harvest Helper](https://github.com/damwhit/harvest_helper) is a tool that provides growing, harvesting and recipe information for the 45 plants in the database as well as a json api so that people can hopefully use this data to build other apps. 

[HappyPlants](https://happyplants.garden/) is a mobile web application that's all about collecting, organising, and adding all kinds of information of your plants. Basically, creating your own plant database in a visual way.

[Automated irrigation system](https://github.com/PatrickHallek/automated-irrigation-system) is an open source application to water plants automatically. Up to now there is almost no free professional software and instructions available to build a DYI irrigation that is scalable, accurate and most importantly, durable.

[Pigrow](https://github.com/Pragmatismo/Pigrow) is a garden automation suite designed to help gardeners monitor, log, graph and control their grow space using a raspberry Pi, various sensor and a few relay modules.

[Tania](https://usetania.org/) is a farm management software for the hobbyist and smallholder farmer. 


### Maps

[Back to the Top](#table-of-contents)

[Magic Earth](https://www.magicearth.com/) is aTurn-by-turn navigation, OpenStreetMap, Crowd-Sourced Traffic, 3D maps, Satellite maps, Offline maps and Transit.

[Organic Maps](https://organicmaps.app/) is a free Android & iOS offline maps app for travelers, tourists, hikers, and cyclists. It uses crowd-sourced OpenStreetMap data and is developed with love by MapsWithMe (MapsMe) founders and our community. No ads, no tracking, no data collection, no crapware. 

[MapTiler Server](https://www.maptiler.com/server/self-host-satellite-maps/) is a self-hosted Aerial and satellite imagery maps of the entire world from your own server or laptop.

[GPSLogger](https://gpslogger.app/) is a GPS tool that uses the GPS capabilities of your Android phone to log coordinates to GPS format files at regular intervals. This can be particularly useful if you want to geotag your photos after a day out or share your travel route with someone. 

[KelperJs](http://keplerjs.io/) is a open source full-stack geosocial network platform.

[OpenStreetMap(OSM)](https://www.openstreetmap.org/) is a map of the world, created by people like you and free to use under an open license. Hosting is supported by UCL, Fastly, Bytemark Hosting, and other partners.

[uMap](https://github.com/umap-project/umap) is a tool that lets you create maps with OpenStreetMap layers in a minute and embed them in your site. 

[Martin](https://martin.maplibre.org/) is a tile server able to generate [vector tiles](https://github.com/mapbox/vector-tile-spec) from large [PostGIS](https://github.com/postgis/postgis) databases on the fly, or serve tiles from [PMTile](https://protomaps.com/blog/pmtiles-v3-whats-new) and [MBTile](https://github.com/mapbox/mbtiles-spec) files. Martin optimizes for speed and heavy traffic, and is written in Rust.

[MapLibre GL JS](https://github.com/maplibre/maplibre-gl-js) is an open-source library for publishing maps on your websites or webview based apps. Fast displaying of maps is possible thanks to GPU-accelerated vector tile rendering. 

[MapLibre Native](https://maplibre.org/) is an Interactive vector tile maps for iOS, Android and other platforms. 

[Maplibre-rs ](https://github.com/maplibre/maplibre-rs) is an Experimental Maps for Web, Mobile and Desktop.

### Bookmarks

[Back to the Top](#table-of-contents)

[Linkding](https://github.com/sissbruecker/linkding/) is a simple bookmark service that you can host yourself. It's designed be to be minimal, fast, and easy to set up using Docker.

[Linkwarden](https://linkwarden.app/) is a fully self-hostable, open-source collaborative bookmark manager to collect, organize and archive webpages. [Linkwarden Docker Image](https://gist.github.com/joekrill/cc503e21e14f95fefa91acc5f869dac1)

[LinkAce](https://www.linkace.org/) is a self-hosted bookmark archive to collect links of your favorite websites.

[Eagle](https://eagle.cool/) is a tool to collect, search and organize your design files in a logical way and all in one place.

[Shlink](https://shlink.io/) is a self-hosted URL shortener that keeps control over all your shortened URLs, by serving them under your own domains, using this simple yet powerful tool.

[Pinry](https://docs.getpinry.com/) is a tiling image board system for people who want to save, tag, and share images, videos and webpages in an easy to skim through format.

[Shaark](https://github.com/MarceauKa/shaark) is a self-hosted platform to keep and share your content: web links, posts, passwords and pictures.

[Maglit](https://maglit.me/) is an encrypted and privacy respecting Link Shortener service that supports not only your regular website links but also Magnet Links which are extensively used to download and share torrents.

### Photos

[Back to the Top](#table-of-contents)

[PhotoPrism®](https://docs.photoprism.app/license/docs/) is an AI-powered app for browsing, organizing & sharing your photo collection. It makes use of the latest technologies to tag and find pictures automatically without getting in your way. You can run it at home, on a private server, or in the cloud.

[Immich](https://immich.app/) is a high performance self-hosted photo and video backup solution directly from your mobile phone.

[Piwigo](https://piwigo.org/) is a full featured, self-hosted, and open source photo gallery application for the web. It comes with more than 200 templates, plugins, and configurations that let you personalize how your photos are presented. It allows users to upload photos from digiKam, Shotwell, Lightroom or mobile applications. Lastly, users can create galleries and give viewing permissions to their clients. They can download individual photos or whole albums, post comments, give ratings, mark photos as favorites, and perform searches.

[Czkawka](https://github.com/qarmin/czkawka) is a Multi-functional app to find duplicates, empty folders, similar images, etc.

[Phockup](https://github.com/ivandokov/phockup) is a Media sorting tool to organize photos and videos from your camera in folders by year, month and day. 

[PiGallery 2](https://github.com/bpatrik/pigallery2) is a  fast directory-first photo gallery website, with rich UI, optimized for running on low resource servers (especially on Raspberry Pi).

[Photoview](https://photoview.github.io/) is a simple self-hosted and user-friendly photo gallery that's made for photographers and aims to provide an easy and fast way to navigate directories, with thousands of high-resolution photos.

[digiKam](https://www.digikam.org/) is a free and open-source Professional Photo Management tool.

[ShareX](https://getsharex.com/) is a free and open source program that lets you capture or record any area of your screen and share it with a single press of a key. It also allows uploading images, text or other types of files to many supported destinations you can choose from.

[PhotoSync](https://www.photosync-app.com/home.html) is a service to wirelessly transfer, backup & share photos/videos to your computer, NAS, other phones and popular cloud/photo services. It's available for Windows, MacOS, Linux, Android, and iOS.

[Lychee](https://lycheeorg.github.io/) is a great looking and easy-to-use photo-management-system you can run on your server, to manage and share photos. 

[Photoview](https://photoview.github.io/) is a simple and user-friendly photo gallery that's made for photographers and aims to provide an easy and fast way to navigate directories, with thousands of high-resolution photos. 

[Gimme-iPhotos](https://github.com/Zebradil/Gimme-iPhotos) is a tool uses [pyicloud](https://github.com/picklepete/pyicloud) to synchronize photos and videos from iCloud to your local machine.

[PyiCloud](https://github.com/picklepete/pyicloud) is a module which allows pythonistas to interact with iCloud webservices. It's powered by the fantastic [requests](https://github.com/kennethreitz/requests) HTTP library.

[Pixelfed](https://pixelfed.org/) is a fresh take on photo sharing. It decentralized ActivityPub protocol so you can comment, follow, and interact with remote Pixelfed, Mastodon and Pleroma posts and profiles from your Pixelfed account as if you were both on the same website.

[Chevereto](https://hub.docker.com/r/linuxserver/chevereto) is an image hosting software that allows you to create a beautiful and full-featured image hosting website on your own server.

[Got Your Back (GYB)](https://github.com/GAM-team/got-your-back) is a command line tool for backing up your Gmail messages to your computer using Gmail's API over HTTPS. 

[Upscayl](https://upscayl.github.io/) is a free and open source desktop application that lets you upscale your low resolution images using advanced AI Models. Upscayl is a Linux-First Application that prioritizes Linux builds but is also cross-platform.

[Librephotos](https://github.com/LibrePhotos/librephotos) is a self-hosted open source photo management service. This is the repository of the backend. 

[Librephotos frontend](https://github.com/LibrePhotos/librephotos-frontend) is a self-hosted open source photo management service. This is the repository of the frontend. 

[Librephotos  Mobile](https://github.com/LibrePhotos/librephotos-mobile) is an open-source Android and iOS Mobile Application for self-hosted Librephotos Server.

[Librephotos Docker](https://github.com/LibrePhotos/librephotos-docker) is the Dockerfiles for the automated build process of LibrePhotos.

[OneFolder](https://github.com/OneFolderApp/OneFolder) is a Desktop app to sort your images the same way you would in Google Photos, but locally, no need to run a server (and compatible with NAS).

### Pastebins

[Back to the Top](#table-of-contents)

[Bepasty](https://bepasty-server.readthedocs.io/en/latest/) is a pastebin for all kinds of files. 

[Bin](https://github.com/w4/bin) is a paste bin that's actually minimalist.

[Dpaste](https://dpaste.org/) is a Simple pastebin with multiple text and code option, with short url result easy to remember. 

[Drift](https://github.com/MaxLeiter/drift) is a Self-hosted Github Gist clone. 

[EdPaste](https://github.com/ptnr/EdPaste) is a Self-hosted pastebin written in Laravel (PHP Framework).

[ExBin](https://github.com/m1dnight/exbin) is a pastebin with public/private snippets and netcat server.

[Fiche](https://github.com/solusipse/fiche) is a Command line pastebin, all you need is netcat. 

[Filite](https://github.com/raftario/filite) is a simple, light and standalone pastebin, URL shortener and file-sharing service. 

[FlashPaper](https://github.com/AndrewPaglusch/FlashPaper) is a one-time encrypted zero-knowledge password/secret sharing application focused on simplicity and security. No database or complicated set-up required. 

[Hasty Paste](https://enchantedcode.co.uk/hasty-paste/) is a place to quickly paste some text and share it. Mostly used for sharing debug logs and such to help developers provide tech support. The project aims to be both fast and minimal. 

[Lenpaste](https://git.lcomrade.su/root/lenpaste) is a Web service that allows you to share notes anonymously, an alternative to pastebin. 

[LogPaste](https://github.com/mtlynch/logpaste) is a Minimal pastebin web app that's easy to self-host and persists data to any S3-compatible backend. 

[MicroBin](https://microbin.eu/) is a super tiny, feature rich, configurable, self-contained and self-hosted paste bin web application. It is very easy to set up and use, and will only require a few megabytes of memory and disk storage. [MicroBin Docker install setup](https://microbin.eu/docs/installation-and-configuration/docker/).

[Opengist](https://github.com/thomiceli/opengist) is a Self-hosted pastebin powered by Git. 

[Paaster](https://paaster.io) is a secure by default end-to-end encrypted pastebin built with the objective of simplicity. 

[Pastefy](https://pastefy.app/) - Beautiful, simple and easy to deploy Pastebin with optional Client-Encryption, Multitab-Pastes, an API, a highlighted Editor and more.

[Pastila](https://pastila.nl/) is a Minimalistic paste service. Single page, zero click experience.

[Pasty](https://github.com/lus/pasty) is a fast and lightweight code pasting server. 

[PrivateBin](https://privatebin.info/) is a minimalist, opensource online pastebin/discussion board where the server has zero knowledge of hosted data.

[Prologic pastebin](https://git.mills.io/prologic/pastebin) is a Simple pastebin service with convenient api and CLI. 

[PurritoBin](https://github.com/PurritoBin/PurritoBin) is a Ultra fast, minimalistic, encrypted command line paste-bin, where the server has no knowledge of the paste data. 

[Rustypaste](https://github.com/orhun/rustypaste) is a minimal file upload/pastebin service. 

[Spacebin](https://spaceb.in/) is a Reliable Pastebin server in Golang and Fiber. 

[Sup3rS3cretMes5age](https://github.com/algolia/sup3rS3cretMes5age) is a simple to deploy and use secret message service using Hashicorp Vault as a secrets storage.

[Wastebin](https://github.com/matze/wastebin) is a Lightweight, minimal and fast pastebin with an SQLite backend. 

[YABin](https://github.com/Yureien/YABin) is a pastebin that contains plentiful features while remaining simple. Supports optional E2E encryption, a client-side CLI app, syntax highlighting, minimalistic UI, APIs, keyboard shortcuts, and more. It can even be run in serverless environments.


### Note-Taking

[Back to the Top](#table-of-contents)

[Joplin](https://joplinapp.org/) is an open source note-taking app that you can securely access from any device. 

[HedgeDoc](https://hedgedoc.org/) is an open-source, web-based, self-hosted, collaborative markdown editor. 

[Lapce](http://lapce.dev/) is a Lightning-fast And Powerful Code Editor written in pure Rust with a UI in Druid (which is also written in Rust). 

[nb](https://xwmx.github.io/nb) is a CLI and local web plain text note‑taking, bookmarking, and archiving with linking, tagging, filtering, search, Git versioning & syncing, Pandoc conversion, + more, in a single portable script. 

[Outline](https://www.getoutline.com/) is the fastest knowledge base for growing teams. It provides a beautiful, realtime collaborative, feature packed, and markdown compatible. 

[Rustpad](https://rustpad.io/#yAbbW9) is an open-source collaborative text editor based on the operational transformation algorithm. Share a link to this pad with others, and they can edit from their browser while seeing your changes in real time.

[Turtl](https://turtlapp.com/) is a secure, collaborative notebook for bookmarks or passwords, files or shopping lists.

[The Everything App](https://anytype.io/) is an app where you can do everything: Protect your thoughts & data with end-to-end encryption. Local, on-device encryption. Only you have encryption keys. Offline account creation: control your keys, own your data. No server, no gatekeeper: peer-to-peer sync on local networks. Locally store your data, self-host your backups where you please.

[TiddlyWiki](https://tiddlywiki.com/) is a single-file mode wiki application for todo lists, effective project management tool and of course writing drafts and notes. It has extensions for all the major browsers.

[Laverna](https://laverna.cc/) is a note taking application with Markdown editor and encryption support. Consider it like open source alternative to Evernote. 

[Notesnook](https://notesnook.com/) is a fully open source & end-to-end encrypted note taking alternative to Evernote. 

[Zettlr](https://www.zettlr.com/) is an open-source Markdown editor for the 21st century.

[Carnet](https://www.getcarnet.app/) is a complete open source note taking app. It has extensions for all the major browsers.

[Frog](https://tenderowl.com/work/Frog) is a tool that quickly extract text from almost any source: youtube, screencasts, PDFs, webpages, photos, etc. Grab the image and get the text.

[Zeal](https://zealdocs.org/) is an offline documentation browser for software developers inspired by [Dash](https://kapeli.com/dash).

### Time Monitoring

[Back to the Top](#table-of-contents)

[ActivityWatch](https://activitywatch.net) is an app that automatically tracks how you spend time on your devices.

[Kimai](https://www.kimai.org/)  is a free & open source timetracker. It tracks work time and prints out a summary of your activities on demand. 

[Solidtime](https://www.solidtime.io/) is an open source time tracking software for individuals and teams, with a modern user interface and reporting.

[TimeTagger](https://timetagger.app) is an open source time-tracker based on an interactive timeline and powerful reporting. 

[Traggo](https://traggo.net/)  is a tag-based time tracking tool. In Traggo there are no tasks, only tagged time spans.

### Wikis

[Back to the Top](#table-of-contents)

[Archivy](https://github.com/archivy/archivy) is a self-hostable knowledge repository that allows you to learn and retain information in your own personal and extensible wiki. 

[BookStack](https://www.bookstackapp.com/) - BookStack is a simple, self-hosted, easy-to-use platform for organizing and storing information. It allows for documentation to be stored in a book like fashion.

[Cowyo](https://github.com/schollz/cowyo) - Cowyo is a feature-rich wiki for minimalists. 

[django-wiki](https://github.com/django-wiki/django-wiki) - Wiki system with complex functionality for simple integration and a superb interface. Store your knowledge with style: Use django models. 

[Documize](https://documize.com) - Modern Docs + Wiki software with built-in workflow, single binary executable, just bring MySQL/Percona.

[Dokuwiki](https://www.dokuwiki.org/DokuWiki) - Easy to use, lightweight, standards-compliant wiki engine with a simple syntax allowing reading the data outside the wiki. All data is stored in plain text files, therefore no database is required. 

[Gitit](https://github.com/jgm/gitit) - Wiki program that stores pages and uploaded files in a git repository, which can then be modified using the VCS command line tools or the wiki's web interface. 

[Gollum](https://github.com/gollum/gollum) - Simple, Git-powered wiki with a sweet API and local frontend.

[Instiki](https://golem.ph.utexas.edu/wiki/instiki/show/HomePage) - Instiki is a wiki clone so pretty and easy to set up, you'll wonder if it’s really a wiki. Runs on Rails and focuses on portability and stability.

- [Mediawiki](https://www.mediawiki.org/wiki/MediaWiki) - MediaWiki is a free and open-source wiki software package written in PHP. It serves as the platform for Wikipedia and the other Wikimedia projects, used by hundreds of millions of people each month.

[Pepperminty Wiki](https://github.com/sbrl/Pepperminty-Wiki) - Complete markdown-powered wiki contained in a single PHP file. 

[PineDocs](https://github.com/xy2z/PineDocs) - Simple, fast, customizable and lightweight site for browsing files.

[PmWiki](https://www.pmwiki.org) - Wiki-based system for collaborative creation and maintenance of websites. 

[PukiWiki](https://pukiwiki.osdn.jp/) - PukiWiki is a free, simple, open-source wiki management system. Minimalistic and simple design with many tools for collaborative work. Created in Japanese, so translator needed. 

[Raneto](https://raneto.com/) - Raneto is an open source Knowledgebase platform that uses static Markdown files to power your Knowledgebase. 

[TiddlyWiki](https://tiddlywiki.com/) - Reusable non-linear personal web notebook. 

[Tiki](https://tiki.org/HomePage) - Wiki CMS Groupware with the most built-in features. 

[TWiki](https://twiki.org/) - TWiki is a Perl-based structured wiki application, typically used to run a collaboration platform, knowledge or document management system, a knowledge base, or team portal. 

[WackoWiki](https://wackowiki.org/) - WackoWiki is a light and easy to install multilingual Wiki-engine. 

[Gramax](https://gram.ax/) - Free, open-source application for creating, editing, and publishing Git-driven documentation sites using Markdown and a visual editor.

### Gaming

[Back to the Top](#table-of-contents)

[Cartridge](https://github.com/unclebacon-live/cartridge) is a self-hosted game library made with Laravel + Vue.js.

**Cartridge Features**

   - Scan for ROM files and match with IGDB game information
   - Serve ROM download links alongside game details
   - Manage access to library with user creation and permissions (WIP)
   - Allow users to request games (Planned)
   - Play select ROMs in-browser using JS emulators (Planned)
   - Track played and favorite games (even ones that aren't available for download) (Planned)
   
[Moonlight Game Streaming](https://moonlight-stream.org/) is a program that let you stream from your PC games over the Internet with no configuration required. Stream from almost any device, whether you're in another room or miles away from your gaming rig. [Sunshine](https://github.com/LizardByte/Sunshine) is a **Game stream host for Moonlight** that is a self-hosted, low latency, cloud gaming solution with support for AMD, Intel, and NVIDIA GPUs. It is an open source implementation of NVIDIA's GameStream.

<p align="center">
<img src="https://user-images.githubusercontent.com/45159366/106686398-11463d80-657f-11eb-841a-d534829ccc3d.png">
<br />
</p>

[Chiaki](https://git.sr.ht/~thestr4ng3r/chiaki) is a Free and Open Source Software Client for PlayStation 4 and PlayStation 5 Remote Play for Linux, FreeBSD, OpenBSD, Android, macOS, Windows, Nintendo Switch and potentially even more platforms. 

   
#### Game Emulators

[EmuDeck](https://www.emudeck.com/) is a tool that takes care of everything for your retrogaming needs from RetroArch Configuration, Bezels, Gamepad Configuration for GameCube, Wii, Citra, SNES, etc. EmuDeck will even install EmulationStation Desktop Edition and carry over all their custom configurations and no need to configure ROM paths or anything. 

[EmulationStation Desktop Edition (ES-DE)](https://www.es-de.org/) is a frontend application for browsing and launching games from your multi-platform game collection. It's  available for Unix/Linux, macOS(M1 & Intel) and Windows.

[RetroPie](https://retropie.org.uk/) is a frontend for emulators that allows you to turn your Raspberry Pi, ODroid C1/C2, or PC into a retro-gaming machine. It builds upon Raspbian, [EmulationStation](https://github.com/Aloshi/EmulationStation), RetroArch and many other projects to enable you to play your favourite Arcade, home-console, and classic PC games with the minimum set-up.

<p align="center">
<img src="https://user-images.githubusercontent.com/45159366/153087555-e1bde100-6079-4089-a33d-804e29064789.png">
<br />
</p>

[RetroArch](https://www.retroarch.com/) is a frontend for emulators, game engines and media players. It enables you to run classic games on a wide range of computers and consoles through its slick graphical interface. Settings are also unified so configuration is done once and for all. [RetroArch Flatpak](https://flathub.org/apps/details/org.libretro.RetroArch)

[Pterodactyl](https://pterodactyl.io/) is a free, open-source game server management panel built with PHP, React, and Go. Designed with security in mind, Pterodactyl runs all game servers in isolated Docker containers while exposing a beautiful and intuitive UI to end users.

[LinuxGSM (Linux Game Server Managers)](https://linuxgsm.com/) is a command-line tool for quick, simple deployment and management of Linux dedicated game servers.

[Cartridge](https://github.com/unclebacon-live/cartridge) is a self-hosted game library made with Laravel + Vue.js.

**Cartridge Features**

   - Scan for ROM files and match with IGDB game information
   - Serve ROM download links alongside game details
   - Manage access to library with user creation and permissions (WIP)
   - Allow users to request games (Planned)
   - Play select ROMs in-browser using JS emulators (Planned)
   - Track played and favorite games (even ones that aren't available for download) (Planned)

<p align="center">
<img src="https://user-images.githubusercontent.com/45159366/172274231-d691a850-1879-44fb-8fa0-08e549d7bb29.png">
<br />
 Cartridge UI
</p>

[Dolphin](https://dolphin-emu.org) is an emulator for two recent Nintendo video game consoles: the GameCube and the Wii. It allows PC gamers to enjoy games for these two consoles in full HD (1080p) with several enhancements: compatibility with all PC controllers, turbo speed, networked multiplayer, and even more. 

[Citra](https://citra-emu.org/) is an open-source emulator for the Nintendo 3DS capable of playing many of your favorite games. 

[yuzu](https://yuzu-emu.org) is an experimental open-source emulator for the Nintendo Switch from the creators of Citra.[

[m64p](https://m64p.github.io/) is a Nintendo 64 Emulator. It uses mupen64plus-gui, a brand new mupen64plus frontend written in Qt5. It supports all of the things you’d expect from a frontend (savestate management, pausing, screenshots). 

[DeSmuME](https://desmume.org/) is a Nintendo DS emulator. 

[Snes9x](https://www.snes9x.com/) is a portable, freeware Super Nintendo Entertainment System (SNES) emulator.  

[bsnes](https://github.com/bsnes-emu/bsnes) is a Super Nintendo (SNES) emulator focused on performance, features, and ease of use. 

[mGBA](https://mgba.io/) is a new emulator for running Game Boy Advance games. It aims to be faster and more accurate than many existing Game Boy Advance emulators, as well as adding features that other emulators lack. 

[DOSBox](https://www.dosbox.com/) is an open-source DOS emulator which primarily focuses on running DOS Games.

[DOSBox Staging](https://github.com/dosbox-staging/dosbox-staging) is a full x86 CPU emulator (independent of host architecture), capable of running DOS programs that require real or protected mode. 

[Flycast](https://github.com/flyinghead/flycast) is a multi-platform Sega Dreamcast, Naomi and Atomiswave emulator derived from reicast. 

[PCSX2](https://pcsx2.net/) is a PlayStation 2 'emulator', a free program that tries to replicate the PlayStation 2 console to enable you to play PS2 games on your PC. 

[RPCS3](https://rpcs3.net/) is an experimental open-source Sony PlayStation 3 emulator and debugger written in C++ for Windows and Linux. RPCS3 started development in May of 2011 by its founders DH and Hykem. The emulator is currently capable of running over 1800 commercial titles powered by Vulkan and OpenGL. 

[MAME](https://www.mamedev.org/) is a Arcade Machine Emulator.

[xemu](https://xemu.app/) is an original Xbox emulator.

[Xenia](https://github.com/xenia-project/xenia) is an Xbox 360 Emulator.

**Also checkout these subreddits for more great Game Emulators recommendations**
  
   - [r/emulation](https://www.reddit.com/r/emulation/)
   - [r/emulations](https://www.reddit.com/r/emulators/)
   - [r/RetroArch](https://www.reddit.com/r/RetroArch/)
   - [r/RetroPie](https://www.reddit.com/r/RetroPie/)
   - [r/DolphinEmulator](https://www.reddit.com/r/DolphinEmulator/)
   - [r/Citra](https://www.reddit.com/r/Citra/)
   - [r/cemu](https://www.reddit.com/r/cemu/)
   - [r/yuzu](https://www.reddit.com/r/yuzu/)
   - [r/OpenEmu](https://www.reddit.com/r/OpenEmu/)
   - [r/MAME](https://www.reddit.com/r/MAME/)
   - [r/EmuDev](https://www.reddit.com/r/EmuDev/)
   - [r/Roms](https://www.reddit.com/r/Roms/)

### Foundations/Projects

[Back to the Top](#table-of-contents)

[Matter](https://buildwithmatter.com/) is an open standard for smart home technology that lets your device work with any Matter-certified ecosystem using a single protocol. Matter comes from the [Connectivity Standards Alliance](https://csa-iot.org/), an organization of hundreds of companies(Amazon, Apple, Google, Comcast, Zigbee Alliance, and Connectivity Standards Alliance (CSA) creating products for the smart home.

[Open Source Hardware Association (OSHWA)](https://www.oshwa.org) is a non-profit organization that advocates for open-source hardware. It aims to act as a hub of open source hardware activity of all types while actively cooperating with other initiatives such as the TAPR Open Hardware License, open-source development groups at CERN, and the Open Source Initiative (OSI).

[The Open Connectivity Foundation](https://openconnectivity.org) is dedicated to ensuring secure interoperability for consumers, businesses and industries by delivering a standard communications platform, a bridging specification, an open source implementation and a certification program allowing devices to communicate regardless of form factor, operating system, service provider, transport technology or ecosystem.

[Raspberry Pi Foundation](https://www.raspberrypi.org/about/) is a UK-based charity with the mission to enable young people to realise their full potential through the power of computing and digital technologies. 

[OpenSSF(Open Source Security Foundation)](https://openssf.org/) is a cross-industry forum for a collaborative effort to improve open source software security. 

[OpenJS Foundation](https://openjsf.org/) is the premier home for critical open source JavaScript projects, including Appium, Dojo, jQuery, Node.js, and webpack, and 27 more.

[EdgeX Foundry](https://www.edgexfoundry.org) is a vendor-neutral project under the Linux Foundation. The initiative is aligned around a common goal: the simplification and standardization of the foundation for edge computing architectures in the Industrial IoT market, while still allowing the ecosystem to add significant value.

[Eclipse Foundation](https://www.eclipse.org) provides our global community of individuals and organizations with a mature, scalable and commercially-friendly environment for open source software collaboration and innovation.

### System Hardware

[Back to the Top](table-of-contents)
 
 * [Refurbished Servers on Amazon](https://www.amazon.com/refurbished-servers/s?k=refurbished+servers&rh=p_36%3A10000-60000&qid=1667083059&rnid=386442011&ref=sr_nr_p_36_2)
 * [Network Switches & Hubs on ebay](https://www.ebay.com/b/Enterprise-Network-Switches-Hubs/182091/bn_887002)
 * [Server Monkey](https://www.servermonkey.com/servers.html)
 * [The Server Store](https://www.theserverstore.com/)
 

#### CPUs

**Intel Processors(x86)**

[Back to the Top](table-of-contents)

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/198867859-20c9906d-4b0f-41b8-8ed5-cb3b8425c7fd.png">
  <br />
</p>

I recommend using Intel CPUs no older than the second generation of the Intel Core processors (Core i7, i5, i3) AKA **Sandy Bridge(Jan. 2011)** for those that want to utilize [Intel® Quick Sync Video](https://www.intel.com/content/www/us/en/architecture-and-technology/quick-sync-video/quick-sync-video-general.html). Though, if you're concerned about power efficiency(~5W idle) I would recommend 7th Generation or newer.

Also, I recommend using **[Intel® QuickAssist Technology (Intel® QAT)](https://www.intel.com/content/www/us/en/architecture-and-technology/intel-quick-assist-technology-overview.html)** a scalable, flexible, and extendable way to accelerate data encryption/decryption and compression for applications from networking to enterprise, cloud to storage, and content delivery to database. Available in 3rd Gen Intel® Xeon® Scalable Processors and Intel Atom® Processor C Series/P Series.
 
 * [Intel Celeron Processor N Series](https://ark.intel.com/content/www/us/en/ark/products/series/87282/intel-celeron-processor-n-series.html)
 * [Intel Atom Series](https://ark.intel.com/content/www/us/en/ark.html#@PanelLabel29035)
 * [Intel Pentium](https://ark.intel.com/content/www/us/en/ark.html#@PanelLabel29862)
 * [Intel i3](https://ark.intel.com/content/www/us/en/ark.html#@PanelLabel122139)
 * [Intel i5](https://ark.intel.com/content/www/us/en/ark.html#@PanelLabel122139)
 * [Intel i7](https://ark.intel.com/content/www/us/en/ark.html#@PanelLabel122139)
 * [Intel Xeon](https://ark.intel.com/content/www/us/en/ark.html#@PanelLabel595)

**AMD Processors(x86)**

[Back to the Top](table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/198867861-ff988ac9-a6f8-4db5-90e4-1f2d8c933fed.png">
  <br />
</p>

 * [AMD Athlon](https://www.amd.com/en/processors/athlon-pro)
 * [AMD Ryzen G-Series](https://cpuarchive.com/CPU/AMD/Ryzen)
 * [AMD Ryzen 3](https://cpuarchive.com/CPU/AMD/Ryzen)
 * [AMD Ryzen 5](https://cpuarchive.com/CPU/AMD/Ryzen)
 * [AMD Ryzen 7](https://cpuarchive.com/CPU/AMD/Ryzen)
 * [AMD Threadripper](https://www.amd.com/en/processors/threadripper-creators)


#### Devices

[Back to the Top](table-of-contents)

**Note: Will be adding more device soon!**

 * [Raspberry Pi](https://github.com/mikeroyal/Self-Hosting-Guide#raspberry-pi)
 * [Turing Pi 2](https://turingpi.com/)
 * [Home Assistant Yellow](https://www.home-assistant.io/blog/2021/09/13/home-assistant-yellow/)
 * [ZimaBoard](https://www.zimaboard.com/) 
 * [ODROID-H3 and H3+](https://ameridroid.com/products/odroid-h3)
 * [Intel® NUC Mini PCs](https://www.intel.com/content/www/us/en/products/details/nuc.html)
 * [Beelink mini PC](https://www.bee-link.com/)
 * [M1 Mac Mini](https://www.apple.com/mac-mini/) 
 * [Nexcom Industrial Computers](https://www.nexcom.com/Products/industrial-computing-solutions/industrial-fanless-computer/core-i-performance)
 * [Aeotec MultiSensor 7, 6-in-1 Zwave Sensors](https://www.amazon.com/dp/B08XHZP7NV)
 * [reTerminal Raspberry Pi (CM4 module) all-in-one board](https://www.seeedstudio.com/ReTerminal-with-CM4-p-4904.html) 
 * [KOOLCORE R1 - The smallest mini PC with 4 x 2.5G LANs](https://www.ikoolcore.com/products/ikoolcore)
 * [Khadas VIM1S](https://www.khadas.com/vim1s)
 * [Asustor DriveStor 4 NAS](https://www.asustor.com/product?p_id=71)
 * [TRENDnet TEG-S350 (2.5 GbE) Switch](https://www.amazon.com/TRENDnet-2-5GBASE-T-Compatible-10-100-1000Mbps-TEG-S350/dp/B08XWK4HNT)
 * [Storinator™](https://www.45drives.com/products/storage/) is a line of Ultra-Large, Direct-Wired storage Servers by [45Drives](https://www.45drives.com/).
 * [HL15 from 45HomeLab](https://store.45homelab.com/configure/hl15) is an open-source, open-platform, 15-bay homelab server. The HL15 features enterprise architecture and strength brought to a scale that works for the homelab. The server's direct-wired architecture can provide blazing fast transfer speed of up to 2GB per second. 
 * [LattePanda Sigma](https://www.lattepanda.com/lattepanda-sigma) is a powerful and compact x86 Windows single board computer (SBC). It features the 13th Intel® Core™ i5-1340P Rapter Lake (12-Core, 16-Thread) processor and 16GB Dual-Channel LPDDR5-6400MHz memory.
 * [Apex Storage X21](https://www.apexstoragedesign.com/apexstoragex21) is a storage solution that gives you have the freedom to choose system hardware thatworks best for you with the following benefits.
    * Host 21 x M.2 Gen 4 NVME SSD’s
    * 168 TB + Storage Per Card
    * 31 GBps Read/Write Speeds
    * Industry Leading IOPS
    * 100 PCIe 4.0 Lanes
    * Full UEFI/Secure Boot Support
 * [GL.iNet](https://www.gl-inet.com/) is a leading developer of OpenWrt Wi-Fi and IoT Network Solutions. They build Wi-Fi routers, IoT gateways and remote device management platforms for a wide range of scenarios. All their routers include powerful built-in firewall, Shadow also supports OpenVPN, WireGuard® and customized DNS server in order to level up your online security.
 * [Protectli Vault](https://protectli.com/) is a series of small computers that have firewalls with advanced firmware protection to keep your network safe. All Vaults are Opertaing System (OS) agnostic and support a variety of popular open source software distributions. Run a firewall like OPNsense, pfSense, or others. Also, run any hypervisor on your system.
 * [Espclicker](https://www.pricelesstoolkit.com/en/projects/32-espclicker.html) is a small device that you can use to integrate not IoT devices into your smart home setup, It connects directly to the push buttons of the device, which you want to control, and then simulates pressing them. You can simulate button clicks, hold time, and multiple clicks. 
 * [Pockethernet](https://pockethernet.com/) is a smartphone connected Ethernet network analyzer & cable tester that fits into your pocket. It helps any IT admin dealing with Ethernet network installation and maintenance. It lets you check the ethernet link, find cable faults, PoE voltage, VLAN, DHCP results and much more with the press of a button.
 * [$13 USD voice assistant remote for Home Assistant](https://www.home-assistant.io/voice_control/thirteen-usd-voice-remote/)
 * [ATOM ECHO](https://docs.m5stack.com/en/atom/atomecho) is a Programmable Smart Speaker based on the M5ATOM design. Music can be played using the BT (Bluetooth Technology) capabilities of the ESP32 from a mobile phone or tablet. The device could be programmed to access AWS, Azure, and other cloud platforms, using the built-in microphone and speaker for voice interaction. 
 
### Operating Systems

[Back to the Top](#table-of-contents)

**Creating a bootable media device(USB/MicroSD card)**

[Rufus](https://rufus.ie/) is a utility that helps format and create bootable USB flash drives.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/158471950-74640216-66ed-407b-a615-e643284ba0b8.png">
  <br />
  Rufus
</p>

**OR**

[Etcher](https://www.balena.io/etcher/) is an open source, cross-platform software that makes it easy to flash operating system images to a microSD card or USB device.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/157350348-e43ea5a2-2346-4b0b-acc0-fc3352c3d820.png">
  <br />
  Etcher UI
</p>

**A List of Operating Systems that are great for either settig up a personal Home Server or a Enterprise Server for your Organization/Company.**

[Home Assistant OS](https://home-assistant.io/hassio/) is a container-based system for managing your Home Assistant Core installation and related applications. The system is controlled via Home Assistant which communicates with the Supervisor. The Supervisor provides an API to manage the installation. This includes changing network settings or installing and updating software.

<h2 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177719719-9108f14f-9ca0-45e4-b1f5-55efaf1803e6.png">
  <br />
 Home Assistant OS 
</h2>

[Umbrel](https://umbrel.com/) is an OS for running a personal server in your home. It can Self-host open source apps like Nextcloud, Bitcoin node, and more. 

<h2 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/198820005-e10b3c23-f87e-4f3a-bbd2-efe74db3681f.png">
  <br />
  Umbrel
</h2>

[CasaOS](https://casaos.io/) is a simple, easy-to-use, elegant open-source Home Cloud system. 

<h2 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/198867868-bdf3c448-0c0d-49a2-be7b-c32ae5f2ad3a.png">
  <br />
  CasaOS
</h2>

[TrueNAS® CORE](https://www.truenas.com/truenas-core/) is the world's most popular storage OS because it gives you the power to build your own professional-grade storage system to use in a variety of data-intensive applications without any software costs. It's based on FreeBSD and Linux, using the OpenZFS file system. 

<h2 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/216557724-bf621a1e-01f6-477b-b71a-2675121d20e8.png">
  <br />
  TrueNAS CORE
</h2>

[Alpine Linux](https://www.alpinelinux.org/) is a security-oriented, lightweight Linux distribution based on musl libc and busybox.

 * [Alpine Linux Wiki](https://wiki.alpinelinux.org/wiki/Main_Page)

 * [Alpine Linux Community](https://alpinelinux.org/community)

#### Xfce4 Desktop

**Enable the [Community repository](https://wiki.alpinelinux.org/wiki/Enable_Community_Repository), then execute command:**

``apk add xfce4``

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/144766372-ec177b63-4d4d-4b00-aee6-889bc15a7597.png">
  <br />
  Alpine Linux Xfce
</p>


#### Mate Desktop

**Enable the [Community repository](https://wiki.alpinelinux.org/wiki/Enable_Community_Repository), then execute command:**

``apk add mate-desktop-environment``

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/144766373-b813b402-16cd-4a99-930a-ff893600f016.png">
  <br />
  Alpine Linux MATE
</p>


[Ubuntu](https://ubuntu.com/) is a modern open source operating system on Linux for the enterprise Server, Desktop, Cloud, and IoT developed by Canonical. 

 * [Ubuntu Server](https://ubuntu.com/download/server)
 
 * [Ubuntu for ARM](https://ubuntu.com/download/server/arm)
 
 * [Ubuntu for Raspberry Pi](https://ubuntu.com/raspberry-pi)

 * [Ubuntu Flavours](https://www.ubuntu.com/download/flavours) is for those that prefer an alternative desktop environment such as [KDE Plasma Desktop](https://kubuntu.org/), [MATE](https://ubuntu-mate.org/), [Xfce](https://xubuntu.org/), [LXQt](https://lubuntu.me/), [Budgie](https://ubuntubudgie.org/), and [UKUI](https://www.ubuntukylin.com/) you can download a Flavour for your preferred desktop environment and use that to install Ubuntu, pre-configured for the desktop environment of your choice.
 
<h3 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/164793005-67371e3c-d74d-4b40-9fd1-b9a71bd4172a.png">
  <br />
  Ubuntu 
</h3>

[Debian](https://www.debian.org/) is an operating system and a distribution of Free Software. It is maintained and updated through the work of many users who volunteer their time and effort.

<h3 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/129622953-4b379400-9145-4d5b-9572-bcda571894f4.png">
  <br />
  Debian 11 
</h3>
  
[Linux Mint](https://linuxmint.com/) is a modern, elegant, and comfortable open source operating system(based on Debian and Ubuntu), which is both powerful and easy to use for both new and advanced users. The flagsip version of Linux Mint uses the [Cinnamon desktop environment](https://cinnamon-spices.linuxmint.com/) similiar to Windows 7.

<h3 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/157350295-4c6b8ab5-17d2-4e2f-91ca-a111bcdb2a34.png">
  <br />
  Linux Mint 
</h3>

[Linux Mint Debian Edition (LMDE)](https://www.linuxmint.com/download_lmde.php) uses [Debian Bullseye](https://www.debian.org/) as the base for a very stable and rock solid user experience with the Cinnamon desktop.

<h3 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/157350295-4c6b8ab5-17d2-4e2f-91ca-a111bcdb2a34.png">
  <br />
  Linux Mint Debian Edition (LMDE)
</h3>

**[Pop!_OS](https://pop.system76.com)** created by [System76](https://system76.com).

<h3 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/142779593-390dfd58-a246-4299-baf2-adf0207da696.png">
  <br />
Pop!_OS 
</h3>

[Fedora Linux](https://getfedora.org/) is a polished, easy to use operating system for laptop & desktop computers, with a complete set of tools for developers and makers of all kinds. The OS serves as the foundation for which you can scale existing apps and roll out emerging technologies across bare-metal, virtual, container, and all types of cloud environments.

 * [Fedora Spins](https://spins.fedoraproject.org/) is for those that prefer an alternative desktop environment such as KDE Plasma Desktop, MATE; or Xfce, you can download a spin for your preferred desktop environment and use that to install Fedora, pre-configured for the desktop environment of your choice.

 * [Fedora Server](https://getfedora.org/) is a powerful, flexible operating system that includes the best and latest datacenter technologies. It puts you in control of all your infrastructure and services.

 * [Fedora ARM](https://arm.fedoraproject.org/) is an initiative to bring versions of Fedora tailored for running on ARM-based systems.

 * [Fedora Silverblue](https://silverblue.fedoraproject.org/) is a variant of the Fedora Workstation that uses rpm-ostree to provide an immutable OS image with reliable updates and easy rollbacks.

 * [Fedora Kinoite](https://kinoite.fedoraproject.org/) is an immutable desktop operating system. It aims to be extremely stable and reliable. It also aims to be an excellent platform for developers and for those using container-focused workflows. Kinoite is a variant of the Fedora KDE Spin.

 * [Fedora CoreOS](https://getfedora.org/coreos?stream=stable) is an automatically-updating, minimal operating system for running containerized workloads securely and at scale.

<h3 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/142779592-8b70c81e-ac10-4bb3-91b5-efe25fa9afb4.png">
  <br />
Fedora Linux
</h3>


[CentOS Stream](https://www.centos.org/centos-stream/) is a continuously delivered distro(uses the Fedora OS base) that tracks just ahead of Red Hat Enterprise Linux (RHEL) development, positioned as a midstream between Fedora Linux and RHEL.

<h3 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/145488524-ebfd666a-bf90-43d8-bc41-8c363e4e233a.png">
  <br />
 CentOS Stream
</h3>

[Red Hat® Enterprise Linux® (RHEL)](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux) the world's leading enterprise Linux platform. The OS serves as the foundation for which you can scale existing apps and roll out emerging technologies across bare-metal, virtual, container, and all types of cloud environments.

<h3 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/171923060-f9276330-5d4d-4d6a-9d41-99b9972f0cb2.png">
  <br />
Red Hat Enterprise Linux Desktop
</h3>


[AlmaLinux](https://almalinux.org/) is an open source enterprise-ready Linux distribution forked from Red Hat Enterprise Linux(RHEL). It's a very stable/solid operating system especially for production envrionments such as servers, though, you can also install a GUI on AlmaLinux and use it as a desktop OS. It was founded by the team behind the [CloudLinux OS](https://www.cloudlinux.com/all-products/product-overview/cloudlinuxos).

 * [AlmaLinux Wiki](https://wiki.almalinux.org/)

 * [Migrate from CentOS 8](https://github.com/AlmaLinux/almalinux-deploy)

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/124993377-24ab7800-dff9-11eb-90b4-4a121eff6de3.png">
 <br />	
 AlmaLinux Desktop Setup and Install
 </p>


[Rocky Linux](https://rockylinux.org/) is a community enterprise operating system designed to be 100% bug-for-bug compatible and forked from Red Hat Enterprise Linux(RHEL) now that its [downstream partner(Red Hat) has shifted direction](https://blog.centos.org/2020/12/future-is-centos-stream/). 

 * [Rocky Linux Wiki](https://wiki.rockylinux.org/)

 * [Rocky Linux Documentation](https://docs.rockylinux.org/)

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/124993391-2b39ef80-dff9-11eb-9197-40c84c7f385f.png">
  <br />
  Rocky Linux Desktop
</p>

[SUSE](https://www.suse.com/) is a leading Linux OS most adaptable Linux operating system and the only open Kubernetes management platform thanks to their acquistion of [Rancher](https://rancher.com/). They also developer of [SUSE Linux Enterprise](https://www.suse.com/download/) and the primary sponsor of the community-supported [openSUSE Project](https://software.opensuse.org/), which develops the openSUSE Linux distribution.

* [openSUSE Leap](https://en.opensuse.org/Portal:Leap) is a brand new way of building openSUSE and is new type of a hybrid Linux distribution. Leap uses source from SUSE Linux Enterprise (SLE), which gives Leap a level of stability unmatched by other Linux distributions, and combines that with community developments to give users, developers and sysadmins the best stable Linux experience available. 

 * [openSUSE Tumbleweed](https://en.opensuse.org/Portal:Tumbleweed) is a pure rolling release version of openSUSE containing the latest "stable" versions of all software instead of relying on rigid periodic release cycles. The project does this for users that want the newest stable software. 

 * [openSUSE Kubic](https://get.opensuse.org/kubic/) is a multi-purpose Standalone & Kubernetes Container Operating System based on openSUSE MicroOS. Kubic uses kubeadm to provide an easy way of configuring a Kubernetes cluster across multiple machines, while our MicroOS base keeps your operating system updated automatically, with fully atomic rollbacks if required.

 * [openSUSE MicroOS](https://get.opensuse.org/microos/) is a M icro Service OS providing Transactional (Atomic) Updates upon a read-only btrfs root filesystem. It's designed to host container workloads with automated administration & patching.
 
  <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/145488499-6aae18fa-1dab-4a1f-96dc-fcd73fec5f19.png">
  <br />
</p>

 <h3 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/110253144-9f766080-7f3d-11eb-9a01-2ac6738637e9.png">
  <br />
  SUSE Linux Enterprise 12
</h3>

<h3 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/110253145-a00ef700-7f3d-11eb-9b5c-d3cee3cbce84.png">
  <br />
  openSUSE 
</h3>

[NixOS](https://nixos.org/) is a Linux distribution built on top of the [Nix package manager](https://nixos.wiki/wiki/Nix). It has tools dedicated to DevOps and deployment tasks. [NixOS Guide](https://github.com/mikeroyal/NixOS-Guide)

 * [Nix Tour](https://nixcloud.io/tour/) is an interactive tour that uses the actual package manager to learn you the language by example, in the browser.

 * [Nix](https://nixos.wiki/wiki/Nix) is a package manager and build system that parses reproducible build instructions specified in the [Nix Expression Language](https://nixos.wiki/wiki/Nix_Expression_Language), is a pure functional language with lazy evaluation. Nix expressions are pure functions taking dependencies as arguments and producing derivation specifying a reproducible build environment for the package. Nix stores the results of the build in unique addresses specified by a hash of the complete dependency tree, creating an immutable package store that allows for atomic upgrades, rollbacks and concurrent installation of different versions of a package, essentially eliminating [dependency hell](https://en.wikipedia.org/wiki/Dependency_hell).

 * [Nix Expression Language](https://nixos.wiki/wiki/Nix_Expression_Language) is a pure, lazy, functional language. Purity means that operations in the language don't have side-effects (for instance, there is no variable assignment). The language is not a full-featured, general purpose language. Its main job is to describe packages, compositions of packages, and the variability within packages.

 * [Nixpkgs](https://nixos.wiki/wiki/Nixpkgs) is the largest repository of [Nix](https://nixos.wiki/wiki/Nix) packages(over 80,000 packages) and [NixOS](https://nixos.wiki/wiki/NixOS) modules. The repository is [hosted on GitHub](https://github.com/nixos/nixpkgs) and maintained by the community, with official backing from the [NixOS Foundation](https://nixos.org/). Additionally, checkout [Language-specific package helpers](https://nixos.wiki/wiki/Language-specific_package_helpers) and [Alternative Package Sets](https://nixos.wiki/wiki/Alternative_Package_Sets).

 * [NixOS Packages Search](https://search.nixos.org/packages) is a tool for searching through NixOS packages.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/173939766-8972583c-855e-4a9b-b9f1-761b60ea255e.png">
  <br />
  NixOS Packages Search
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/173939768-31847173-88ab-45f0-8501-0980d1a2a29e.png">
  <br />
  NixOS Desktop with the new Calamares Installer
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/128645111-b2a92dd2-f246-4df0-b05c-5b0ffce05448.png">
  <br />
  NixOS with the Plasma Desktop
</p>

### BSD

[Back to the Top](#table-of-contents)

[FreeBSD](https://www.freebsd.org/) is an Unix-like operating system used to power modern servers, desktops, and embedded platforms. A large community has continually developed it for more than thirty years. Its advanced networking, security, and storage features have made FreeBSD the platform of choice for many of the busiest web sites and most pervasive embedded networking and storage devices.

<p align="center">
<img src="https://user-images.githubusercontent.com/45159366/125211868-67ba5500-e25e-11eb-86eb-440fbaf28b7d.png">
<br />
</p>

**FreeBSD Software ports. Source: [FreeBSD Software](https://www.freebsdsoftware.org)**

[OpenBSD](https://www.openbsd.org/) is a security-focused, free and open-source, Unix-like operating system based on the Berkeley Software Distribution. It comes with a secure minimal firewall, webserver, mailserver, and an optional graphical desktop.

[NetBSD](https://netbsd.org/)  is a free, fast, secure, and highly portable Unix-like Open Source operating system. It is available for a wide range of platforms, from large-scale servers and powerful desktop systems to handheld and embedded devices.

 * [NetBSD Documentation](http://netbsd.org/docs/)

[DragonFly BSD](https://www.dragonflybsd.org/) is a free and open-source Unix-like operating system forked from FreeBSD 4.8.

 * [DragonFly Documentation](https://www.dragonflybsd.org/docs/)

### The BSD Desktop for the average user

[GhostBSD](https://www.ghostbsd.org/) is a simple desktop-oriented operating system based on FreeBSD with MATE, OpenRC and OS packages for simplicity. GhostBSD has a selection of commonly used software preinstalled and required to start using it to its full potential.

 * [GhostBSD Wiki](https://wiki.ghostbsd.org/index.php/Main_Page)

 * [GhostBSD Community](https://forums.ghostbsd.org/index.php)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/125211866-66892800-e25e-11eb-985b-26588de87615.png">
  <br />
</p>

**GhostBSD Desktop. Source: [GhostBSD](https://www.ghostbsd.org/)**


### Storage

 [Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

  -[Storage Reference Guide by Storage Review](https://www.storagereview.com/storage-reference-guide)
  
  - [Western Digital Hard Drives Storage size range 2TB up to 20TB](https://www.westerndigital.com/c/internal-drives.0_TB-4_TB.11_TB-20_TB.5_TB-10_TB.hard_drives)
 
  - [Seagate Hard Drives Storage size range 2TB up to 18TB](https://www.seagate.com/internal-hard-drives/hdd/)
 
  - [Hard Drives Storage size range 2TB up to 20TB from Bestbuy](https://www.bestbuy.com/site/searchpage.jsp?id=pcat17071&qp=harddrivesizerange_facet%3DStorage%20Capacity~2TB%20-%203TB%5Eharddrivesizerange_facet%3DStorage%20Capacity~4TB%20-%207TB%5Eharddrivesizerange_facet%3DStorage%20Capacity~8TB%20-%2011TB%5Eharddrivesizerange_facet%3DStorage%20Capacity~12TB%20or%20More%5Einternalorexternal_facet%3DInternal%20Or%20External~Internal&st=hard+drive)
 
  - [Hard Drives Storage size range 1TB up to 20TB on Newegg](https://www.newegg.com/p/pl?d=hard+drives&N=600003298%20600003311%20600003316%20600003299%20600543907%20600003300%20601331745%20600083978%20600217643%20600486069%20600490667%20600376735%20601192404%20601398066%20601355746%20601334339%20601322010%20600376738%20600003341%20600003347%20100167523)

  - [Hard Drives Storage size range 1TB up to 18TB on Amazon](https://www.amazon.com/s?k=hard+drives&i=computers&rh=n%3A1254762011%2Cp_n_feature_two_browse-bin%3A5446812011%7C5446813011%7C5446815011%7C5446816011%7C7817230011%2Cp_n_feature_keywords_six_browse-bin%3A6158683011&s=review-rank&dc&qid=1653712565&rnid=562234011&ref=sr_st_review-rank)

**Useful Tools for Storage Management**

[Scrutiny](https://github.com/AnalogJ/scrutiny) is a WebUI for smartd Hard Drive S.M.A.R.T Monitoring, Historical Trends & Real World Failure Thresholds.

[smartd](https://www.smartmontools.org/) is SMART Disk Monitoring Daemon for Linux. It controls and monitors storage systems using the Self-Monitoring, Analysis and Reporting Technology System (SMART) built into most modern ATA/SATA, SCSI/SAS and NVMe disks. In many cases, these utilities will provide advanced warning of disk degradation and failure.
  
[DUA (Disk Usage Analyzer)](https://lib.rs/crates/dua-cli) is a tool to conveniently learn about the usage of disk space of a given directory. It's parallel by default and will max out your SSD, providing relevant information as fast as possible. Optionally delete superfluous data, and do so more quickly than rm.

[Perkeep](https://github.com/perkeep/perkeep) is a set of open source formats, protocols, and software for modeling, storing, searching, sharing and synchronizing data. It can be easily accessed via a phone, browser or FUSE filesystem.

[duf](https://github.com/muesli/duf) is a Disk Usage/Free Utility for Linux, BSD, macOS & Windows.

[Dirstat-rs](https://github.com/scullionw/dirstat-rs) is a fast, cross-platform disk usage CLI, similar to [Windirstat](https://windirstat.net/). 

[Dutree](https://github.com/nachoparker/dutree) is a tool to analyze file system usage written in Rust.

[Shufflecake](https://shufflecake.net/) is a tool for Linux that allows to create multiple hidden volumes on a storage device in such a way that it is very difficult, even under forensic inspection, to prove the existence of such volumes.

[btdu](https://github.com/CyberShadow/btdu) is a sampling disk usage profiler for btrfs.
 
[Btrfs maintenance toolbox](https://github.com/kdave/btrfsmaintenance) is a set of scripts supplementing the btrfs filesystem and aims to automate a few maintenance tasks. This means the scrub, balance, trim or defragmentation.

### File systems

[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

* [FSArchiver](https://www.fsarchiver.org/) is a system tool that allows you to save the contents of a file system to a compressed archive file. The file system can be restored on a partition which has a different size and it can be restored on a different file system. 

[WekaFS](https://www.weka.io/resources/datasheet/wekafs-the-weka-file-system/) is the world's fastest shared parallel file system and delivers unmatched performance at ANY scale while offering the same enterprise features and benefits of traditional storage. It meets all storage challenges, delivering 10x the performance of legacy network attached storage (NAS) systems and 3x the performance of local server storage.

[GlusterFS](https://www.gluster.org/) is a free and open source scalable network filesystem. Gluster is a scalable network filesystem. Using common off-the-shelf hardware, you can create large, distributed storage solutions for media streaming, data analysis, and other data- and bandwidth-intensive tasks.

[Ceph](https://ceph.io/) is a software-defined storage solution designed to address the object, block, and file storage needs of data centers adopting open source as the new norm for high-growth block storage, object stores and data lakes. Ceph provides enterprise scalable storage while keeping [CAPEX](https://corporatefinanceinstitute.com/resources/knowledge/modeling/how-to-calculate-capex-formula/) and [OPEX](https://www.investopedia.com/terms/o/operating_expense.asp) costs in line with underlying bulk commodity disk prices.

[Hadoop Distributed File System (HDFS)](https://www.ibm.com/analytics/hadoop/hdfs) is a distributed file system that handles large data sets running on commodity hardware. It is used to scale a single Apache Hadoop cluster to hundreds (and even thousands) of nodes. HDFS is one of the major components of Apache Hadoop, the others being [MapReduce](https://www.ibm.com/analytics/hadoop/mapreduce) and [YARN](https://hadoop.apache.org/docs/current/hadoop-yarn/hadoop-yarn-site/YARN.html).

[ZFS](https://docs.oracle.com/cd/E19253-01/819-5461/zfsover-2/) is an enterprise-ready open source file system and volume manager with unprecedented flexibility and an uncompromising commitment to data integrity.

  * [ZFSBootMenu](https://zfsbootmenu.org/) is a Linux bootloader that attempts to provide an experience similar to the FreeBSD bootloader. It takes advantage of ZFS features, it allows a user to have multiple “boot environments” (with different distros, for example), manipulate snapshots before booting, and even bootstrap a system installation via ```zfs recv```.

[OpenZFS](https://openzfs.org/wiki/Main_Page ) is an open-source storage platform. It includes the functionality of both traditional file systems and volume manager. It has many advanced features including:

  - Protection against data corruption.
  - Integrity checking for both data and metadata.
  - Continuous integrity verification and automatic "self-healing" repair.

[Btrfs](https://btrfs.wiki.kernel.org/index.php/Main_Page) is a modern copy on write (CoW) filesystem for Linux aimed at implementing advanced features while also focusing on fault tolerance, repair and easy administration. Its main features and benefits are:

  - Snapshots which do not make the full copy of files
  - RAID - support for software-based RAID 0, RAID 1, RAID 10
  - Self-healing - checksums for data and metadata, automatic detection of silent data corruptions
  
[Composefs](https://github.com/containers/composefs) is a native Linux file system designed to help sharing filesystem contents, as well as ensuring said content is not modified. The initial target usecase are container images and ostree commits.
  
[MergerFS](https://github.com/trapexit/mergerfs) is a union filesystem geared towards simplifying storage and management of files across numerous commodity storage devices. It is similar to mhddfs, unionfs, and aufs.

**MergerFS Features**

  - Configurable behaviors / file placement
  - Ability to add or remove filesystems at will
  - Resistance to individual filesystem failure
  - Support for extended attributes (xattrs)
  - Support for file attributes (chattr)
  - Runtime configurable (via xattrs)
  - Works with heterogeneous filesystem types
  - Moving of file when filesystem runs out of space while writing
  - Ignore read-only filesystems when creating files
  - Turn read-only files into symlinks to underlying file
  - Hard link copy-on-write / CoW
  - Support for POSIX ACLs
  
[Proxmox Cluster File System (PMXCFS)](https://pve.proxmox.com/wiki/Cluster_Manager) is a File System used to transparently distribute the cluster configuration to all cluster nodes.

[UnionFS](https://unionfs.filesystems.org/) is a filesystem service for Linux, FreeBSD and NetBSD which implements a union mount for other file systems. It allows files and directories of separate file systems, known as branches, to be transparently overlaid, forming a single coherent file system. 

[OverlayFS](https://www.kernel.org/doc/html/latest/filesystems/overlayfs.html) is a modern union filesystem that is similar to [AUFS](https://en.wikipedia.org/wiki/Aufs), but faster and with a simpler implementation. It's typically used on systems running on embed devices, like OpenWRT, where is useful to preserve a basic set of configurations and at the same time allowing the user to perform modifications.
  
[Bcachefs](https://bcachefs.org/) is an advanced new filesystem for Linux, with an emphasis on reliability and robustness and the complete set of features one would expect from a modern filesystem. Scalability has been tested to 50+ TB, will eventually scale far higher. 

[Squashfs](https://www.kernel.org/doc/html/latest/filesystems/squashfs.html) is a compressed read-only filesystem for Linux. It uses zlib, lz4, lzo, or xz compression to compress files, inodes and directories. Inodes in the system are very small and all blocks are packed to minimize data overhead.

[SeaweedFS](https://github.com/seaweedfs/seaweedfs) is a fast distributed storage system for blobs, objects, files, and data lake, for billions of files! Blob store has O(1) disk seek, cloud tiering. Filer supports Cloud Drive, cross-DC active-active replication, Kubernetes, POSIX FUSE mount, S3 API, S3 Gateway, Hadoop, WebDAV, encryption, Erasure Coding. 

[CubeFS](https://cubefs.io/) is a cloud native distributed storage platform. It's commonly used as the storage infrastructure for online applications, database or data processing services and machine learning jobs orchestrated by Kubernetes.

[Apple File System (APFS)](https://support.apple.com/guide/disk-utility/file-system-formats-available-in-disk-utility-dsku19ed921c/mac) is  the default file system for Mac computers using macOS 10.13 or later, features strong encryption, space sharing, snapshots, fast directory sizing, and improved file system fundamentals.

[NTFS(New Technology File System)](https://docs.microsoft.com/en-us/windows-server/storage/file-server/ntfs-overview) is the primary file system for recent versions of Windows and Windows Server—provides a full set of features including security descriptors, encryption, disk quotas, and rich metadata, and can be used with Cluster Shared Volumes (CSV) to provide continuously available volumes that can be accessed simultaneously from multiple nodes of a failover cluster.

[exFAT(Extended File Allocation Table )](https://docs.microsoft.com/en-us/windows/win32/fileio/exfat-specification) is the file system that was the successor to FAT32 in the FAT family of file systems. It was optimized for flash memory such as USB flash drives and SD cards.

### Books
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

  - [Self-hosted Cookbook](https://github.com/tborychowski/self-hosted-cookbook) is a cookbook, for docker-compose based recipes, for self-hosted applications and services. 
  
  - [Geek's Cookbook](https://github.com/geek-cookbook/geek-cookbook) is a collection of guides for establishing your own highly-available "private cloud" and using it to run self-hosted services such as GitLab, Plex, NextCloud, etc. 
 
  - [Database Books(PDFs)](https://github.com/miollek/Free-Database-Books)
  
### Podcasts
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

  
  - [Self-Hosted Podcast](https://selfhosted.show/) is a chat show between Chris and Alex two long-time "self-hosters" who share their lessons and take you along for the journey as they learn new ones. 
  
  - [Self-Hosted SRE(Site Reality Engineer) Podcast](https://sshsre.fireside.fm/) is a feed to say thank you to our Self-Hosted Site Reality Engineers!
  
  -  [Home Assistant Podcast](https://hasspodcast.io) is a biweekly podcast with the latest news and interesting guests.

### YouTube Channels
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

  - [Jeff Geerling](https://www.youtube.com/c/JeffGeerling)
  
  - [Level1Techs](https://www.youtube.com/c/Level1Techs)
 
  - [Open Source is Awesome](https://www.youtube.com/c/AwesomeOpenSource)
  
  - [Self-Hosted Show by Jupiter Broadcasting](https://www.youtube.com/watch?v=XBhhVHVQ148&list=PLUW3LUwQvegxit4XMxUNW3qrRFmgP_aaT)
 
  - [Techno Tim](https://www.youtube.com/c/TechnoTimLive)
 
  - [Raid Owl](https://www.youtube.com/c/RaidOwl)
  
  - [NextCloud](https://www.youtube.com/c/Nextcloud)
  
  - [Raspberry Pi](https://www.youtube.com/c/raspberrypi)
  
  - [Wolfgang's Channel](https://www.youtube.com/c/WolfgangsChannel)
  
  - [Pro Tech Show](https://www.youtube.com/c/ProTechShow)
  
  - [Geeked](https://www.youtube.com/c/GeekedTV)
  
  - [The Tinker Dad](https://www.youtube.com/c/TheTinkerDad)
  
  - [DB Tech](https://www.youtube.com/c/DBTechYT)
  
  - [The Digital Life](https://www.youtube.com/c/TheDigitalLifeTech)
 
  - [censiCLICK](https://www.youtube.com/c/censiCLICK)
  
  - [Home Network Geek](https://www.youtube.com/channel/UCCniXOLmZ85FHN8c8K_c0LA/featured)
  
  
### Tutorials & Resources
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

  - [Awesome-SelfHosted](https://github.com/awesome-selfhosted/awesome-selfhosted) is a directory of free software solutions and web applications which can be hosted locally.
  
  - [Awesome Sysadmin](https://github.com/awesome-foss/awesome-sysadmin) is a curated list of amazingly awesome open source sysadmin resources.
  
  - [Personal Security Checklist](https://github.com/Lissy93/personal-security-checklist) is a curated checklist of 300+ tips for protecting digital security and privacy in 2022.

  - [Awesome Privacy](https://github.com/Lissy93/awesome-privacy) is acurated list of privacy & security-focused software and services. 
 
  - [Perfect Media Server](https://perfectmediaserver.com/) is a project aim is to share knowledge and information about building an open-source media server. It was created by [Alex Kretzschmar AKA ironicbadger](https://github.com/ironicbadger).
  
  - [/r/Selfhosted Official Wiki](https://wiki.r-selfhosted.com/getting-started/how-to-self-host/)
  
  - [45Drives Knowledge Base](https://knowledgebase.45drives.com/) is an affordable enterprise storage solutions for any data size - large or small. It provides high-performance, high-capacity storage servers and data destruction solutions for all industries.

  - [Self-hosting by any tech docs](https://tech.anytype.io/how-to/self-hosting)
  
  - [Noted - Self Hosted App and Product Reviews](https://noted.lol/)

  - [How I fell into the self-hosting rabbit hole in 2021](https://www.windowscentral.com/self-hosting-2021)
  
  - [The (hardware) key to making phishing defense seamless with Cloudflare Zero Trust and Yubico](https://blog.cloudflare.com/making-phishing-defense-seamless-cloudflare-yubico/)
  
  - [Shelly 2.5: Flash ESPHome Over The Air](https://savjee.be/blog/shelly-2.5-flash-esphome-over-the-air/)
  
  - [HDMI Distribution over your Home Network? Low-Cost HDMI Matrix using IP-Based Hardware](https://www.apalrd.net/posts/2022/hdmi_ip/)
  
  - [Microsecond accurate NTP with a Raspberry Pi and PPS GPS](https://austinsnerdythings.com/2021/04/19/microsecond-accurate-ntp-with-a-raspberry-pi-and-pps-gps/)

  - [Deploy Your Self-Hosted Mattermost Server](https://mattermost.com/deploy/)
  
  - [Monitor your Internet with a Raspberry Pi by Jeff Geerling](https://www.jeffgeerling.com/blog/2021/monitor-your-internet-raspberry-pi)

  -[Storage Reference Guide by Storage Review](https://www.storagereview.com/storage-reference-guide)
  
  - [NextCloud Migration Guide](https://nextcloud.com/migration/)
  
  - [GitLab self-managed subscription](https://docs.gitlab.com/ee/subscriptions/self_managed/)
  
  - [Proxmox VE Training Courses](https://www.proxmox.com/en/training)
  
  - [Self-Hosted GitLab with CodeFlow](https://www.getcodeflow.com/self-hosted-gitlab.html)
  
  - [Self-host Appsmith in Just a Few Minutes on Digital Ocean AppSmith](https://www.appsmith.com/blog/self-host-appsmith-in-just-a-few-minutes-on-digital-ocean)
  
  - [Linode Guides & Tutorials](https://www.linode.com/docs/guides/)
  
  - [Linode Beginner's Guide](https://www.linode.com/docs/guides/linode-beginners-guide/)
  
  - [Access a Pi-hole or Raspberry Pi from anywhere | Tailscale](https://tailscale.com/kb/1114/pi-hole/)
  
  - [Tailscale on Kubernetes | Tailscale](https://tailscale.com/kb/1185/kubernetes/)
  
  - [Tailscale on Proxmox host | Tailscale](https://tailscale.com/kb/1133/proxmox/)
  
  - [Configuring Linux DNS | Tailscale](https://tailscale.com/kb/1188/linux-dns/)
  
  - [Run a private Minecraft server with Tailscale | Tailscale](https://tailscale.com/kb/1137/minecraft/)
  
  - [Set up a dogcam with Tailscale, Raspberry Pi, and Motion | Tailscale](https://tailscale.com/kb/1076/dogcam/)
  
  - [Defined Networking is Open for Business by Ryan Huber](https://www.defined.net/blog/open-for-business/)
  
  - [Automating Host Creation with the API](https://docs.defined.net/guides/automating-host-creation/)
  
  - [Azure Self-hosted gateway overview](https://docs.microsoft.com/en-us/azure/api-management/self-hosted-gateway-overview)
  
  - [Create and configure a self-hosted integration runtime for Azure Data Factory and Synapse pipelines](https://docs.microsoft.com/en-us/azure/data-factory/create-self-hosted-integration-runtime?tabs=data-factory)

  - [Run a self-hosted agent in Docker - Azure Pipelines | Microsoft Docs](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/docker)

  - [Azure DevOps Self Hosted](https://github.com/Azure/DevOps-Self-Hosted)
  
 ### Subreddits
 [Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)
  
  - [r/Selfhosted](https://www.reddit.com/r/selfhosted/)
  - [r/Webhosting](https://www.reddit.com/r/webhosting/)
  - [r/NextCloud](https://www.reddit.com/r/NextCloud/)
  - [r/HomeServer](https://www.reddit.com/r/HomeServer/)
  - [r/Homeassistant](https://www.reddit.com/r/homeassistant/)
  - [r/Homebridge](https://www.reddit.com/r/homebridge/)
  - [r/HomeKit](https://www.reddit.com/r/HomeKit/)
  - [r/SmartThings](https://www.reddit.com/r/SmartThings/)
  - [r/Proxmox](https://www.reddit.com/r/Proxmox/)
  - [r/Tailscale](https://www.reddit.com/r/Tailscale/)
  - [r/WireGuard](https://www.reddit.com/r/WireGuard/)
  - [r/Adguard](https://www.reddit.com/r/Adguard/)
  - [r/Pihole](https://www.reddit.com/r/pihole/)
  - [r/Raspberry_pi](https://www.reddit.com/r/raspberry_pi/)
  - [r/RASPBERRY_PI_PROJECTS](https://www.reddit.com/r/RASPBERRY_PI_PROJECTS/)
  - [r/RetroPie](https://www.reddit.com/r/RetroPie/)
  - [r/Arduino](https://www.reddit.com/r/arduino/)
  - [r/ArduinoProjects](https://www.reddit.com/r/ArduinoProjects/)
  - [r/Opensource](https://www.reddit.com/r/opensource/)
  - [r/Devops](https://www.reddit.com/r/devops/)
  - [r/Kubernetes](https://www.reddit.com/r/kubernetes/)
  - [r/Docker](https://www.reddit.com/r/docker/)
  - [r/Portainer](https://www.reddit.com/r/portainer/)
  - [r/Ansible](https://www.reddit.com/r/ansible/)
  - [r/Terraform](https://www.reddit.com/r/Terraform/)
  - [r/CloudFlare](https://www.reddit.com/r/CloudFlare/)
  - [r/Homeautomation](https://www.reddit.com/r/homeautomation/)
  - [r/HomeNetworking](https://www.reddit.com/r/HomeNetworking/)
  - [r/Homelab](https://www.reddit.com/r/homelab/)
  - [r/Synology](https://www.reddit.com/r/synology/)
  - [r/unRAID](https://www.reddit.com/r/unRAID/)
  - [r/QNAP](https://www.reddit.com/r/qnap/)
  - [r/OpenWrt](https://www.reddit.com/r/openwrt/)
  - [r/Smarthome](https://www.reddit.com/r/smarthome/)
  - [r/TpLink](https://www.reddit.com/r/TpLink/)
  - [r/DataHoarder](https://www.reddit.com/r/DataHoarder/)
  - [r/ZFS](https://www.reddit.com/r/zfs/)
  - [r/PFSENSE](https://www.reddit.com/r/PFSENSE/)
  - [r/OpenMediaVault](https://www.reddit.com/r/OpenMediaVault/)
 

# WireGuard
[Back to the Top](#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/147891038-00f57362-e843-4bfb-be31-606c954d4e6c.png">
  <br />
</p>

### What is WireGuard?

[Back to the Top](#table-of-contents)

[WireGuard®](https://www.wireguard.com/) is a straight-forward, fast and modern VPN that utilizes state-of-the-art cryptography. It aims to be faster, simpler, leaner, and more useful than IPsec while avoiding the massive headache. WireGuard is designed as a general-purpose VPN for running on embedded interfaces and super computers alike, fit for many circumstances. Initially released for the Linux kernel, it is now cross-platform (Windows, macOS, BSD, iOS, Android) and widely deployable. 

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190848622-d1c8b109-f08c-4a89-b43d-816c510e4f2e.png">
  <br />
</p>

### What is Tailscale?

[Back to the Top](#table-of-contents)

[Tailscale](https://github.com/tailscale) is a WireGuard-based app that makes secure, private networks easy for teams of any scale. It works like an [overlay network](https://tailscale.com/blog/how-tailscale-works/) between the computers of your networks using all kinds of [NAT traversal sorcery](https://tailscale.com/blog/how-nat-traversal-works/).

 * [Tailscale Terraform Provider](https://github.com/tailscale/terraform-provider-tailscale)
 * [Tailscale Docker extension](https://github.com/tailscale/docker-extension)
 * [Tailscale Synology](https://github.com/tailscale/tailscale-synology)


<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/191301110-4c688e1b-da46-4f19-a25f-c285d66403e5.png">
  <br />
</p>

How NAT Traversal works on a Home router. Credit: [Tailscale](https://tailscale.com/blog/how-nat-traversal-works/).

[Headscale](https://github.com/juanfont/headscale) is an open source, self-hosted implementation of the Tailscale coordination server.

### What is Netmaker?

[Back to the Top](#table-of-contents)

[Netmaker](https://www.netmaker.org/) is a tool that enables you to create relays, gateways, full VPN meshes, and even zero trust networks. It's fully configurable to let you maximize the power of Wireguard.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/191140241-4ad71f9a-7f1f-4d93-be3a-2d625b144dca.png">
  <br />
</p>

NetMaker Architecture. Credit: [Netmaker](https://netmaker.readthedocs.io/en/v0.7.2/index.html).

### WireGuard Tools
[Back to the Top](#table-of-contents)

[Wiretrustee](https://wiretrustee.com/) is a WireGuard®-based mesh network that connects your devices into a single private network.

[Wireguard Manager](https://github.com/complexorganizations/wireguard-manager) is a tool that enables you to build your own vpn under a minute.

[Tailscale](https://github.com/tailscale) is a WireGuard-based app that makes secure, private networks easy for teams of any scale. It works like an [overlay network](https://tailscale.com/blog/how-tailscale-works/) between the computers of your networks using all kinds of [NAT traversal sorcery](https://tailscale.com/blog/how-nat-traversal-works/).

[Headscale](https://github.com/juanfont/headscale) is an open source, self-hosted implementation of the Tailscale coordination server.

[Firezone](https://firezone.dev/) is a self-hosted WireGuard®-based VPN server and Linux firewall.

[NetBird](https://netbird.io/) is an open-source VPN management platform built on top of WireGuard® making it easy to create secure private networks for your organization or home.

[Mistborn](https://gitlab.com/cyber5k/mistborn) is a secure platform for easily standing up and managing your own cloud services: including firewall, ad-blocking, and multi-factor WireGuard VPN access.

[Mistborn CLI](https://gitlab.com/cyber5k/mistborn-cli) is a Command-line interface for [Mistborn](https://gitlab.com/cyber5k/mistborn).

[BoringTun](https://github.com/cloudflare/boringtun) is an implementation of the WireGuard® protocol designed for portability and speed. It's successfully deployed on millions of [iOS](https://apps.apple.com/us/app/1-1-1-1-faster-internet/id1423538627) and [Android](https://play.google.com/store/apps/details?id=com.cloudflare.onedotonedotonedotone&hl=en_US) consumer devices as well as thousands of Cloudflare Linux servers.

[PiVPN](https://pivpn.io/) is the simplest VPN installer, designed for [Raspberry Pi](https://www.raspberrypi.com).

[Algo VPN](https://github.com/trailofbits/algo) is a set of Ansible scripts that simplify the setup of a personal WireGuard and IPsec VPN. It uses the most secure defaults available and works with common cloud providers.

[Pro Custodibus](https://www.procustodibus.com/features/) is a tool for managing WireGuard with a variety of business VPN (Virtual Private Network) use cases, such as site-to-site connectivity, secure remote access from anywhere, secure access to the cloud (Amazon Web Services, Google Cloud Platform, Microsoft Azure, etc), and more.

[Drago](https://seashell.github.io/drago) is a flexible configuration manager for WireGuard designed to make it simple to configure secure network overlays spanning heterogeneous nodes distributed across different clouds and physical locations. Drago is in active development, and we welcome contributions from the open-source community.

[Netmaker](https://netmaker.org/) is a tool that helps connect any computers together over a secure, fast, private network, and manage multiple networks from a central server.

[Kilo](https://github.com/squat/kilo) is a multi-cloud network overlay built on WireGuard and designed for Kubernetes. Kilo connects nodes in a cluster by providing an encrypted layer 3 network that can span across data centers and public clouds. The Pod network created by Kilo is always fully connected, even when the nodes are in different networks or behind NAT. By allowing pools of nodes in different locations to communicate securely, Kilo enables the operation of multi-cloud clusters. Kilo's design allows clients to VPN to a cluster in order to securely access services running on the cluster.

[Subspace](https://github.com/subspacecloud/subspace) is a simple WireGuard VPN server GUI.

[WG UI](https://github.com/EmbarkStudios/wg-ui) is a basic, self-contained management service for WireGuard with a self-serve web UI.

[WireHole](https://github.com/IAmStoxe/wirehole) is a combination of WireGuard, PiHole, and Unbound in a docker-compose project with the intent of enabling users to quickly and easily create and deploy a personally managed full or split-tunnel WireGuard VPN with ad blocking capabilities (via Pihole), and DNS caching with additional privacy options (via Unbound).

[Gluetun](https://github.com/qdm12/gluetun) is a lightwieght VPN client in a thin Docker container for multiple VPN providers, written in Go, and uses OpenVPN or Wireguard, DNS over TLS, with a few proxy servers built-in.

[Ethr](https://github.com/microsoft/ethr) is a cross platform network performance measurement tool written in golang. The goal of this project is to provide a native tool for comprehensive network performance measurements of bandwidth, connections/s, packets/s, latency, loss & jitter, across multiple protocols such as TCP, UDP, HTTP, HTTPS, and across multiple platforms such as Windows, Linux and other Unix systems.

### Setting up WireGuard with PiVPN

[Back to the Top](#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190881122-3accce96-dbc1-46ba-9e67-bff78f160475.png">
  <br />
</p>

**Installing PiVPN:**

```sudo apt install curl -y```

```curl -L https://install.pivpn.io | bash```

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880700-48034b3b-c3d2-459e-b52b-ed5d699fe31a.png">
  <br />
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880702-9da353e8-2a25-4b9c-bb48-4d28af696e1e.png">
  <br />
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880703-5d71fb3c-1ad9-4511-bb21-da60da25c9d7.png">
  <br />
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880704-2042e18b-bc60-4b53-8251-2e3628b3083e.png">
  <br />
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880705-8270b271-2cf4-49b7-b133-a04509167425.png">
  <br />
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880706-401973df-8d3d-4c18-bd79-49948b8d1ee2.png">
  <br />
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880708-9c8aedf5-81bd-4f93-bf87-d5c713194b13.png">
  <br />
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880709-28f88ff7-38bf-4ebe-916c-8228c13050ea.png">
  <br />
</p>


### Setting up WireGuard on Unraid

[Back to the Top](#table-of-contents)

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190881124-635b4c29-41c6-423d-bff9-07e811a5f319.png">
  <br />
</p>

 Select Apps, then search for WireGuard and install **Wireguard-Easy**.
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880956-9ad5d1e6-5905-46ec-9d94-6f1c0a42a997.jpg">
  <br />
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880957-d20e3fa1-b219-407a-b80b-b84cc59bb2a0.png">
  <br />
  VPN manager
</p>

 Almost all of the settings can stay as default, however, there are a few that we will modify.

   * Set the WG_HOST variable to be the IP address of your Unraid server.
   * If you’d like to modify the WireGuard port (51820), you can do that here.
   * Change the default Web GUI password. 
    
<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880958-e5c2c3f8-fd85-47c5-beb4-cc06d19899b4.png">
  <br />
</p>

    
### Setting up WireGuard on pfSense
  
  [Back to the Top](#table-of-contents)
  
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190881128-e03216b9-ecc6-4c12-a41e-0de7d1b51579.png">
  <br />
</p>
   
   When looking at how to set up WireGuard on pfSense, the first thing that we need to do is install the package. Follow the instructions below to install the WireGuard package on pfSense.
   
<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880975-b103fead-2596-4819-bb82-18414baa4fb4.jpg">
  <br />
</p>


* Open the Package Manager and search for WireGuard, then Install the latest version of the package.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880976-1c7d0b18-8e50-4072-8f32-a6991b7d3923.jpg">
  <br />
</p>

* After the package has installed, select VPN then WireGuard and under the Tunnels section, select Add Tunnel. 

* In the Tunnel Configuration, set the Description as WireGuard, the Listen Port as 51820, then Generate private and public keys.

* Copy the Public Key. We will need this for our client configuration.

* Create the tunnel, then select Settings, and ensure that Enable WireGuard is selected. Then Save and Apply. 

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880978-70ccc9f1-f5be-479a-9f95-234a4f90ee87.jpg">
  <br />
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190880979-6a1db7b4-bace-47ea-8ba5-43b375a821ba.jpg">
  <br />
</p>

### Setting up WireGuard on OpenWRT

[Back to the Top](#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190891717-a0972531-ec9d-4b7d-8543-2a68fb1792d2.png">
  <br />
</p>

**Quick Links:**

 * [WireGuard route all traffic through wireguard tunnel](https://openwrt.org/docs/guide-user/services/vpn/wireguard/all-traffic-through-wireguard)
 * [Automated WireGuard Server and Multi-client](https://openwrt.org/docs/guide-user/services/vpn/wireguard/automated)
 * [WireGuard basics](https://openwrt.org/docs/guide-user/services/vpn/wireguard/basics)
 * [WireGuard client](https://openwrt.org/docs/guide-user/services/vpn/wireguard/client)
 * [WireGuard extras](https://openwrt.org/docs/guide-user/services/vpn/wireguard/extras)
 * [WireGuard performance](https://openwrt.org/docs/guide-user/services/vpn/wireguard/performance)
 * [WireGuard Road-Warrior Configuration](https://openwrt.org/docs/guide-user/services/vpn/wireguard/road-warrior)
 * [WireGuard](https://openwrt.org/docs/guide-user/services/vpn/wireguard/start)
 * [WireGuard server](https://openwrt.org/docs/guide-user/services/vpn/wireguard/server)
 * [WireGuard peers](https://openwrt.org/docs/guide-user/services/vpn/wireguard/serverclient)
 * [Automated WireGuard site-to-site VPN configuration](https://openwrt.org/docs/guide-user/services/vpn/wireguard/site-to-site)
 

In your router’s webUI, navigate to System - Software, click Update lists:

In the Filter field, type WireGuard, locate and install the **wireguard, wireguard-tools, kmod-wireguard, and luci-app-wireguard packages.** **Note: The wireguard package is included in version 22.02.**

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190891718-b56b1152-2236-4d2c-bfbd-0f9f8f064e01.jpeg">
  <br />
</p>

**Generate WireGuard keypair**

 SSH into your router as ‘root’ ([OpenWrt Wiki](https://openwrt.org/docs/guide-quick-start/sshadministration)):

   ```ssh root@192.168.1.1```

 Generate WireGuard keys:

  ```wg genkey | tee privatekey | wg pubkey > publickey```
     
  ```chmod 600 privatekey```

  Note your Private & Public keys, you will need them later:

  ```cat privatekey```
    
  ``` cat publickey```

**Creating an Interface**

 Navigate to Network - Interface,

 Click the Add new interface... button and enter the following configuration:
   * Name - give it any name
   * Protocol - WireGuard VPN

 Create interface

 In the General Settings tab:
   * Bring up on boot - Checked
   * Private Key - copy and paste the generated previously Private key
   * IP Address - enter the WireGuard IP Address obtained in the Client Area ending with /32, e.g. 172.27.124.169/32
        
        
**Add a Firewall zone**

 Navigate to Network - Firewall

 Click the Add button and enter the following configuration:
   * Name - Give it any name
   *  Input - Reject
   *  Output - Accept
   *  Forward - Reject
   *  Masquerading - Checked
   *  MSS clamping - Checked
   *  Covered networks - select the previously created VPN tunnel interface
   *  Allow forward to destination zones - Unspecified
   *  Allow forward from source zones - lan
      
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190891722-8e64c915-9fbf-48e2-ae4d-73a1bd4c9489.jpeg">
  <br />
</p>
       
**DNS**

 Navigate to Network - Interfaces

 Click on the Edit button next to the WAN interface

  In the Advanced Settings tab, uncheck the Use DNS servers advertised by peer and specify one of the following DNS servers in the Use custom DNS servers field:
  
  * 172.16.0.1 = regular DNS with no blocking
  * 10.0.254.2 = standard AntiTracker to block advertising and malware domains
  * 10.0.254.3 = Hardcore Mode AntiTracker to also block Google and Facebook domains
      
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190891723-43aa1b88-ab91-4f87-935b-03f052add368.jpeg">
  <br />
</p> 

Click the Save button.

**Last Steps**

  * A device reboot is not required, though it may be useful to confirm that everything behaves as expected.
  * Run a leak test at [https://www.dnsleaktest.com](https://www.dnsleaktest.com/) via one of the internal network clients attached to your OpenWRT router.
  
### Setting up WireGuard on Home Assistant

[Back to the Top](#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190974554-6611b441-2487-4e82-a5f5-018e6ee887d8.png">
  <br />
</p>

**Install Wireguard Add-on in Home Assistant**

 * Next, open up Home Assistant. Go to Supervisor > Add-on store, and search for WireGuard.
 
 * Click the WireGuard addon, and the click Install.
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190974557-6e466f3a-75c5-46fe-ab95-406fad796318.png">
  <br />
</p>
 
**Configure Wireguard Settings**

After installing WireGuard, do not start it yet. We need to configure a few options first.

 * Click the Configuration tab at the very top.

 * There are **two blocks of code here: server and peers.** The server section is the WireGuard server info, and the peers section is where you’d add new devices that will connect to your VPN.
 
 **Server Configuration**

   * **Host:** add the subdomain you just created. (vpn.mydomain.com)
   * **Addresses:** If your internal network is using the 192.168.x.x or 10.x.x.x range, you can leave the default IP addresses WireGuard has provided. (see note above)
   * **DNS:** Set to your router’s internal IP address (**Open CMD > ipconfig /all > Under DNS servers**)
        If you have Adguard or PiHole installed, you can use the IP address of those instead. This will allow you to block ads even when connected to the WireGuard VPN.

**Peers Configuration**

This is where you’ll create WireGuard configuration files for each of the devices you want to connect to WireGuard with. For this example, I’m using my phone and leaving ```allowed_ips``` and ```client_allowed_ips``` as is. If you adding multiple devices, then you’ll need to copy the entire block of code starting at name, give it a different name, and add the next available IP address (For example: 172.27.66.4)

Click **Save** once finished.

Then, go back to the Info tab and click **Start**.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/190974558-dad4b4e4-295d-4074-84b8-44ca1be7078a.png">
  <br />
</p>

**Port Forward**

The next step is to forward port 51820 from your Home Assistant server through your router. Unfortunately, there are so many different types of routers, each with different steps to port forward. The important thing to note is that you’ll be **port forwarding 51820(wireguard port)** from the internal IP of your Home Assistant instance (for example: 192.168.68.24) and choosing the **UDP protocol only**.
 
 **Download Wireguard app on mobile device**

Download the WireGuard app from the [Apple App Store](https://apps.apple.com/us/app/wireguard/id1441195209) or [Google Play Store](https://play.google.com/store/apps/details?id=com.wireguard.android&hl=en_US&gl=US). You will need it for the next step.

If all goes well, you can click into the new tunnel connection from within the app. If you see data flowing under the Transfer section, that means you are good to go.

**Improving Security**

Once you have everything setup and working correctly, you should read through the [WireGuard Addon docs](https://github.com/hassio-addons/addon-wireguard/blob/main/wireguard/DOCS.md) to setup up ```allowed_ips``` and ```client_allowed_ips``` to further secure your VPN instance. There’s also some other helpful options you can configure such as log level, but these are all optional.

# Nextcloud
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/150701955-f1f514a8-82e6-462f-9fc9-8926b6b7de3e.png">
  <br />
  
</p>

[Nextcloud](https://nextcloud.com) is an industry-leading, on-premises content collaboration platform for file sync & share and communication server. It is fully open source and you can host it yourself or pay a company to do it for you. Also checkout the following links below:

   - [Nextcloud App Store](https://apps.nextcloud.com)

   - [Nextcloud GitHub](https://github.com/nextcloud)

   - [Nextcloud Developer Program](https://nextcloud.com/developer)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/150701961-ac8be115-34c1-4012-bd69-d1f22a10e48c.png">
  <br />
Nexcloud login screen
</p>

[Nextcloud Hub](https://nextcloud.com/hub/) is a tool that allows you to share and collaborate on documents, send and receive email, manage your calendar and have video chats without data leaks. As fully on-premises solution, Nextcloud Hub provides the benefits of online collaboration without the compliance and security risks.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/150701964-df1dd8d9-1d3a-4376-81e8-f49439fb4356.png">
  <br />
Nexcloud Hub
</p>

[Nextcloud AIO (All In One)](https://github.com/nextcloud/all-in-one) is a tool that provides easy deployment and maintenance with most features included in this one Nextcloud instance. 

**Features it includes:**

   * Nextcloud
   * Nextcloud Office
   * High performance backend for Nextcloud Files
   * High performance backend for Nextcloud Talk
   * Backup solution (based on BorgBackup)
   * Imaginary
   * ClamAV
   * Fulltextsearch

[Nextcloud Desktop Client](https://nextcloud.com/install/#install-clients) is a tool to synchronize files from Nextcloud Server with your computer.

[Nextcloud Deck](https://apps.nextcloud.com/apps/deck) is a kanban style organization tool aimed at personal planning and project organization for teams integrated with Nextcloud.

[Nextcloud Files](https://nextcloud.com/files/) is a tool tool that allows your employees have easy access to their files, photos and documents to work and can share and collaborate with team members, customers and partners. So IT knows nobody besides those they shared with has access to those files.

[Nextcloud Talk](https://nextcloud.com/talk/) is a tool that protects your communication better than other team collaboration platforms like Microsoft Teams or Slack, making sure your data stays on your servers. It also goes further than other encrypted communication technologies by keeping even metadata from leaking.

[Nextcloud Home](https://nextcloud.com/athome/) is a tool that allows you store your documents, calendar, contacts and photos on your server at home, at one of at one Nextcloud's providers or in a data center you trust.

[Nextcloud Enterprise](https://nextcloud.com/enterprise/) is a service that gives professional organizations software optimized and tested for mission critical environments.

[Nextcloud Outlook Integration](https://nextcloud.com/outlook/) is a tool that automatically upload files to replace large attachments or integrate Calendars and Contacts in Microsoft Outlook.

[Collabora Online in Nextcloud](https://nextcloud.com/collaboraonline/) is a powerful LibreOffice-based online office suite with collaborative editing, which supports all major document, spreadsheet and presentation file formats and works in all modern browsers.

[ONLYOFFICE integration in Nextcloud](https://nextcloud.com/onlyoffice/) is a service that empowers your users to collaborate on office documents with team members in real time. It has compatibility with Microsoft Office formats means perfect documents, every time.

[Nextcloud VM(virtual machine appliance)](https://download.nextcloudvm.com/) is a set of carefully crafted family of [*nix](https://bit.ly/2UaCC7b) scripts, which interactively guide you through a quality-controlled installation of a Nextcloud instance for Home/SME Server and scripts for Raspberry Pi 4. It is Community developed and maintained.

[LibreSign](https://libresign.github.io/) is a Libre digital signature app for Nextcloud. 

# Raspberry Pi 
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/103486513-4cecbc80-4db3-11eb-89a0-fa155cbcdbda.png">
  <br />
</p>

## Models of Raspberry Pi boards

[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

**Raspberry Pi 4 Model B**

<p align="center">
<img src="https://user-images.githubusercontent.com/45159366/103486342-08acec80-4db2-11eb-8696-f51475c9787a.jpeg">
</p>

[Check out the Raspberry Pi 4](https://www.raspberrypi.org/products/raspberry-pi-4-model-b/)

**Raspberry Pi 4 Model B Hardware Specifications**

 - Broadcom BCM2711, Quad core Cortex-A72 (ARM v8) 64-bit SoC @ 1.5GHz
 - 2GB, 4GB or 8GB LPDDR4-3200 SDRAM (depending on model)
 - 2.4 GHz and 5.0 GHz IEEE 802.11ac wireless 
 - Bluetooth 5.0, BLE
 - Gigabit Ethernet
 - 2 USB 3.0 ports; 2 USB 2.0 ports.
 - Raspberry Pi standard 40 pin GPIO header (fully backwards compatible with previous Pi boards)
 - 2 × micro-HDMI ports (up to 4kp60 supported)
 - OpenGL ES 3.0 graphics

**Raspberry Pi 400 Personal Computer Kit**

<p align="center">
<img src="https://user-images.githubusercontent.com/45159366/103486343-09458300-4db2-11eb-989a-6f0cd451c7b0.png">
</p>

[Check out the Raspberry Pi 400 Personal Computer Kit](https://www.raspberrypi.org/products/raspberry-pi-400/)

**Raspberry Pi 400 Hardware Specifications**

 - Broadcom BCM2711, Quad core Cortex-A72 (ARM v8) 64-bit SoC @ 1.8GHz
 - 4GB LPDDR4-3200 SDRAM 
 - 2.4 GHz and 5.0 GHz IEEE 802.11ac wireless 
 - Bluetooth 5.0, BLE
 - Gigabit Ethernet
 - 2 USB 3.0 ports; 2 USB 2.0 ports.
 - Raspberry Pi standard 40 pin GPIO header 
 - 2 × micro-HDMI ports (up to 4kp60 supported)
 - OpenGL ES 3.0 graphics
 
 **Raspberry Pi Pico Microcontroller**
 
<p align="center">
<img src="https://user-images.githubusercontent.com/45159366/105645203-e6593c80-5e4e-11eb-96cb-66f64a9a4367.png">
</p>

[Check out the Raspberry Pi Pico](https://www.raspberrypi.org/products/raspberry-pi-pico/)

**Raspberry Pi Pico Hardware Specifications**

 - RP2040 microcontroller chip designed by Raspberry Pi in the UK
 - Dual-core Arm Cortex-M0+ processor, flexible clock running up to 133 MHz
 - 264KB on-chip SRAM
 - 2MB on-board QSPI Flash
 - 26 multifunction GPIO pins, including 3 analogue inputs
 - 2 × UART, 2 × SPI controllers, 2 × I2C controllers, 16 × PWM channels
 - 1 × USB 1.1 controller and PHY, with host and device support
 - 8 × Programmable I/O (PIO) state machines for custom peripheral support
 - Castellated module allows soldering direct to carrier boards
 - Drag-and-drop programming using mass storage over USB
 - Low-power sleep and dormant modes
 - Accurate on-chip clock
 - Temperature sensor
 - Accelerated integer and floating-point libraries on-chip


**Raspberry Pi OS. The default Operating System for every Raspberry Pi device**

[Check out Raspberry Pi OS](https://www.raspberrypi.org/software/operating-systems/)

<img src="https://user-images.githubusercontent.com/45159366/103486345-0a76b000-4db2-11eb-9e96-e7f234bdc950.png">


## Raspberry Pi Learning Resources
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

[Raspberry Pi](https://www.raspberrypi.org/) is an ARM powered single board computer(SBC) that is the size of a credit card and costs around $35.

[Raspberry Pi Foundation](https://www.raspberrypi.org/about/) is a UK-based charity that works to put the power of computing and digital making into the hands of people all over the world.

[Microsecond accurate NTP with a Raspberry Pi and PPS GPS](https://austinsnerdythings.com/2021/04/19/microsecond-accurate-ntp-with-a-raspberry-pi-and-pps-gps/)

[Getting Started with Raspberry Pi Projects](https://projects.raspberrypi.org/)

[Online learning for the Raspberry Pi](https://www.raspberrypi.org/training/online/)

[Raspberry Pi Training Program](https://www.raspberrypi.org/training/)

[Raspberry Pi Online Courses on Udemy](https://www.udemy.com/topic/raspberry-pi/)

[Raspberry Pi Online Courses on Coursera](https://www.coursera.org/courses?languages=en&query=raspberry%20pi)

[The Raspberry Pi Platform and Python Programming course on Coursera](https://www.coursera.org/learn/raspberry-pi-platform)

[Learning Raspberry Pi with Online Courses on edX](https://www.edx.org/learn/raspberry-pi)

[Raspberry Pi Online Training Courses on LinkedIn Learning](https://www.linkedin.com/learning/topics/raspberry-pi)

[Getting Started with Raspberry Pi course on FutureLearn](https://www.futurelearn.com/courses/getting-started-with-your-raspberry-pi)

[Home Assistant on Raspberry Pi](https://www.home-assistant.io/getting-started/)

[PiSwitch: Build your own Nintendo Switch-style console](https://magpi.raspberrypi.org/articles/piswitch-nintendo-switch-console)


## Raspberry Pi Operating Systems
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

[Raspberry Pi OS](https://www.raspberrypi.org/software/operating-systems/)

[Hass.io(Home Assistant OS)](https://www.home-assistant.io/hassio/installation/)

[OmniROM(Android 11) based on ASOP](https://forum.xda-developers.com/t/omnirom-android-r-11-for-pi-4.4183121/)

[Manjaro Linux ARM](https://manjaro.org/download/#ARM)

[Arch Linux ARM](https://archlinuxarm.org/platforms/armv8/broadcom/raspberry-pi-4)

[Ubuntu MATE for Raspberry Pi](https://ubuntu-mate.org/ports/raspberry-pi/)

[Ubuntu Desktop for Raspberry Pi](https://ubuntu.com/raspberry-pi)

[Ubuntu Core on a Raspberry Pi](https://ubuntu.com/download/raspberry-pi-core)

[Ubuntu Server for ARM](https://ubuntu.com/download/server/arm)

[Fedora ARM](https://arm.fedoraproject.org)

[Kali Linux for the Raspberry Pi](https://www.kali.org/docs/arm/kali-linux-raspberry-pi/)

[Twister OS](https://twisteros.com/)

[TitusPi](https://github.com/ChrisTitusTech/TitusPi)

[RetroArch](https://www.retroarch.com/?page=platforms)

[RetroPie](https://retropie.org.uk/)

[LibreELEC](https://libreelec.tv/)

[OSMC](https://osmc.tv)

[RISC OS](https://www.riscosopen.org/content/)

[DietPi](https://github.com/MichaIng/DietPi)

[Windows 10 IoT Core](https://docs.microsoft.com/en-us/windows/iot-core/windows-iot-core)


## Raspberry Pi Tools
[Back to the Top](#table-of-contents)

[Raspberry Pi Imager](https://www.raspberrypi.org/software/) is the quick and easy way to install Raspberry Pi OS and other operating systems to a microSD card, ready to use with your Raspberry Pi.

[Raspberry Pi Locator](https://rpilocator.com/) is a website to track Raspberry Pi 4 model B, Compute Module 4, Pi Zero 2 W, and Pico availability across multiple retailers in different countries.

[Raspberry Pi Network Install (Beta)](https://www.raspberrypi.com/documentation/computers/getting-started.html#installing-over-the-network-beta) is a feature can be used to start the Raspberry Pi Imager application directly on a Raspberry Pi 4, or a Raspberry Pi 400, by downloading it from the internet using an Ethernet cable. The Raspberry Pi Imager application, which will run in memory on your Raspberry Pi, can then be used to flash the operating system onto a blank SD Card or USB disk, just like normal. 

[Raspberry Pi Bootloader](https://www.raspberrypi.com/documentation/computers/raspberry-pi.html#updating-the-bootloader) is a feature, which is now available in beta, that utilize an **EEPROM(Electrically Erasable Programmable Read-Only Memory)** to store the system’s bootloader. This EEPROM is persistent storage that is located on the Pi’s mainboard. The advantage of using the EEPROM instead is that the Raspberry Pi 4 can perform tasks without needing any storage to be attached.

[Etcher](https://www.balena.io/etcher/) is an open source, cross-platform software that makes it easy to flash operating system images to a microSD card or USB device.

[Home Assistant](https://www.home-assistant.io/) is an open source home automation that puts local control and privacy first. Home Assistant is powered by a worldwide community of tinkerers and DIY enthusiasts that runs great on Raspberry Pi. 

[Gladys Assistant](https://github.com/gladysassistant/gladys) is a  privacy-first, open-source home assistant and runs great on Raspberry Pi.

[Kodi for Raspberry Pi](https://kodi.tv/download/853) is a free and open source media player application developed by the XBMC/Kodi Foundation.

[Pi-hole](https://pi-hole.net/) is a [DNS sinkhole](https://en.wikipedia.org/wiki/DNS_Sinkhole) that protects your devices from unwanted content, without installing any client-side software, intended for use on a private network. It is designed for use on embedded devices with network capability, such as the Raspberry Pi, but it can be used on other machines running Linux and cloud implementations.

[PiKVM](https://github.com/pikvm/pikvm) is a very simple and fully functional Raspberry Pi-based KVM over IP.

[PiShrink](https://github.com/Drewsif/PiShrink) is a bash script that automatically shrink a pi image that will then resize to the max size of the SD card on boot. 

[RPiPlay](https://github.com/FD-/RPiPlay) is an open-source implementation of an AirPlay mirroring server for the Raspberry Pi that supports iOS 9 and later.

[Gpiozero](https://github.com/gpiozero/gpiozero) is a simple interface to GPIO(General-Purpose Input/Output) devices with the Raspberry Pi.

[Balena Sound](https://sound.balenalabs.io/) is a single or multi-room streamer for an existing audio device using a Raspberry Pi! It supports Bluetooth, Airplay and Spotify Connect.

[OpenBalena](https://balena.io/open) is a platform to deploy and manage connected devices.

### Home Assistant
[Back to the Top](#table-of-contents)
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177719719-9108f14f-9ca0-45e4-b1f5-55efaf1803e6.png">
  <br />
</p>

[Home Assistant](https://home-assistant.io/hassio/) is a container-based system for managing your Home Assistant Core installation and related applications. The system is controlled via Home Assistant which communicates with the Supervisor. The Supervisor provides an API to manage the installation. This includes changing network settings or installing and updating software.

**Quick Links**

 - [Getting Started with Home Assistant](https://home-assistant.io/getting-started)
 - [Home Assistant for Raspberry Pi](https://www.home-assistant.io/installation/raspberrypi/)
 - [Installing Home Assistant OS using Proxmox 7](https://github.com/Kanga-Who/home-assistant/blob/master/Home%20Assistant%20with%20Proxmox%20installation.md)

[Home Assistant Frontend](https://demo.home-assistant.io/) is a frontend for Home Assistant. 

#### Tools to write the HA image to your boot media(microSD card or USB device)

[Raspberry Pi Imager](https://www.raspberrypi.org/software/) is the quick and easy way to install Raspberry Pi OS and other operating systems to a microSD card, ready to use with your Raspberry Pi.

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177719735-575326e7-3f29-4175-8ca1-b9eabb15e2e6.png">
  <br />
</p>

[Etcher](https://www.balena.io/etcher/) is an open source, cross-platform software that makes it easy to flash operating system images to a microSD card or USB device.

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177719741-a88c162f-bfa9-469f-a87e-e9f12c175e07.png">
  <br />
</p>

### Home Assistant integrations

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177719765-602b4658-c8bf-4952-a238-4b986efbb7cb.png">
  <br />
</p>

Home Assistant integrations. Credit: [Home Assistant](https://www.home-assistant.io/integrations/)

[ESPHome](https://esphome.io/) is a system to control your ESP8266/ESP32 by simple yet powerful configuration files and control them remotely through Home Automation systems.

[Shelly Cloud](https://shelly.cloud/) is a Smart home control tool that has been perfected and provides precise monitoring of your Shelly devices no matter where you are. Shelly devices are compatible with Alexa, Google Home, Android, and iOS. 

[Plex media server](https://www.plex.tv/) is a application that gives you the power to add, access and share all the entertainment that matters to you, on almost any device. With 50,000+ on demand titles and hundreds of channels of live TV, plus your own personal media collection, using one powerful app.

[Amazon Alexa](https://alexa.amazon.com/) is a smart virtual assistant software to manage Alexa-enabled devices, control music playback, view shopping lists on the go, keep track of upcoming reminders, check on active timers and much more. 

[Google Assistant](https://assistant.google.com/) is a smart virtual assistant software on mobile and home automation devices.

[Apple HomeKit](https://www.apple.com/shop/accessories/all/homekit) is a software framework that enables your app to coordinate and control home automation accessories from multiple vendors to present a coherent, user-focused interface. Using HomeKit, your app can: Discover HomeKit-compatible automation accessories and add them to a persistent, cross-device home configuration database.

[Samsung SmartThings](https://www.smartthings.com/) is a sofwtare frmaeowrk that you can connect, monitor and control multiple smart home devices quicker and easier. Connect your Samsung smart TVs, smart appliances, smart speakers and brands like Ring, Nest and Philips Hue all from one app.

[Ecobee](https://www.ecobee.com) is a home automation company in Canada that makes thermostats for residential and commercial use.

[Lutron Caséta](https://www.lutron.com/en-US/Products/Pages/SingleRoomControls/CasetaWireless/Overview.aspx) is a smart lighting control system that is a great solution for giving any client smart lighting control. It was purposely built to work in homes of all ages and it works with older wiring as well as new.

[Philips Hue](https://www.philips-hue.com) is  a smart lighting system. The smart lights, Hue Bridge, and smart controls will forever change the way you experience light.

[Sonos](https://www.sonos.com) is the wireless home sound system that fills as many rooms as you want with great-sounding music, movies, and TV. 

[MQTT](https://mqtt.org/) is an [OASIS standard](https://www.oasis-open.org/standards/) messaging protocol for the Internet of Things (IoT). It is designed as an extremely lightweight publish/subscribe messaging transport that is ideal for connecting remote devices with a small code footprint and minimal network bandwidth.

[Zigbee](https://csa-iot.org/all-solutions/zigbee/) is the full-stack, secure, reliable, and market-proven solution used by a majority of large smart home ecosystem providers, such as Amazon's Echo Plus, Samsung SmartThings, Signify (Philips Hue), and more.

[openHAB](https://github.com/openhab) is a cross-platform software with the aim to integrate all kinds of Smart Home technologies, devices, etc. 

[Z-Wave](https://www.z-wave.com/) is the leading wireless communications protocol behind many of the secure, trusted brands that are working to make everyone's home smarter and safer.

[Zwavejs2Mqtt](https://zwave-js.github.io/zwavejs2mqtt/) is a fully configurable Zwave to MQTT Gateway and Control Panel Web UI.

[Z-Wave JS Server](https://github.com/zwave-js/zwave-js-server) is a small server wrapper around Z-Wave JS to access it via a WebSocket.

[Z-Wave JS Config DB Browser](https://devices.zwave-js.io/) is the official device configuration reference to find out if your device is supported. Currently supports 387 brands, spanning at least 2075 device configurations.

### Homebridge
[Back to the Top](#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177946864-bd962065-a863-4f97-b6be-a8f98861efa4.png">
  <br />
</p>

[Homebridge](https://homebridge.io/) is a software frameowrk that allows you to integrate with smart home devices that do not natively support [HomeKit](https://www.apple.com/shop/accessories/all/homekit). There are over 2,000 Homebridge plugins supporting thousands of different smart accessories. 

- [Official Homebridge Raspberry Pi Image](https://github.com/homebridge/homebridge-raspbian-image/wiki/Getting-Started)
- [Setup Homebridge on a Raspberry Pi (Raspbian)](https://github.com/homebridge/homebridge/wiki/Install-Homebridge-on-Raspbian)
- [Setup Homebridge on Debian or Ubuntu](https://github.com/homebridge/homebridge/wiki/Install-Homebridge-on-Debian-or-Ubuntu-Linux)
- [Setup Homebridge on Red Hat, CentOS Stream or Fedora](https://github.com/homebridge/homebridge/wiki/Install-Homebridge-on-Red-Hat%2C-CentOS-or-Fedora-Linux) 
- [Setup Homebridge on Docker (Linux)](https://github.com/homebridge/homebridge/wiki/Install-Homebridge-on-Docker)


#### Tools to write the Homebridge image to your boot media(microSD card or USB device)

[Raspberry Pi Imager](https://www.raspberrypi.org/software/) is the quick and easy way to install Raspberry Pi OS and other operating systems to a microSD card, ready to use with your Raspberry Pi.

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177719735-575326e7-3f29-4175-8ca1-b9eabb15e2e6.png">
  <br />
</p>

[Etcher](https://www.balena.io/etcher/) is an open source, cross-platform software that makes it easy to flash operating system images to a microSD card or USB device.

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177719741-a88c162f-bfa9-469f-a87e-e9f12c175e07.png">
  <br />
</p>

[Homebridge UI](https://github.com/oznu/homebridge-config-ui-x) is a tool that provides an easy to use interface to manage your Homebridge plugins, configuration and accessories.

   - Install and configure Homebridge plugins.
   - Monitor your Homebridge server via a fully customisable widget-based dashboard.
   - View and control Homebridge accessories.
   - Backup and Restore your Homebridge instance.
    
  <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177949596-0d02c572-fa6b-4fc7-adbd-d136f81149fb.png">
  <br />
  Homebridge UI
 </p> 
 
### ESPHome

[Back to the Top](#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/178136653-b6e635f6-5fa9-40a6-9903-e0dfb912ed80.png">
  <br />
</p>

[ESPHome](https://esphome.io/) is a system to control your ESP8266/ESP32 by simple yet powerful configuration files and control them remotely through Home Automation systems.

#### Quick Links

 - [ESP Web Tools](https://esphome.github.io/esp-web-tools/)

 - [Installing ESPHome Manually | ESPHome](https://esphome.io/guides/installing_esphome.html)
 
 - [Getting Started with the ESPHome Command Line](https://esphome.io/guides/getting_started_command_line.html)
 
 - [Getting Started with ESPHome and Home Assistant](https://esphome.io/guides/getting_started_hassio.html)
 
 - [ESPHome on the Raspberry Pi Pico! | Jeff Geerling](https://www.jeffgeerling.com/blog/2022/esphome-on-raspberry-pi-pico)
 
 - [How to Start on Raspberry Pi Home Automation | ESPHome](https://www.instructables.com/How-to-Start-on-Raspberry-Pi-Home-Automation-ESPHo/)

 - [ESPHome Setup | Integrating Home Assistant with Adafruit IO](https://learn.adafruit.com/integrating-adafruit-io-with-home-assistant/esphome-setup)

### Install ESPHome using Home Assistant

In [Home Assistant](https://www.home-assistant.io/integrations/esphome/) go to: 

  **Configuration > Add-ons, Backups & Supervisor > Add-on Store (button in the lower right corner) or click on the My Home Assistant Link below:**

Open your Home Assistant instance and show the Supervisor add-on store.

[![ESPHome HA](https://user-images.githubusercontent.com/45159366/178136849-9a5deed7-beb8-4a62-aeda-ce9aec3fac3e.svg)](https://my.home-assistant.io/redirect/config_flow_start?domain=esphome)

   -  Next, search for ESPHome, click on the result and then click on the Install button. 
   
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/178137323-40fb0ec9-f35c-43d7-b60c-08588c89fd33.png">
  <br />
</p>
   
   -  When the installation is finished, the Install button will be replaced with Start button – click on it to start the ESPHome add-on. 
   
<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/178137277-b71897d5-2684-451c-af2f-ab85f9b1affa.png">
  <br />
</p>

   -  Wait a few seconds for the ESPHome to start and then click on the Open Web UI button.
   
<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/178137097-7753aed9-c3e7-4fba-9b52-570771609572.png">
  <br />
</p>
   
### Install ESPHome using Docker

  - First thing is to pull the [ESPHome Docker image from Docker Hub](https://hub.docker.com/u/esphome) (Online). 

    ```docker pull esphome/esphome```

  - Then, start the ESPHome wizard. This wizard will ask you about your device type, your device name, your WiFi credentials and finally will generate a yaml file containing all of the configurations for you. 
   
   ```docker run --rm -v "${PWD}":/config -it esphome/esphome wizard stl.yaml```
  
   -  Now, connect your ESP device to the device where Docker is running (either using an USB cable or Serial-To-USB adapter) and if you are on Linux type the following command :

   ```dmesg | grep ttyUSB```
   
   - Put your device in programming mode (if needed) and execute the next command to install the ESPHome on the device connected to the /dev/ttyUSB1 using the configuration stored in stl.yaml file 
   
  ```docker run --rm -v "${PWD}":/config --device=/dev/ttyUSB1 -it esphome/esphome run stl.yaml```
   
### Install ESPHome using Python

 - If you are on macOS or Linux check if Python 3.8 or later is installed by executing the command.
  
 ```python3 --version```
  
 - If you are on macOS, you need to install wheel and esphome packages by using the following command.
  
 ```pip3 install wheel esphome```
  
 - If you are on Linux, you have to install esphome package by using the following command.
  
  ```pip3 install --user esphome```
   
 - If you are on macOS or Linux you can start the ESPHome wizard using the following command.
  
  ```esphome wizard stl-python.yaml```
   
 - Finally, connect your ESP device to your Computer (using USB cable or Serial-To-usb adapter) and put it in programming mode (if needed). Then, Install ESPHome using the configuration in the stl-python.yaml file.
  
  ```esphome run stl-python.yaml```
  
### Turning Raspberry Pi into a Router

[Back to the Top](#table-of-contents)

#### Software

[OpenWrt Project](https://openwrt.org/) is a Linux operating system targeting embedded devices. Instead of trying to create a single, static firmware, OpenWrt provides a fully writable filesystem with package management. It's primarily used on embedded devices to route network traffic.

  * [OpenWrt Wiki - Raspberry Pi setup](https://openwrt.org/toh/raspberry_pi_foundation/raspberry_pi)

**Download the appropriate OpenWrt image for your Raspberry PI by going to the link above.**

### Tools to write the Operating System (OS) image to your boot media(microSD card)

[Raspberry Pi Imager](https://www.raspberrypi.org/software/) is the quick and easy way to install Raspberry Pi OS and other operating systems to a microSD card, ready to use with your Raspberry Pi.

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/177719735-575326e7-3f29-4175-8ca1-b9eabb15e2e6.png">
  <br />
</p>

#### Hardware

[Raspberry Pi Router Board for CM4 module (Cost: $55 USD)](https://www.seeedstudio.com/CM4-Router-Board-p-5211.html) is an expansion board based on the Raspberry Pi Compute Module 4. It brings Raspberry Pi CM4 two full-speed gigabit network ports and offers better performance, lower CPU usage, and higher stability for a long time work compared with a USB network card. It's compatible with [Raspberry Pi OS](https://www.raspberrypi.com/software/operating-systems/), [Ubuntu Server](https://ubuntu.com/download/raspberry-pi) and other Raspberry Pi systems.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/183271470-728741bd-0d52-480d-8ebe-8c9817589093.png">
  <br />
  Raspberry Pi Router Board for CM4 module
</p>

**Technical Specs:**

 * Compatible Module: Raspberry Pi Compute Module 4 series.
 * BCM2711 4 core @ 1.5GHz Cortex-A72.
 * Support standard Raspberry Pi HAT interface.
 * Support POE HAT to supply power to the board.
 * Support POE HAT for external power supply.
 * Full-speed dual gigabit network interface.
 * Master-slave dual USB2.0 interface.
 * Micro SD card slot, used to support non-eMMC version of CM4.
 * Standard HDMI video output interface.
 * 0.91 inch IIC OLED display.
 * 5V DC fan interface(Support controlling via PWM signal).
 * Ethernet: high-performance Gigabit ethernet controller RTL8111E chip, JXD 2111x G2406s chip as isolation transformer.
   * Port0: Compute Module 4 Built-In.
   * Port1: PCI Express 1000BASE-T NIC.
 * GPIO: 40-Pin GPIO compatible with Raspberry Pi.

### Setting Watchdog Timer (WDT) on Raspberry Pi
[Back to the Top](#table-of-contents)

[Watchdog Timer (WDT)](https://en.wikipedia.org/wiki/Watchdog_timer) is a timer that monitors microcontroller (MCU) programs to see if they are out of control or have stopped operating.

### Installing and enabling WDT service

To enable watchdog you have to change the boot parameters by adding **dtparam=watchdog=on** in **/boot/config.txt** using a text editor such as nano, vim, gedit, etc.. Also, install watchdog package and enable it to start at startup. Also, make sure to restart your Raspberry Pi for these settings to take effect.

```pi@raspberrypi:~ $ sudo apt install watchdog```

```pi@raspberrypi:~ $sudo systemctl enable watchdog```

### Configure WDT service

Configuration file for watchdog can be found in **/etc/watchdog.conf**. 

```
max-load-1 = 24
watchdog-device = /dev/watchdog
realtime = yes
priority = 1
```

**To start the WTD service:**

```pi@raspberrypi:~ $ sudo systemctl start watchdog```

**Check watchdog status:**

```pi@raspberrypi:~ $ sudo systemctl status watchdog```

**To stop the service:**

```pi@raspberrypi:~ $ sudo systemctl stop watchdog```

## Raspberry Pi Upgrades
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

[Raspberry Pi Cases from Pi-Shop US](https://www.pishop.us/product-category/raspberry-pi/pi-cases/)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112692629-80803580-8e3c-11eb-8b5c-c4879113a058.png">
</p>


[Raspberry Pi Cases from The Pi Hut](https://thepihut.com/collections/raspberry-pi-cases)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112692621-7eb67200-8e3c-11eb-9a88-ae72443701ce.png">
</p>

[X825 expansion board](https://www.amazon.com/Geekworm-Raspberry-Storage-Expansion-Compatible/dp/B07VXF2HJG) provides a complete storage solution for newest Raspberry Pi 4 Model B, it supports up to 4TB 2.5-inch SATA hard disk drives (HDD) / solid-state drive (SSD).

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112692608-7bbb8180-8e3c-11eb-80f6-1b1d9d8656e0.png">
</p>


[Sabrent M.2 SSD [NGFF] to USB 3.0 / SATA III 2.5-Inch Aluminum Enclosure Adapter](https://www.amazon.com/Sabrent-2-5-Inch-Aluminum-Enclosure-EC-M2CU/dp/B07924J5NT/ref=sr_1_10?crid=28O2JRHO9DE4G&dchild=1&keywords=m.2+to+usb+3.0+adapter&qid=1616632834&sprefix=m.2+to+usb,aps,236&sr=8-10)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112692658-88d87080-8e3c-11eb-81f1-1c796145cf7a.png">
</p>


[Samsung 970 EVO 250GB - NVMe PCIe M.2 2280 SSD](https://www.amazon.com/dp/B07BN5FJZQ/ref=twister_B08KGF1DPF?_encoding=UTF8&psc=1)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112692666-8c6bf780-8e3c-11eb-85a6-1f160a10a01a.png">
</p>


[Western Digital 1TB WD Blue SN550 NVMe Internal SSD](https://www.amazon.com/dp/B07YFF8879/ref=twister_B082KVPKQ5?_encoding=UTF8&psc=1)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112692675-8d9d2480-8e3c-11eb-9ed1-e08c2932d5ab.png">
</p>


[SAMSUNG T5 Portable SSD](https://www.amazon.com/Samsung-500GB-Portable-Solid-State/dp/B074WZJ4MF/ref=sr_1_4?crid=343DRDX8SJJV6&dchild=1&keywords=samsung+t5+portable+ssd&qid=1616632092&sprefix=samsung+t5+portable,aps,374&sr=8-4)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112692679-8ece5180-8e3c-11eb-94e5-18796639776e.png">
</p>


[Samsung SSD 860 EVO 250GB mSATA Internal SSD](https://www.amazon.com/Samsung-250GB-mSATA-Internal-MZ-M6E250BW/dp/B07864YNTZ/ref=sr_1_8?crid=2KRBSPRQYUIOH&dchild=1&keywords=samsung+850+evo+msata&qid=1616632277&sprefix=samsung+850+evo+m,aps,233&sr=8-8)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112692689-91c94200-8e3c-11eb-82ed-28d6ab05c072.png">
</p>


[Samsung 850 EVO 120GB SSD mSATA](https://www.amazon.com/Samsung-850-120GB-mSATA-MZ-M5E120BW/dp/B00TGIVQ4G/ref=sr_1_9?crid=2KRBSPRQYUIOH&dchild=1&keywords=samsung+850+evo+msata&qid=1616632277&sprefix=samsung+850+evo+m,aps,233&sr=8-9)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/112692696-92fa6f00-8e3c-11eb-8c7a-c169bb0c9b1e.png">
</p>

# Grafana
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/124398126-eea08800-dcc8-11eb-8129-087e924d9eed.png">
  <br />
</p>

## Grafana Learning Resources

[Grafana](https://grafana.com/) is an analytics platform that enables you to query and visualize data, then create and share dashboards based on your visualizations. Easily visualize metrics, logs, and traces from multiple sources such as Prometheus, Loki, Elasticsearch, InfluxDB, Postgres, Fluentd, Fluentbit, Logstash and many more.

[Getting Started with Grafana](https://grafana.com/docs/)

[Grafana Community](https://community.grafana.com/)

[Grafana Professional Services Training | Grafana Labs](https://grafana.com/training/)

[Grafana Pro Training AWS | Grafana Labs](https://grafana.com/training/aws/)

[Grafana Tutorials](https://grafana.com/tutorials/)

[Top Grafana Courses on Udemy](https://www.udemy.com/topic/grafana/)

[Grafana Online Training Courses | LinkedIn Learning](https://www.linkedin.com/learning/topics/grafana)

[Grafana Training Courses - NobleProg](https://www.nobleprog.com/grafana-training)

[Setting Up Grafana to Visualize Our Metrics Course on Coursera](https://www.coursera.org/lecture/continuous-integration/setting-up-grafana-to-visualize-our-metrics-part-4-of-10-OOMzF)

## Grafana Tools

[Grafana Cloud ](https://grafana.com/products/cloud/) is a composable observability platform, integrating metrics, traces and logs with Grafana. Leverage the best open source observability software – including Prometheus, Loki, and Tempo – without the overhead of installing, maintaining, and scaling your observability stack.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/124398133-f3653c00-dcc8-11eb-8465-8633072daf41.png">
  <br />
</p>

**Grafana Cloud Integrations. Source: [Grafana](https://grafana.com/products/cloud/)**

[Grafana Enterprise](https://grafana.com/products/enterprise/) is a service that includes features that provide better scalability, collaboration, operations, and governance in a self-managed environment.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/124398134-f4966900-dcc8-11eb-8633-448074c93f71.png">
  <br />
</p>

**Grafana Enterprise Stack. Source: [Grafana](https://grafana.com/products/enterprise/)**

[Grafana Tempo](https://grafana.com/oss/tempo/) is an open source high-scale distributed tarcing backend. Tempo is cost-efficient, requiring only object storage to operate, and is deeply integrated with Grafana, Loki, and Prometheus.

[Grafana MetricTank](https://grafana.com/oss/metrictank/) is a multi-tenant timeseries platform for Graphite developed by Grafana Labs. MetricTank provides high-availability(HA) and efficient long-term storage, retrieval, and processing for large-scale environments.

[Grafana Tanka](https://grafana.com/oss/tanka/) is a robust configuration utility for your [Kubernetes](https://kubernetes.io/) cluster, powered by the [Jsonnet](https://jsonnet.org/) language.

[Grafana Loki](https://grafana.com/oss/loki/) is a horizontally-scalable, highly-available(HA), multi-tenant log aggregation system inspired by Prometheus.

[Cortex](https://grafana.com/oss/cortex/) is a project that lets users query metrics from many Prometheusservers in a single place, without any gaps in the grpahs due to server failture. Also, Cortex lets you store Prometheus metrics for long term capacity planning and performance analysis.

[Graphite](https://grafana.com/oss/graphite/) is an open source monitoring system.


# Networking
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/82833053-d1687b80-9e71-11ea-8c6d-074100f2f54b.png">
  <br />
</p>

## Networking Tools & Concepts

[cURL](https://curl.se/) is a computer software project providing a library and command-line tool for transferring data using various network protocols(HTTP, HTTPS, FTP, FTPS, SCP, SFTP, TFTP, DICT, TELNET, LDAP LDAPS, MQTT, POP3, POP3S, RTMP, RTMPS, RTSP, SCP, SFTP, SMB, SMBS, SMTP or SMTPS). cURL is also used in cars, television sets, routers, printers, audio equipment, mobile phones, tablets, settop boxes, media players and is the Internet transfer engine for thousands of software applications in over ten billion installations.

[cURL Fuzzer](https://github.com/curl/curl-fuzzer) is a quality assurance testing for the curl project.

[DoH](https://github.com/curl/doh) is a stand-alone application for DoH (DNS-over-HTTPS) name resolves and lookups.

[Authelia](https://www.authelia.com/) is an open-source highly-available authentication server providing single sign-on capability and two-factor authentication to applications running behind [NGINX](https://nginx.org/en/).

[nginx(engine x)](https://nginx.org/en/) is an HTTP and reverse proxy server, a mail proxy server, and a generic TCP/UDP proxy server, originally written by Igor Sysoev.

[Proxmox Virtual Environment(VE)](https://www.proxmox.com/en/) is a complete open-source platform for enterprise virtualization. It inlcudes a built-in web interface that you can easily manage VMs and containers, software-defined storage and networking, high-availability clustering, and multiple out-of-the-box tools on a single solution.

[Wireshark](https://www.wireshark.org/) is a very popular network protocol analyzer that is commonly used for network troubleshooting, analysis, and communications protocol development. Learn more about the other useful [Wireshark Tools](https://wiki.wireshark.org/Tools) available.

[HTTPie](https://github.com/httpie/httpie) is a command-line HTTP client. Its goal is to make CLI interaction with web services as human-friendly as possible. HTTPie is designed for testing, debugging, and generally interacting with APIs & HTTP servers.

[HTTPStat](https://github.com/reorx/httpstat) is a tool that visualizes curl statistics in a simple layout.

[Wuzz](https://github.com/asciimoo/wuzz) is an interactive cli tool for HTTP inspection. It can be used to inspect/modify requests copied from the browser's network inspector with the "copy as cURL" feature.

[Websocat](https://github.com/vi/websocat) is a ommand-line client for WebSockets, like netcat (or curl) for ws:// with advanced socat-like functions.

    • Connection: In networking, a connection refers to pieces of related information that are transferred through a network. This generally infers that a connection is built before the data transfer (by following the procedures laid out in a protocol) and then is deconstructed at the at the end of the data transfer.

    • Packet: A packet is, generally speaking, the most basic unit that is transferred over a network. When communicating over a network, packets are the envelopes that carry your data (in pieces) from one end point to the other.

Packets have a header portion that contains information about the packet including the source and destination, timestamps, network hops. The main portion of a packet contains the actual data being transferred. It is sometimes called the body or the payload.

    • Network Interface: A network interface can refer to any kind of software interface to networking hardware. For instance, if you have two network cards in your computer, you can control and configure each network interface associated with them individually.

A network interface may be associated with a physical device, or it may be a representation of a virtual interface. The "loop-back" device, which is a virtual interface to the local machine, is an example of this.

    • LAN: LAN stands for "local area network". It refers to a network or a portion of a network that is not publicly accessible to the greater internet. A home or office network is an example of a LAN.

    • WAN: WAN stands for "wide area network". It means a network that is much more extensive than a LAN. While WAN is the relevant term to use to describe large, dispersed networks in general, it is usually meant to mean the internet, as a whole.
If an interface is connected to the WAN, it is generally assumed that it is reachable through the internet.

    • Protocol: A protocol is a set of rules and standards that basically define a language that devices can use to communicate. There are a great number of protocols in use extensively in networking, and they are often implemented in different layers.

Some low level protocols are TCP, UDP, IP, and ICMP. Some familiar examples of application layer protocols, built on these lower protocols, are HTTP (for accessing web content), SSH, TLS/SSL, and FTP.

    • Port: A port is an address on a single machine that can be tied to a specific piece of software. It is not a physical interface or location, but it allows your server to be able to communicate using more than one application.

    • Firewall: A firewall is a program that decides whether traffic coming into a server or going out should be allowed. A firewall usually works by creating rules for which type of traffic is acceptable on which ports. Generally, firewalls block ports that are not used by a specific application on a server.

    • NAT: Network address translation is a way to translate requests that are incoming into a routing server to the relevant devices or servers that it knows about in the LAN. This is usually implemented in physical LANs as a way to route requests through one IP address to the necessary backend servers.

    • VPN: Virtual private network is a means of connecting separate LANs through the internet, while maintaining privacy. This is used as a means of connecting remote systems as if they were on a local network, often for security reasons.

## Network Layers

	While networking is often discussed in terms of topology in a horizontal way, between hosts, its implementation is layered in a vertical fashion throughout a computer or network. This means is that there are multiple technologies and protocols that are built on top of each other in order for communication to function more easily. Each successive, higher layer abstracts the raw data a little bit more, and makes it simpler to use for applications and users. It also allows you to leverage lower layers in new ways without having to invest the time and energy to develop the protocols and applications that handle those types of traffic.

	As data is sent out of one machine, it begins at the top of the stack and filters downwards. At the lowest level, actual transmission to another machine takes place. At this point, the data travels back up through the layers of the other computer. Each layer has the ability to add its own "wrapper" around the data that it receives from the adjacent layer, which will help the layers that come after decide what to do with the data when it is passed off.

	One method of talking about the different layers of network communication is the OSI model. OSI stands for Open Systems Interconnect.This model defines seven separate layers. The layers in this model are:

    • Application: The application layer is the layer that the users and user-applications most often interact with. Network communication is discussed in terms of availability of resources, partners to communicate with, and data synchronization.

    • Presentation: The presentation layer is responsible for mapping resources and creating context. It is used to translate lower level networking data into data that applications expect to see.

    • Session: The session layer is a connection handler. It creates, maintains, and destroys connections between nodes in a persistent way.

    • Transport: The transport layer is responsible for handing the layers above it a reliable connection. In this context, reliable refers to the ability to verify that a piece of data was received intact at the other end of the connection. This layer can resend information that has been dropped or corrupted and can acknowledge the receipt of data to remote computers.

    • Network: The network layer is used to route data between different nodes on the network. It uses addresses to be able to tell which computer to send information to. This layer can also break apart larger messages into smaller chunks to be reassembled on the opposite end.

    • Data Link: This layer is implemented as a method of establishing and maintaining reliable links between different nodes or devices on a network using existing physical connections.

    • Physical: The physical layer is responsible for handling the actual physical devices that are used to make a connection. This layer involves the bare software that manages physical connections as well as the hardware itself (like Ethernet).

The TCP/IP model, more commonly known as the Internet protocol suite, is another layering model that is simpler and has been widely adopted.It defines the four separate layers, some of which overlap with the OSI model:

    • Application: In this model, the application layer is responsible for creating and transmitting user data between applications. The applications can be on remote systems, and should appear to operate as if locally to the end user.
The communication takes place between peers network.

    • Transport: The transport layer is responsible for communication between processes. This level of networking utilizes ports to address different services. It can build up unreliable or reliable connections depending on the type of protocol used.

    • Internet: The internet layer is used to transport data from node to node in a network. This layer is aware of the endpoints of the connections, but does not worry about the actual connection needed to get from one place to another. IP addresses are defined in this layer as a way of reaching remote systems in an addressable manner.

    • Link: The link layer implements the actual topology of the local network that allows the internet layer to present an addressable interface. It establishes connections between neighboring nodes to send data.

### Interfaces
**Interfaces** are networking communication points for your computer. Each interface is associated with a physical or virtual networking device. Typically, your server will have one configurable network interface for each Ethernet or wireless internet card you have. In addition, it will define a virtual network interface called the "loopback" or localhost interface. This is used as an interface to connect applications and processes on a single computer to other applications and processes. You can see this referenced as the "lo" interface in many tools.

## Network Protocols

Networking works by piggybacks on a number of different protocols on top of each other. In this way, one piece of data can be transmitted using multiple protocols encapsulated within one another.

**Media Access Control(MAC)** is a communications protocol that is used to distinguish specific devices. Each device is supposed to get a unique MAC address during the manufacturing process that differentiates it from every other device on the internet. Addressing hardware by the MAC address allows you to reference a device by a unique value even when the software on top may change the name for that specific device during operation. Media access control is one of the only protocols from the link layer that you are likely to interact with on a regular basis.

**The IP protocol** is one of the fundamental protocols that allow the internet to work. IP addresses are unique on each network and they allow machines to address each other across a network. It is implemented on the internet layer in the IP/TCP model. Networks can be linked together, but traffic must be routed when crossing network boundaries. This protocol assumes an unreliable network and multiple paths to the same destination that it can dynamically change between. There are a number of different implementations of the protocol. The most common implementation today is IPv4, although IPv6 is growing in popularity as an alternative due to the scarcity of IPv4 addresses available and improvements in the protocols capabilities.

**ICMP: internet control message protocol** is used to send messages between devices to indicate the availability or error conditions. These packets are used in a variety of network diagnostic tools, such as ping and traceroute. Usually ICMP packets are transmitted when a packet of a different kind meets some kind of a problem. Basically, they are used as a feedback mechanism for network communications.

**TCP: Transmission control protocol** is implemented in the transport layer of the IP/TCP model and is used to establish reliable connections. TCP is one of the protocols that encapsulates data into packets. It then transfers these to the remote end of the connection using the methods available on the lower layers. On the other end, it can check for errors, request certain pieces to be resent, and reassemble the information into one logical piece to send to the application layer. The protocol builds up a connection prior to data transfer using a system called a three-way handshake. This is a way for the two ends of the communication to acknowledge the request and agree upon a method of ensuring data reliability. After the data has been sent, the connection is torn down using a similar four-way handshake. TCP is the protocol of choice for many of the most popular uses for the internet, including WWW, FTP, SSH, and email. It is safe to say that the internet we know today would not be here without TCP.

**UDP: User datagram protocol** is a popular companion protocol to TCP and is also implemented in the transport layer. The fundamental difference between UDP and TCP is that UDP offers unreliable data transfer. It does not verify that data has been received on the other end of the connection. This might sound like a bad thing, and for many purposes, it is. However, it is also extremely important for some functions. It’s not required to wait for confirmation that the data was received and forced to resend data, UDP is much faster than TCP. It does not establish a connection with the remote host, it simply fires off the data to that host and doesn't care if it is accepted or not. Since UDP is a simple transaction, it is useful for simple communications like querying for network resources. It also doesn't maintain a state, which makes it great for transmitting data from one machine to many real-time clients. This makes it ideal for VOIP, games, and other applications that cannot afford delays.

**HTTP: Hypertext transfer protocol** is a protocol defined in the application layer that forms the basis for communication on the web. HTTP defines a number of functions that tell the remote system what you are requesting. For instance, GET, POST, and DELETE all interact with the requested data in a different way.

**FTP: File transfer protocol** is in the application layer and provides a way of transferring complete files from one host to another. It is inherently insecure, so it is not recommended for any externally facing network unless it is implemented as a public, download-only resource.

**DNS: Domain name system** is an application layer protocol used to provide a human-friendly naming mechanism for internet resources. It is what ties a domain name to an IP address and allows you to access sites by name in your browser.

**SSH: Secure shell** is an encrypted protocol implemented in the application layer that can be used to communicate with a remote server in a secure way. Many additional technologies are built around this protocol because of its end-to-end encryption and ubiquity. There are many other protocols that we haven't covered that are equally important. However, this should give you a good overview of some of the fundamental technologies that make the internet and networking possible.

[REST(REpresentational State Transfer)](https://www.codecademy.com/articles/what-is-rest) is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other.

[JSON Web Token (JWT)](https://jwt.io) is a compact URL-safe means of representing claims to be transferred between two parties. The claims in a JWT are encoded as a JSON object that is digitally signed using JSON Web Signature (JWS).

[OAuth 2.0](https://oauth.net/2/) is an open source authorization framework that enables applications to obtain limited access to user accounts on an HTTP service, such as Amazon, Google, Facebook, Microsoft, Twitter GitHub, and DigitalOcean. It works by delegating user authentication to the service that hosts the user account, and authorizing third-party applications to access the user account.

# Docker
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/113521410-2e32c900-954e-11eb-8311-065fa0099546.png">
  <br />
</p>


<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/113521413-2ffc8c80-954e-11eb-9d19-b9c996bc524b.png">
  <br />
</p>

**Container Architecture. Source: [Containerd.io](https://containerd.io)**

## Docker Learning Resources

[Docker Training Program](https://www.docker.com/dockercon/training)

[Docker Certified Associate (DCA) certification](https://training.mirantis.com/dca-certification-exam/)

[Docker Documentation | Docker Documentation](https://docs.docker.com/)

[The Docker Workshop](https://courses.packtpub.com/courses/docker)

[Docker Courses on Udemy](https://www.udemy.com/topic/docker/)

[Docker Courses on Coursera](https://www.coursera.org/courses?query=docker)

[Docker Courses on edX](https://www.edx.org/learn/docker)

[Docker Courses on Linkedin Learning](https://www.linkedin.com/learning/topics/docker)

## Docker Tools

[Docker](https://www.docker.com/) is an open platform for developing, shipping, and running applications. Docker enables you to separate your applications from your infrastructure so you can deliver software quickly working in collaboration with cloud, Linux, and Windows vendors, including Microsoft.

[Docker Enterprise](https://www.mirantis.com/software/docker/docker-enterprise/) is a subscription including software, supported and certified container platform for CentOS, Red Hat Enterprise Linux (RHEL), Ubuntu, SUSE Linux Enterprise Server (SLES), Oracle Linux, and Windows Server 2016, as well as for cloud providers AWS and Azure. In [November 2019 Docker's Enterprise Platform business was acquired by Mirantis](https://www.mirantis.com/company/press-center/company-news/mirantis-acquires-docker-enterprise/).

[Docker Desktop](https://www.docker.com/products/docker-desktop) is an application for MacOS and Windows machines for the building and sharing of containerized applications and microservices. Docker Desktop delivers the speed, choice and security you need for designing and delivering containerized applications on your desktop. Docker Desktop includes Docker App, developer tools, Kubernetes and version synchronization to production Docker Engines.

[Docker Hub](https://hub.docker.com/) is the world's largest library and community for container images Browse over 100,000 container images from software vendors, open-source projects, and the community.

[Docker Compose](https://docs.docker.com/compose/) is a tool that was developed to help define and share multi-container applications. With Docker Compose, you can create a YAML file to define the services and with a single command, can spin everything up or tear it all down.

[Docker Swarm](https://docs.docker.com/engine/swarm/) is a Docker-native clustering system swarm is a simple tool which controls a cluster of Docker hosts and exposes it as a single "virtual" host.

[Dockerfile](https://docs.docker.com/engine/reference/builder/) is a text document that contains all the commands a user could call on the command line to assemble an image. Using docker build users can create an automated build that executes several command-line instructions in succession.

[Docker Containers](https://www.docker.com/resources/what-container) is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

[Docker Engine](https://www.docker.com/products/container-runtime) is a container runtime that runs on various Linux (CentOS, Debian, Fedora, Oracle Linux, RHEL, SUSE, and Ubuntu) and Windows Server operating systems. Docker creates simple tooling and a universal packaging approach that bundles up all application dependencies inside a container which is then run on Docker Engine.

[Docker Images](https://docs.docker.com/engine/reference/commandline/images/) is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings. Images have intermediate layers that increase reusability, decrease disk usage, and speed up docker build by allowing each step to be cached. These intermediate layers are not shown by default. The SIZE is the cumulative space taken up by the image and all its parent images.

[Docker Network](https://docs.docker.com/engine/reference/commandline/network/) is a that displays detailed information on one or more networks.

[Docker Daemon](https://docs.docker.com/config/daemon/) is a service started by a system utility, not manually by a user. This makes it easier to automatically start Docker when the machine reboots. The command to start Docker depends on your operating system. Currently, it only runs on Linux because it depends on a number of Linux kernel features, but there are a few ways to run Docker on MacOS and Windows as well by configuring the operating system utilities.

[Docker Storage](https://docs.docker.com/storage/storagedriver/select-storage-driver/) is a driver controls how images and containers are stored and managed on your Docker host.

[Kitematic](https://kitematic.com/) is a simple application for managing Docker containers on Mac, Linux and Windows letting you control your app containers from a graphical user interface (GUI).

[Open Container Initiative](https://opencontainers.org/about/overview/) is an open governance structure for the express purpose of creating open industry standards around container formats and runtimes.

[Buildah](https://buildah.io/) is a command line tool to build Open Container Initiative (OCI) images. It can be used with Docker, Podman, Kubernetes.

[Podman](https://podman.io/) is a daemonless, open source, Linux native tool designed to make it easy to find, run, build, share and deploy applications using Open Containers Initiative (OCI) Containers and Container Images. Podman provides a command line interface (CLI) familiar to anyone who has used the Docker Container Engine.

[Containerd](https://containerd.io) is a daemon that manages the complete container lifecycle of its host system, from image transfer and storage to container execution and supervision to low-level storage to network attachments and beyond. It is available for Linux and Windows.


# Kubernetes
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/95383873-a884d800-08a0-11eb-8eaf-57af5b119f56.png">
  <br />
</p>


## Kubernetes Learning Resources

[Kubernetes (K8s)](https://kubernetes.io/) is an open-source system for automating deployment, scaling, and management of containerized applications.

[Getting Kubernetes Certifications](https://training.linuxfoundation.org/certification/catalog/?_sft_technology=kubernetes)

[Getting started with Kubernetes on AWS](https://aws.amazon.com/kubernetes/)

[Kubernetes on Microsoft Azure](https://azure.microsoft.com/en-us/topic/what-is-kubernetes/)

[Intro to Azure Kubernetes Service](https://docs.microsoft.com/en-us/azure/aks/kubernetes-dashboard)

[Azure Red Hat OpenShift ](https://azure.microsoft.com/en-us/services/openshift/)

[Getting started with Google Cloud](https://cloud.google.com/learn/what-is-kubernetes)

[Getting started with Kubernetes on Red Hat](https://www.redhat.com/en/topics/containers/what-is-kubernetes)

[Getting started with Kubernetes on IBM](https://www.ibm.com/cloud/learn/kubernetes)

[Red Hat OpenShift on IBM Cloud](https://www.ibm.com/cloud/openshift)

[Enable OpenShift Virtualization on Red Hat OpenShift](https://developers.redhat.com/blog/2020/08/28/enable-openshift-virtualization-on-red-hat-openshift/)

[YAML basics in Kubernetes](https://developer.ibm.com/technologies/containers/tutorials/yaml-basics-and-usage-in-kubernetes/)

[Elastic Cloud on Kubernetes](https://www.elastic.co/elastic-cloud-kubernetes)

[Docker and Kubernetes](https://www.docker.com/products/kubernetes)

[Running Apache Spark on Kubernetes](http://spark.apache.org/docs/latest/running-on-kubernetes.html)

[Kubernetes Across VMware vRealize Automation](https://blogs.vmware.com/management/2019/06/kubernetes-across-vmware-cloud-automation-services.html)

[VMware Tanzu Kubernetes Grid](https://tanzu.vmware.com/kubernetes-grid)

[All the Ways VMware Tanzu Works with AWS](https://tanzu.vmware.com/content/blog/all-the-ways-vmware-tanzutm-works-with-aws)

[VMware Tanzu Education](https://tanzu.vmware.com/education)

[Using Ansible in a Cloud-Native Kubernetes Environment](https://www.ansible.com/blog/how-useful-is-ansible-in-a-cloud-native-kubernetes-environment)

[Managing Kubernetes (K8s) objects with Ansible](https://docs.ansible.com/ansible/latest/collections/community/kubernetes/k8s_module.html)

[Setting up a Kubernetes cluster using Vagrant and Ansible](https://kubernetes.io/blog/2019/03/15/kubernetes-setup-using-ansible-and-vagrant/)

[Running MongoDB with Kubernetes](https://www.mongodb.com/kubernetes)

[Kubernetes Fluentd](https://docs.fluentd.org/v/0.12/articles/kubernetes-fluentd)

[Understanding the new GitLab Kubernetes Agent](https://about.gitlab.com/blog/2020/09/22/introducing-the-gitlab-kubernetes-agent/)

[Intro Local Process with Kubernetes for Visual Studio 2019](https://devblogs.microsoft.com/visualstudio/introducing-local-process-with-kubernetes-for-visual-studio%E2%80%AF2019/)

[Kubernetes Contributors](https://www.kubernetes.dev/)

[KubeAcademy from VMware](https://kube.academy/)

[Kubernetes Tutorials from Pulumi](https://www.pulumi.com/docs/tutorials/kubernetes/)

[Kubernetes Playground by Katacoda](https://www.katacoda.com/courses/kubernetes/playground)

[Scalable Microservices with Kubernetes course from Udacity ](https://www.udacity.com/course/scalable-microservices-with-kubernetes--ud615)

## Kubernetes Tools, Frameworks, and Projects

[Open Container Initiative](https://opencontainers.org/about/overview/) is an open governance structure for the express purpose of creating open industry standards around container formats and runtimes.

[Buildah](https://buildah.io/) is a command line tool to build Open Container Initiative (OCI) images. It can be used with Docker, Podman, Kubernetes.

[Podman](https://podman.io/) is a daemonless, open source, Linux native tool designed to make it easy to find, run, build, share and deploy applications using Open Containers Initiative (OCI) Containers and Container Images. Podman provides a command line interface (CLI) familiar to anyone who has used the Docker Container Engine.

[Containerd](https://containerd.io) is a daemon that manages the complete container lifecycle of its host system, from image transfer and storage to container execution and supervision to low-level storage to network attachments and beyond. It is available for Linux and Windows.

[Google Kubernetes Engine (GKE)](https://cloud.google.com/kubernetes-engine/) is a managed, production-ready environment for running containerized applications.

[Azure Kubernetes Service (AKS)](https://azure.microsoft.com/en-us/services/kubernetes-service/) is serverless Kubernetes, with a integrated continuous integration and continuous delivery (CI/CD) experience, and enterprise-grade security and governance. Unite your development and operations teams on a single platform to rapidly build, deliver, and scale applications with confidence.

[Amazon EKS](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html) is a tool that runs Kubernetes control plane instances across multiple Availability Zones to ensure high availability.

[AWS Controllers for Kubernetes (ACK)](https://aws.amazon.com/blogs/containers/aws-controllers-for-kubernetes-ack/) is a new tool that lets you directly manage AWS services from Kubernetes. ACK makes it simple to build scalable and highly-available Kubernetes applications that utilize AWS services.

[Container Engine for Kubernetes (OKE)](https://www.oracle.com/cloud-native/container-engine-kubernetes/) is an Oracle-managed container orchestration service that can reduce the time and cost to build modern cloud native applications. Unlike most other vendors, Oracle Cloud Infrastructure provides Container Engine for Kubernetes as a free service that runs on higher-performance, lower-cost compute.

[Anthos](https://cloud.google.com/anthos/docs/concepts/overview) is a modern application management platform that provides a consistent development and operations experience for cloud and on-premises environments.

[Red Hat Openshift](https://www.openshift.com/) is a fully managed Kubernetes platform that provides a foundation for on-premises, hybrid, and multicloud deployments.

[OKD](https://okd.io/) is a community distribution of Kubernetes optimized for continuous application development and multi-tenant deployment. OKD adds developer and operations-centric tools on top of Kubernetes to enable rapid application development, easy deployment and scaling, and long-term lifecycle maintenance for small and large teams.

[Odo](https://odo.dev/) is a fast, iterative, and straightforward CLI tool for developers who write, build, and deploy applications on Kubernetes and OpenShift.

[Kata Operator](https://github.com/openshift/kata-operator) is an operator to perform lifecycle management (install/upgrade/uninstall) of [Kata Runtime](https://katacontainers.io/) on Openshift as well as Kubernetes cluster.

[Thanos](https://thanos.io/) is a set of components that can be composed into a highly available metric system with unlimited storage capacity, which can be added seamlessly on top of existing Prometheus deployments.

[OpenShift Hive](https://github.com/openshift/hive) is an operator which runs as a service on top of Kubernetes/OpenShift. The Hive service can be used to provision and perform initial configuration of OpenShift 4 clusters.

[Rook](https://rook.io/) is a tool that turns distributed storage systems into self-managing, self-scaling, self-healing storage services. It automates the tasks of a storage administrator: deployment, bootstrapping, configuration, provisioning, scaling, upgrading, migration, disaster recovery, monitoring, and resource management.

[VMware Tanzu](https://tanzu.vmware.com/tanzu) is a centralized management platform for consistently operating and securing your Kubernetes infrastructure and modern applications across multiple teams and private/public clouds.

[Kubespray](https://kubespray.io/) is a tool that combines Kubernetes and Ansible to easily install Kubernetes clusters that can be deployed on [AWS](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/aws.md), GCE, [Azure](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/azure.md), [OpenStack](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/openstack.md), [vSphere](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/vsphere.md), [Packet](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/packet.md) (bare metal), Oracle Cloud Infrastructure (Experimental), or Baremetal.

[KubeInit](https://github.com/kubeinit/kubeinit) provides Ansible playbooks and roles for the deployment and configuration of multiple Kubernetes distributions.

[Rancher](https://rancher.com/) is a complete software stack for teams adopting containers. It addresses the operational and security challenges of managing multiple Kubernetes clusters, while providing DevOps teams with integrated tools for running containerized workloads.

[K3s](https://github.com/rancher/k3s) is a highly available, certified Kubernetes distribution designed for production workloads in unattended, resource-constrained, remote locations or inside IoT appliances.

[Helm](https://helm.sh/) is a Kubernetes Package Manager tool that makes it easier to install and manage Kubernetes applications.

[Knative](https://knative.dev/) is a Kubernetes-based platform to build, deploy, and manage modern serverless workloads. Knative takes care of the operational overhead details of networking, autoscaling (even to zero), and revision tracking.

[KubeFlow](https://www.kubeflow.org/) is a tool dedicated to making deployments of machine learning (ML) workflows on Kubernetes simple, portable and scalable.

[Etcd](https://etcd.io/) is a distributed key-value store that provides a reliable way to store data that needs to be accessed by a distributed system or cluster of machines. Etcd is used as the backend for service discovery and stores cluster state and configuration for Kubernetes.

[OpenEBS](https://openebs.io/) is a Kubernetes-based tool to create stateful applications using Container Attached Storage.

[Container Storage Interface (CSI)](https://www.architecting.it/blog/container-storage-interface/) is an API that lets container orchestration platforms like Kubernetes seamlessly communicate with stored data via a plug-in.

[MicroK8s](https://microk8s.io/) is a tool that delivers the full Kubernetes experience. In a Fully containerized deployment with compressed over-the-air updates for ultra-reliable operations. It is supported on Linux, Windows, and MacOS.

[Charmed Kubernetes](https://ubuntu.com/kubernetes/features) is a well integrated, turn-key, conformant Kubernetes platform, optimized for your multi-cloud environments developed by Canonical.

[Grafana Kubernetes App](https://grafana.com/grafana/plugins/grafana-kubernetes-app) is a toll that allows you to monitor your Kubernetes cluster's performance. It includes 4 dashboards, Cluster, Node, Pod/Container and Deployment. It allows for the automatic deployment of the required Prometheus exporters and a default scrape config to use with your in cluster Prometheus deployment.

[KubeEdge](https://kubeedge.io/en/) is an open source system for extending native containerized application orchestration capabilities to hosts at Edge.It is built upon kubernetes and provides fundamental infrastructure support for network, app. deployment and metadata synchronization between cloud and edge.

[Lens](https://k8slens.dev/)  is the most powerful IDE for people who need to deal with Kubernetes clusters on a daily basis. It has support for MacOS, Windows and Linux operating systems.

[Flux CD](https://fluxcd.io/) is a tool that automatically ensures that the state of your Kubernetes cluster matches the configuration you've supplied in Git. It uses an operator in the cluster to trigger deployments inside Kubernetes, which means that you don't need a separate continuous delivery tool.

[Platform9 Managed Kubernetes (PMK)](https://platform9.com/managed-kubernetes/) is a Kubernetes as a service that ensures fully automated Day-2 operations with 99.9% SLA on any environment, whether in data-centers, public clouds, or at the edge.

# Ansible
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/113448802-62bd4e00-93b1-11eb-9114-419e758af23b.png">
  <br />
</p>

**[Mac Development Ansible Playbook by Jeff Geerling](https://github.com/geerlingguy/mac-dev-playbook)**

## Ansible Learning Resources

[Ansible](https://www.ansible.com/) is a simple IT automation engine that automates cloud provisioning, configuration management, application deployment, intra-service orchestration, and many other IT needs. It uses a very simple language (YAML, in the form of Ansible Playbooks) that allows you to describe your automation jobs in a way that approaches plain English. Anisble works on Linux (Red Hat EnterPrise Linux(RHEL) and Ubuntu) and Microsoft Windows.

[Red Hat Training for Ansible](https://www.ansible.com/products/training-certification)

[Top Ansible Courses Online from Udemy](https://www.udemy.com/topic/ansible/)

[Introduction to Ansible: The Fundamentals on Coursera](https://www.coursera.org/projects/ansible-fundamentals)

[Learning Ansible Fundamentals on Pluralsight](https://www.pluralsight.com/courses/ansible-fundamentals)

[Introducing Red Hat Ansible Automation Platform 2.1](https://www.ansible.com/blog/introducing-red-hat-ansible-automation-platform-2.1)

[Ansible Documentation](https://docs.ansible.com/ansible/latest/index.html)

[Ansible Galaxy User Guide](https://docs.ansible.com/ansible/latest/galaxy/user_guide.html)

[Ansible Use Cases](https://www.ansible.com/use-cases?hsLang=en-us)

[Ansible Integrations](https://www.ansible.com/integrations?hsLang=en-us)

[Ansible Collections Overview](https://github.com/ansible-collections/overview/blob/main/README.rst)

[Working with playbooks](https://docs.ansible.com/ansible/latest/user_guide/playbooks.html)

[Ansible for DevOps Examples by Jeff Geerling](https://github.com/geerlingguy/ansible-for-devops)

[Getting Started: Writing Your First Playbook - Ansible](https://www.ansible.com/blog/getting-started-writing-your-first-playbook)

[Working With Modules in Ansible](https://docs.ansible.com/ansible/latest/user_guide/modules.html)

[Ansible Best Practices: Roles & Modules](https://www.ansible.com/resources/webinars-training/ansible-best-practices-roles-modules)

[Working with command line tools for Ansible](https://docs.ansible.com/ansible/latest/user_guide/command_line_tools.html)

[Encrypting content with Ansible Vault](https://docs.ansible.com/ansible/latest/user_guide/vault.html)

[Using vault in playbooks with Ansible](https://docs.ansible.com/ansible/latest/user_guide/playbooks_vault.html)

[Using Ansible With Azure](https://docs.microsoft.com/en-us/azure/developer/ansible/overview)

[Configuring Ansible on an Azure VM](https://docs.microsoft.com/en-us/azure/developer/ansible/install-on-linux-vm)

[How to Use Ansible: An Ansible Cheat Sheet Guide from DigitalOcean](https://www.digitalocean.com/community/cheatsheets/how-to-use-ansible-cheat-sheet-guide)

[Intro to Ansible on Linode | Spatial Labs](https://spatial-labs.dev/posts/202101072328-intro-to-ansible-on-linode/)

## Ansible DevOps Tools Integration

[Ansible Automation Hub](https://www.ansible.com/products/automation-hub) is the official location to discover and download supported [collections](https://docs.ansible.com/ansible/latest/user_guide/collections_using.html#collections), included as part of an Ansible Automation Platform subscription. These content collections contain modules, plugins, roles, and playbooks in a downloadable package.

[Collections](https://docs.ansible.com/ansible/latest/user_guide/collections_using.html#collections) are a distribution format for Ansible content that can include playbooks, roles, modules, and plugins. As modules move from the core Ansible repository into collections, the module documentation will move to the [collections pages](https://docs.ansible.com/ansible/latest/collections/index.html#list-of-collections).

[Ansible Lint](https://ansible-lint.readthedocs.io/en/latest/) is a command-line tool for linting playbooks, roles and collections aimed towards any Ansible users. Its main goal is to promote proven practices, patterns and behaviors while avoiding common pitfalls that can easily lead to bugs or make code harder to maintain.

[Ansible cmdb](https://github.com/fboender/ansible-cmdb) is a tool that takes the output of Ansible’s fact gathering and converts it into a static HTML overview page containing system configuration information.

[Ansible Inventory Grapher](https://github.com/willthames/ansible-inventory-grapher) visually displays inventory inheritance hierarchies and at what level a variable is defined in inventory.

[Ansible Playbook Grapher](https://github.com/haidaraM/ansible-playbook-grapher) is a  command line tool to create a graph representing your Ansible playbook tasks and roles.

[Ansible Shell](https://github.com/dominis/ansible-shell) is an interactive shell for Ansible with built-in tab completion for all the modules.

[Ansible Silo](https://github.com/groupon/ansible-silo) is a self-contained Ansible environment by [Docker](https://www.docker.com/).

[Ansigenome](https://github.com/nickjj/ansigenome) is a command line tool designed to help you manage your Ansible roles.

[ARA](https://github.com/openstack/ara) is a records Ansible playbook runs and makes the recorded data available and intuitive for users and systems by integrating with Ansible as a callback plugin.

[Capistrano](https://capistranorb.com/documentation/overview/what-is-capistrano/) is a remote server automation tool. It supports the scripting and execution of arbitrary tasks, and includes a set of sane-default deployment workflows.

[Fabric](https://www.fabfile.org) is a high level Python (2.7, 3.4+) library designed to execute shell commands remotely over SSH, yielding useful Python objects in return. It builds on top of [Invoke](https://www.pyinvoke.org) (subprocess command execution and command-line features) and [Paramiko](https://paramiko.org/) (SSH protocol implementation), extending their APIs to complement one another and provide additional functionality.

[ansible-role-wireguard](https://galaxy.ansible.com/githubixx/ansible_role_wireguard) is an Ansible role for installing WireGuard VPN. Supports Ubuntu, Debian, Archlinx, Fedora and CentOS Stream.

[wireguard_cloud_gateway](https://galaxy.ansible.com/consensus/wireguard_cloud_gateway) is an Ansible role for setting up Wireguard as a gateway VPN server for cloud networks.

[Red Hat OpenShift](https://www.openshift.com/) is focused on security at every level of the container stack and throughout the application lifecycle. It includes long-term, enterprise support from one of the leading Kubernetes contributors and open source software companies.

[OpenShift Hive](https://github.com/openshift/hive) is an operator which runs as a service on top of Kubernetes/OpenShift. The Hive service can be used to provision and perform initial configuration of OpenShift 4 clusters.

# Databases
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/119279004-daec0700-bbdd-11eb-9662-b1fc86ec8448.png">
  <br />
</p>

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/119279002-da537080-bbdd-11eb-9d7a-44efb52f3506.png">
  <br />
</p>


## SQL/NoSQL Learning Resources

[SQL](https://en.wikipedia.org/wiki/SQL) is a standard language for storing, manipulating and retrieving data in relational databases.

[NoSQL](https://www.ibm.com/cloud/blog/sql-vs-nosql) is a database that is interchangeably referred to as "nonrelational, or "non-SQL" to highlight that the database can handle huge volumes of rapidly changing, unstructured data in different ways than a relational (SQL-based) database with rows and tables.

[Transact-SQL(T-SQL)](https://docs.microsoft.com/en-us/sql/t-sql/language-reference) is a Microsoft extension of SQL with all of the tools and applications communicating to a SQL database by sending T-SQL commands.

[Introduction to Transact-SQL](https://docs.microsoft.com/en-us/learn/modules/introduction-to-transact-sql/)

[SQL Tutorial by W3Schools](https://www.w3schools.com/sql/)

[Learn SQL Skills Online from Coursera](https://www.coursera.org/courses?query=sql)

[SQL Courses Online from Udemy](https://www.udemy.com/topic/sql/)

[SQL Online Training Courses from LinkedIn Learning](https://www.linkedin.com/learning/topics/sql)

[Learn SQL For Free from Codecademy](https://www.codecademy.com/learn/learn-sql)

[GitLab's SQL Style Guide](https://about.gitlab.com/handbook/business-ops/data-team/platform/sql-style-guide/)

[OracleDB SQL Style Guide Basics](https://oracle.readthedocs.io/en/latest/sql/basics/style-guide.html)

[Tableau CRM: BI Software and Tools](https://www.salesforce.com/products/crm-analytics/overview/)

[Databases on AWS](https://aws.amazon.com/products/databases/)

[Best Practices and Recommendations for SQL Server Clustering in AWS EC2.](https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/aws-sql-clustering.html)

[Connecting from Google Kubernetes Engine to a Cloud SQL instance.](https://cloud.google.com/sql/docs/mysql/connect-kubernetes-engine)

[Educational Microsoft Azure SQL resources](https://docs.microsoft.com/en-us/sql/sql-server/educational-sql-resources?view=sql-server-ver15)

[MySQL Certifications](https://www.mysql.com/certification/)

[SQL vs. NoSQL Databases: What's the Difference?](https://www.ibm.com/cloud/blog/sql-vs-nosql)

[What is NoSQL?](https://aws.amazon.com/nosql/)

## SQL/NoSQL Tools and Databases

[Netdata](https://github.com/netdata/netdata) is high-fidelity infrastructure monitoring and troubleshooting, real-time monitoring Agent collects thousands of metrics from systems, hardware, containers, and applications with zero configuration. It runs permanently on all your physical/virtual servers, containers, cloud deployments, and edge/IoT devices, and is perfectly safe to install on your systems mid-incident without any preparation.

[Azure Data Studio](https://github.com/Microsoft/azuredatastudio) is an open source data management tool that enables working with SQL Server, Azure SQL DB and SQL DW from Windows, macOS and Linux.

[RStudio](https://rstudio.com/) is an integrated development environment for R and Python, with a console, syntax-highlighting editor that supports direct code execution, and tools for plotting, history, debugging and workspace management.

[MySQL](https://www.mysql.com/) is a fully managed database service to deploy cloud-native applications using the world's most popular open source database.

[PostgreSQL](https://www.postgresql.org/) is a powerful, open source object-relational database system with over 30 years of active development that has earned it a strong reputation for reliability, feature robustness, and performance.

[Amazon DynamoDB](https://aws.amazon.com/dynamodb/) is a key-value and document database that delivers single-digit millisecond performance at any scale. It is a fully managed, multiregion, multimaster, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications.

[Apache Cassandra™](https://cassandra.apache.org/) is an open source NoSQL distributed database trusted by thousands of companies for scalability and high availability without compromising performance. Cassandra provides linear scalability and proven fault-tolerance on commodity hardware or cloud infrastructure make it the perfect platform for mission-critical data.

[Apache HBase™](https://hbase.apache.org/) is an open-source, NoSQL, distributed big data store. It enables random, strictly consistent, real-time access to petabytes of data. HBase is very effective for handling large, sparse datasets. HBase serves as a direct input and output to the Apache MapReduce framework for Hadoop, and works with Apache Phoenix to enable SQL-like queries over HBase tables.

[Hadoop Distributed File System (HDFS)](https://www.ibm.com/analytics/hadoop/hdfs) is a distributed file system that handles large data sets running on commodity hardware. It is used to scale a single Apache Hadoop cluster to hundreds (and even thousands) of nodes. HDFS is one of the major components of Apache Hadoop, the others being [MapReduce](https://www.ibm.com/analytics/hadoop/mapreduce) and [YARN](https://hadoop.apache.org/docs/current/hadoop-yarn/hadoop-yarn-site/YARN.html).

[Apache Mesos](http://mesos.apache.org/) is a cluster manager that provides efficient resource isolation and sharing across distributed applications, or frameworks. It can run Hadoop, Jenkins, Spark, Aurora, and other frameworks on a dynamically shared pool of nodes.

[Apache Spark](https://spark.apache.org/) is a unified analytics engine for big data processing, with built-in modules for streaming, SQL, machine learning and graph processing.

[ElasticSearch](https://www.elastic.co/) is a search engine based on the Lucene library. It provides a distributed, multitenant-capable full-text search engine with an HTTP web interface and schema-free JSON documents. Elasticsearch is developed in Java.

[Logstash](https://www.elastic.co/products/logstash) is a tool for managing events and logs. When used generically, the term encompasses a larger system of log collection, processing, storage and searching activities.

[Kibana](https://www.elastic.co/products/kibana) is an open source data visualization plugin for Elasticsearch. It provides visualization capabilities on top of the content indexed on an Elasticsearch cluster. Users can create bar, line and scatter plots, or pie charts and maps on top of large volumes of data.

[Trino](https://trino.io/) is a Distributed SQL query engine for big data. It is able to tremendously speed up [ETL processes](https://docs.microsoft.com/en-us/azure/architecture/data-guide/relational-data/etl), allow them all to use standard SQL statement, and work with numerous data sources and targets all in the same system.

[Extract, transform, and load (ETL)](https://docs.microsoft.com/en-us/azure/architecture/data-guide/relational-data/etl) is a data pipeline used to collect data from various sources, transform the data according to business rules, and load it into a destination data store.

[Redis(REmote DIctionary Server)](https://redis.io/) is an open source (BSD licensed), in-memory data structure store, used as a database, cache, and message broker. It provides data structures such as strings, hashes, lists, sets, sorted sets with range queries, bitmaps, hyperloglogs, geospatial indexes, and streams.

[FoundationDB](https://www.foundationdb.org/) is an open source distributed database designed to handle large volumes of structured data across clusters of commodity servers. It organizes data as an ordered key-value store and employs ACID transactions for all operations. It is especially well-suited for read/write workloads but also has excellent performance for write-intensive workloads. FoundationDB was acquired by [Apple in 2015](https://techcrunch.com/2015/03/24/apple-acquires-durable-database-company-foundationdb/).

[IBM DB2](https://www.ibm.com/analytics/db2) is a collection of hybrid data management products offering a complete suite of AI-empowered capabilities designed to help you manage both structured and unstructured data on premises as well as in private and public cloud environments. Db2 is built on an intelligent common SQL engine designed for scalability and flexibility.

[MongoDB](https://www.mongodb.com/) is a document database meaning it stores data in JSON-like documents.

[OracleDB](https://www.oracle.com/database/) is a powerful fully managed database helps developers manage business-critical data with the highest availability, reliability, and security.

[MariaDB](https://mariadb.com/) is an enterprise open source database solution for modern, mission-critical applications.

[SQLite](https://sqlite.org/index.html) is a C-language library that implements a small, fast, self-contained, high-reliability, full-featured, SQL database engine.SQLite is the most used database engine in the world. SQLite is built into all mobile phones and most computers and comes bundled inside countless other applications that people use every day.

[SQLite Database Browser](https://sqlitebrowser.org/) is an open source SQL tool that allows users to create, design and edits SQLite database files. It lets users show a log of all the SQL commands that have been issued by them and by the application itself.

[InfluxDB](https://www.influxdata.com/) is an open source time series platform.  This includes APIs for storing and querying data, processing it in the background for [ETL](https://docs.microsoft.com/en-us/azure/architecture/data-guide/relational-data/etl) or monitoring and alerting purposes, user dashboards, Internet of Things sensor data, and visualizing and exploring the data and more. It also has support for processing data from [Graphite](http://graphiteapp.org/).

[Atlas](https://github.com/Netflix/atlas) is an in-memory dimensional [time series database](https://en.wikipedia.org/wiki/Time_series_database).

[CouchbaseDB](https://www.couchbase.com/) is an open source distributed [multi-model NoSQL document-oriented database](https://en.wikipedia.org/wiki/Multi-model_database). It creates a key-value store with managed cache for sub-millisecond data operations, with purpose-built indexers for efficient queries and a powerful query engine for executing SQL queries.

[dbWatch](https://www.dbwatch.com/) is a complete database monitoring/management solution for SQL Server, Oracle, PostgreSQL, Sybase, MySQL and Azure. Designed for proactive management and automation of routine maintenance in large scale on-premise, hybrid/cloud database environments.

[Cosmos DB Profiler](https://hibernatingrhinos.com/products/cosmosdbprof) is a real-time visual debugger allowing a development team to gain valuable insight and perspective into their usage of Cosmos DB database. It identifies over a dozen suspicious behaviors from your application’s interaction with Cosmos DB.

[Adminer](https://www.adminer.org/) is an SQL management client tool for managing databases, tables, relations, indexes, users. Adminer has support for all the popular database management systems such as MySQL, MariaDB, PostgreSQL, SQLite, MS SQL, Oracle, Firebird, SimpleDB, Elasticsearch and MongoDB.

[DBeaver](https://dbeaver.io/) is an open source database tool for developers and database administrators. It offers supports for JDBC compliant databases such as MySQL, Oracle, IBM DB2, SQL Server, Firebird, SQLite, Sybase, Teradata, Firebird, Apache Hive, Phoenix, and Presto.

[DbVisualizer](https://dbvis.com/) is a SQL management tool that allows users to manage a wide range of databases such as Oracle, Sybase, SQL Server, MySQL, H3, and SQLite.

[AppDynamics Database](https://www.appdynamics.com/supported-technologies/database) is a management product for Microsoft SQL Server. With AppDynamics you can monitor and trend key performance metrics such as resource consumption, database objects, schema statistics and more, allowing you to proactively tune and fix issues in a High-Volume Production Environment.

[Toad](https://www.quest.com/toad/) is a SQL Server DBMS toolset developed by Quest. It increases productivity by using extensive automation, intuitive workflows, and built-in expertise. This SQL management tool resolve issues, manage change and promote the highest levels of code quality for both relational and non-relational databases.

[Lepide SQL Server](https://www.lepide.com/sql-storage-manager/) is an open source storage manager utility to analyse the performance of SQL Servers. It provides a complete overview of all configuration and permission changes being made to your SQL Server environment through an easy-to-use, graphical user interface.

[Sequel Pro](https://sequelpro.com/) is a fast MacOS database management tool for working with MySQL. This SQL management tool helpful for interacting with your database by easily to adding new databases, new tables, and new rows.

# Telco 5G
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<img src="https://user-images.githubusercontent.com/45159366/105409952-14881380-5be6-11eb-84fc-b07db69698ed.png">
 
 **VMware Cloud First Approach. Source: [VMware](https://www.vmware.com/products/telco-cloud-automation.html).**
 
 
 <img src="https://user-images.githubusercontent.com/45159366/105409956-1520aa00-5be6-11eb-8215-735c92a5470c.png">
 
 **VMware Telco Cloud Automation Components. Source: [VMware](https://www.vmware.com/products/telco-cloud-automation.html).**
 
## Telco Learning Resources

[HPE(Hewlett Packard Enterprise) Telco Blueprints overview](https://techhub.hpe.com/eginfolib/servers/docs/Telco/Blueprints/infocenter/index.html#GUID-9906A227-C1FB-4FD5-A3C3-F3B72EC81CAB.html)

[Network Functions Virtualization Infrastructure (NFVI) by Cisco](https://www.cisco.com/c/en/us/solutions/service-provider/network-functions-virtualization-nfv-infrastructure/index.html)

[Introduction to vCloud NFV Telco Edge from VMware](https://docs.vmware.com/en/VMware-vCloud-NFV-OpenStack-Edition/3.1/vloud-nfv-edge-reference-arch-31/GUID-744C45F1-A8D5-4523-9E5E-EAF6336EE3A0.html)

[VMware Telco Cloud Automation(TCA) Architecture Overview](https://docs.vmware.com/en/VMware-Telco-Cloud-Platform-5G-Edition/1.0/telco-cloud-platform-5G-edition-reference-architecture/GUID-C19566B3-F42D-4351-BA55-DE70D55FB0DD.html)

[5G Telco Cloud from VMware](https://telco.vmware.com/)

[Maturing OpenStack Together To Solve Telco Needs from Red Hat](https://www.redhat.com/cms/managed-files/4.Nokia%20CloudBand%20&%20Red%20Hat%20-%20Maturing%20Openstack%20together%20to%20solve%20Telco%20needs%20Ehud%20Malik,%20Senior%20PLM,%20Nokia%20CloudBand.pdf)

[Red Hat telco ecosystem program](https://connect.redhat.com/en/programs/telco-ecosystem)

[OpenStack for Telcos by Canonical](https://ubuntu.com/blog/openstack-for-telcos-by-canonical)

[Open source NFV platform for 5G from Ubuntu](https://ubuntu.com/telco)

[Understanding 5G Technology from Verizon](https://www.verizon.com/5g/)

[Verizon and Unity partner to enable 5G & MEC gaming and enterprise applications](https://www.verizon.com/about/news/verizon-unity-partner-5g-mec-gaming-enterprise)

[Understanding 5G Technology from Intel](https://www.intel.com/content/www/us/en/wireless-network/what-is-5g.html)

[Understanding 5G Technology from Qualcomm](https://www.qualcomm.com/invention/5g/what-is-5g)

[Telco Acceleration with Xilinx](https://www.xilinx.com/applications/wired-wireless/telco.html)

[VIMs on OSM Public Wiki](https://osm.etsi.org/wikipub/index.php/VIMs)

[Amazon EC2 Overview and Networking Introduction for Telecom Companies](https://docs.aws.amazon.com/whitepapers/latest/ec2-networking-for-telecom/ec2-networking-for-telecom.pdf)

[Citrix Certified Associate – Networking(CCA-N)](http://training.citrix.com/cms/index.php/certification/networking/)

[Citrix Certified Professional – Virtualization(CCP-V)](https://www.globalknowledge.com/us-en/training/certification-prep/brands/citrix/section/virtualization/citrix-certified-professional-virtualization-ccp-v/)

[CCNP Routing and Switching](https://learningnetwork.cisco.com/s/ccnp-enterprise)

[Certified Information Security Manager(CISM)](https://www.isaca.org/credentialing/cism)

[Wireshark Certified Network Analyst (WCNA)](https://www.wiresharktraining.com/certification.html)

[Juniper Networks Certification Program Enterprise (JNCP)](https://www.juniper.net/us/en/training/certification/)

[Cloud Native Computing Foundation Training and Certification Program](https://www.cncf.io/certification/training/)

## Tools

[Open Stack](https://www.openstack.org/) is an open source cloud platform, deployed as infrastructure-as-a-service (IaaS) to orchestrate data center operations on bare metal, private cloud hardware, public cloud resources, or both (hybrid/multi-cloud architecture). OpenStack includes advance use of virtualization & SDN for network traffic optimization to handle the core cloud-computing services of compute, networking, storage, identity, and image services.

[StarlingX](https://www.starlingx.io/) is a complete cloud infrastructure software stack for the edge used by the most demanding applications in industrial IOT, telecom, video delivery and other ultra-low latency use cases.

[Airship](https://www.airshipit.org/) is a collection of open source tools for automating cloud provisioning and management. Airship provides a declarative framework for defining and managing the life cycle of open infrastructure tools and the underlying hardware.

[Network functions virtualization (NFV)](https://www.vmware.com/topics/glossary/content/network-functions-virtualization-nfv) is the replacement of network appliance hardware with virtual machines. The virtual machines use a hypervisor to run networking software and processes such as routing and load balancing. NFV allows for the separation of communication services from dedicated hardware, such as routers and firewalls. This separation means network operations can provide new services dynamically and without installing new hardware. Deploying network components with network functions virtualization only takes hours compared to months like with traditional networking solutions. 

[Software Defined Networking (SDN)](https://www.vmware.com/topics/glossary/content/software-defined-networking) is an approach to networking that uses software-based controllers or application programming interfaces (APIs) to communicate with underlying hardware infrastructure and direct traffic on a network. This model differs from that of traditional networks, which use dedicated hardware devices (routers and switches) to control network traffic. 

[Virtualized Infrastructure Manager (VIM)](https://www.cisco.com/c/en/us/td/docs/net_mgmt/network_function_virtualization_Infrastructure/3_2_2/install_guide/Cisco_VIM_Install_Guide_3_2_2/Cisco_VIM_Install_Guide_3_2_2_chapter_00.html) is a service delivery and reduce costs with high performance lifecycle management Manage the full lifecycle of the software and hardware comprising your NFV infrastructure (NFVI), and maintaining a live inventory and allocation plan of both physical and virtual resources.

[Management and Orchestration(MANO)](https://www.etsi.org/technologies/open-source-mano) is an ETSI-hosted initiative to develop an Open Source NFV Management and Orchestration (MANO) software stack aligned with ETSI NFV. Two of the key components of the ETSI NFV architectural framework are the NFV Orchestrator and VNF Manager, known as NFV MANO.

[Magma](https://www.magmacore.org/) is an open source software platform that gives network operators an open, flexible and extendable mobile core network solution. Their mission is to connect the world to a faster network by enabling service providers to build cost-effective and extensible carrier-grade networks. Magma is 3GPP generation (2G, 3G, 4G or upcoming 5G networks) and access network agnostic (cellular or WiFi). It can flexibly support a radio access network with minimal development and deployment effort.

[OpenRAN](https://open-ran.org/) is an intelligent Radio Access Network(RAN) integrated on general purpose platforms with open interface between software defined functions. Open RANecosystem enables enormous flexibility and interoperability with a complete openess to multi-vendor deployments.

[Open vSwitch(OVS)](https://www.openvswitch.org/)is an open source production quality, multilayer virtual switch licensed under the open source Apache 2.0 license. It is designed to enable massive network automation through programmatic extension, while still supporting standard management interfaces and protocols (NetFlow, sFlow, IPFIX, RSPAN, CLI, LACP, 802.1ag).

[Edge](https://www.ibm.com/cloud/what-is-edge-computing) is a distributed computing framework that brings enterprise applications closer to data sources such as IoT devices or local edge servers. This proximity to data at its source can deliver strong business benefits, including faster insights, improved response times and better bandwidth availability.

[Multi-access edge computing (MEC)](https://www.etsi.org/technologies/multi-access-edge-computing) is an Industry Specification Group (ISG) within ETSI to create a standardized, open environment which will allow the efficient and seamless integration of applications from vendors, service providers, and third-parties across multi-vendor Multi-access Edge Computing platforms.

[Virtualized network functions(VNFs)](https://www.juniper.net/documentation/en_US/cso4.1/topics/concept/nsd-vnf-overview.html) is a software application used in a Network Functions Virtualization (NFV) implementation that has well defined interfaces, and provides one or more component networking functions in a defined way. For example, a security VNF provides Network Address Translation (NAT) and firewall component functions.
 
[Cloud-Native Network Functions(CNF)](https://www.cncf.io/announcements/2020/11/18/cloud-native-network-functions-conformance-launched-by-cncf/) is a network function designed and implemented to run inside containers. CNFs inherit all the cloud native architectural and operational principles including Kubernetes(K8s) lifecycle management, agility, resilience, and observability.
 
[Physical Network Function(PNF)](https://www.mpirical.com/glossary/pnf-physical-network-function) is a physical network node which has not undergone virtualization. Both PNFs and VNFs (Virtualized Network Functions) can be used to form an overall Network Service.

[Network functions virtualization infrastructure(NFVI)](https://docs.vmware.com/en/VMware-vCloud-NFV/2.0/vmware-vcloud-nfv-reference-architecture-20/GUID-FBEA6C6B-54D8-4A37-87B1-D825F9E0DBC7.html) is the foundation of the overall NFV architecture. It provides the physical compute, storage, and networking hardware that hosts the VNFs. Each NFVI block can be thought of as an NFVI node and many nodes can be deployed and controlled geographically.

# Open Source Security
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

[Open Source Security Foundation (OpenSSF)](https://openssf.org/) is a cross-industry collaboration that brings together leaders to improve the security of open source software by building a broader community, targeted initiatives, and best practices. The OpenSSF brings together open source security initiatives under one foundation to accelerate work through cross-industry support. Along with the Core Infrastructure Initiative and the Open Source Security Coalition, and will include new working groups that address vulnerability disclosures, security tooling and more.

## Security Standards, Frameworks and Benchmarks

[STIGs Benchmarks - Security Technical Implementation Guides](https://public.cyber.mil/stigs/)

[CIS Benchmarks - CIS Center for Internet Security](https://www.cisecurity.org/cis-benchmarks/)

[NIST - Current FIPS](https://www.nist.gov/itl/current-fips)

[ISO Standards Catalogue](https://www.iso.org/standards.html)

[Common Criteria for Information Technology Security Evaluation (CC)](https://www.commoncriteriaportal.org/cc/) is an international standard (ISO / IEC 15408) for computer security. It allows an objective evaluation to validate that a particular product satisfies a defined set of security requirements. 

[ISO 22301](https://www.iso.org/en/contents/data/standard/07/51/75106.html) is the international standard that provides a best-practice framework for implementing an optimised BCMS (business continuity management system).

[ISO27001](https://www.iso.org/isoiec-27001-information-security.html) is the international standard that describes the requirements for an ISMS (information security management system). The framework is designed to help organizations manage their security practices in one place, consistently and cost-effectively.

[ISO 27701](https://www.iso.org/en/contents/data/standard/07/16/71670.html) specifies the requirements for a PIMS (privacy information management system) based on the requirements of ISO 27001.
It is extended by a set of privacy-specific requirements, control objectives and controls. Companies that have implemented ISO 27001 will be able to use ISO 27701 to extend their security efforts to cover privacy management.

[EU GDPR (General Data Protection Regulation)](https://gdpr.eu/) is a privacy and data protection law that supersedes existing national data protection laws across the EU, bringing uniformity by introducing just one main data protection law for companies/organizations to comply with.

[CCPA (California Consumer Privacy Act)](https://www.oag.ca.gov/privacy/ccpa) is a data privacy law that took effect on January 1, 2020 in the State of California. It applies to businesses that collect California residents’ personal information, and its privacy requirements are similar to those of the EU’s GDPR (General Data Protection Regulation).

[Payment Card Industry (PCI) Data Security Standards (DSS)](https://docs.microsoft.com/en-us/microsoft-365/compliance/offering-pci-dss) is a global information security standard designed to prevent fraud through increased control of credit card data.

[SOC 2](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/aicpasoc2report.html) is an auditing procedure that ensures your service providers securely manage your data to protect the interests of your comapny/organization and the privacy of their clients. 

[NIST CSF](https://www.nist.gov/national-security-standards) is a voluntary framework primarily intended for critical infrastructure organizations to manage and mitigate cybersecurity risk based on existing best practice.

## Security Tools

[SELinux](https://github.com/SELinuxProject/selinux) is a security enhancement to Linux which allows users and administrators more control over access control. Access can be constrained on such variables as which users and applications can access which resources. These resources may take the form of files. Standard Linux access controls, such as file modes (-rwxr-xr-x) are modifiable by the user and the applications which the user runs. Conversely, SELinux access controls are determined by a policy loaded on the system which may not be changed by careless users or misbehaving applications.

[AppArmor](https://www.apparmor.net/) is an effective and easy-to-use Linux application security system. AppArmor proactively protects the operating system and applications from external or internal threats, even zero-day attacks, by enforcing good behavior and preventing both known and unknown application flaws from being exploited. AppArmor supplements the traditional Unix discretionary access control (DAC) model by providing mandatory access control (MAC). It has been included in the mainline Linux kernel since version 2.6.36 and its development has been supported by Canonical since 2009.

[Control Groups(Cgroups)](https://www.redhat.com/sysadmin/cgroups-part-one) is a Linux kernel feature that allows you to allocate resources such as CPU time, system memory, network bandwidth, or any combination of these resources for user-defined groups of tasks (processes) running on a system.

[EarlyOOM](https://github.com/rfjakob/earlyoom) is a daemon for Linux that enables users to more quickly recover and regain control over their system in low-memory situations with heavy swap usage. 

[Libgcrypt](https://www.gnupg.org/related_software/libgcrypt/) is a general purpose cryptographic library originally based on code from GnuPG.

[Kali Linux](https://www.kali.org/)  is an open source project that is maintained and funded by Offensive Security, a provider of world-class information security training and penetration testing services.

[Pi-hole](https://pi-hole.net/) is a [DNS sinkhole](https://en.wikipedia.org/wiki/DNS_Sinkhole) that protects your devices from unwanted content, without installing any client-side software, intended for use on a private network. It is designed for use on embedded devices with network capability, such as the Raspberry Pi, but it can be used on other machines running Linux and cloud implementations.

[Aircrack-ng](https://www.aircrack-ng.org/) is a network software suite consisting of a detector, packet sniffer, WEP and WPA/WPA2-PSK cracker and analysis tool for 802.11 wireless LANs. It works with any wireless network interface controller whose driver supports raw monitoring mode and can sniff 802.11a, 802.11b and 802.11g traffic.

[Burp Suite](https://portswigger.net/burp) is a leading range of cybersecurity tools.

[KernelCI](https://foundation.kernelci.org/) is a community-based open source distributed test automation system focused on upstream kernel development. The primary goal of KernelCI is to use an open testing philosophy to ensure the quality, stability and long-term maintenance of the Linux kernel.

[Continuous Kernel Integration project](https://github.com/cki-project) helps find bugs in kernel patches before they are commited to an upstram kernel tree. We are team of kernel developers, kernel testers, and automation engineers.

[eBPF](https://ebpf.io) is a revolutionary technology that can run sandboxed programs in the Linux kernel without changing kernel source code or loading kernel modules. By making the Linux kernel programmable, infrastructure software can leverage existing layers, making them more intelligent and feature-rich without continuing to add additional layers of complexity to the system.

[Cilium](https://cilium.io/) uses eBPF to accelerate getting data in and out of L7 proxies such as Envoy, enabling efficient visibility into API protocols like HTTP, gRPC, and Kafka. 

[Hubble](https://github.com/cilium/hubble) is a Network, Service & Security Observability for Kubernetes using eBPF.

[Istio](https://istio.io/) is an open platform to connect, manage, and secure microservices. Istio's control plane provides an abstraction layer over the underlying cluster management platform, such as Kubernetes and Mesos.

[Certgen](https://github.com/cilium/certgen) is a convenience tool to generate and store certificates for Hubble Relay mTLS.

[Scapy](https://scapy.net/) is a python-based interactive packet manipulation program & library.

[syzkaller](https://github.com/google/syzkaller) is an unsupervised, coverage-guided kernel fuzzer.

[SchedViz](https://github.com/google/schedviz) is a tool for gathering and visualizing kernel scheduling traces on Linux machines.

[oss-fuzz](https://google.github.io/oss-fuzz/) aims to make common open source software more secure and stable by combining modern fuzzing techniques with scalable, distributed execution.

[OSSEC](https://www.ossec.net/) is a free, open-source host-based intrusion detection system. It performs log analysis, integrity checking, Windows registry monitoring, rootkit detection, time-based alerting, and active response.

[Metasploit Project](https://www.metasploit.com/) is a computer security project that provides information about security vulnerabilities and aids in penetration testing and IDS signature development.

[Wfuzz](https://github.com/xmendez/wfuzz) was created to facilitate the task in web applications assessments and it is based on a simple concept: it replaces any reference to the FUZZ keyword by the value of a given payload.

[Nmap](https://nmap.org/) is a security scanner used to discover hosts and services on a computer network, thus building a "map" of the network. 

[Patchwork](https://github.com/getpatchwork/patchwork) is a web-based patch tracking system designed to facilitate the contribution and management of contributions to an open-source project. 

[pfSense](https://www.pfsense.org/) is a free and open source firewall and router that also features unified threat management, load balancing, multi WAN, and more.

[Snowpatch](https://github.com/ruscur/snowpatch) is a continuous integration tool for projects using a patch-based, mailing-list-centric git workflow. This workflow is used by a number of well-known open source projects such as the Linux kernel.

[Snort](https://www.snort.org/) is an open-source, free and lightweight network intrusion detection system (NIDS) software for Linux and Windows to detect emerging threats.

[Wireshark](https://www.wireshark.org/) is a free and open-source packet analyzer. It is used for network troubleshooting, analysis, software and communications protocol development, and education. 

[OpenSCAP](https://www.open-scap.org/) is U.S. standard maintained by [National Institute of Standards and Technology (NIST)](https://www.nist.gov/). It provides multiple tools to assist administrators and auditors with assessment, measurement, and enforcement of security baselines. OpenSCAP maintains great flexibility and interoperability by reducing the costs of performing security audits. Whether you want to evaluate DISA STIGs, NIST‘s USGCB, or Red Hat’s Security Response Team’s content, all are supported by OpenSCAP.

[Tink](https://github.com/google/tink) is a multi-language, cross-platform, open source library that provides cryptographic APIs that are secure, easy to use correctly, and harder to misuse. 

[OWASP](https://www.owasp.org/index.php/Main_Page) is an online community, produces freely-available articles, methodologies, documentation, tools, and technologies in the field of web application security.

[Open Vulnerability and Assessment Language](https://oval.mitre.org/) is a community effort to standardize how to assess and report upon the machine state of computer systems. OVAL includes a language to encode system details, and community repositories of content. Tools and services that use OVAL provide enterprises with accurate, consistent, and actionable information to improve their security.

[ClamAV](https://www.clamav.net/) is an open source antivirus engine for detecting trojans, viruses, malware & other malicious threats.

## Open Source Security Learning Resources

[Microsoft Open Source Software Security](https://www.microsoft.com/en-us/securityengineering/opensource)

[Cloudflare Open Source Security](https://cloudflare.github.io)

[The Seven Properties of Highly Secure Devices](https://www.microsoft.com/en-us/research/publication/seven-properties-highly-secure-devices/)

[How Layer 7 of the Internet Works](https://www.cloudflare.com/learning/ddos/what-is-layer-7/)

[The 7 Kinds of Security](https://www.veracode.com/sites/default/files/Resources/eBooks/7-kinds-of-security.pdf)

[The Libgcrypt Reference Manual](https://www.gnupg.org/documentation/manuals/gcrypt/)

[The Open Web Application Security Project(OWASP) Foundation Top 10](https://owasp.org/www-project-top-ten/)

[Best Practices for Using Open Source Code from The Linux Foundation](https://www.linuxfoundation.org/blog/2017/11/best-practices-using-open-source-code/)

[AWS Certified Security - Specialty Certification](https://aws.amazon.com/certification/certified-security-specialty/)

[Microsoft Certified: Azure Security Engineer Associate](https://docs.microsoft.com/en-us/learn/certifications/azure-security-engineer)

[Google Cloud Certified Professional Cloud Security Engineer](https://cloud.google.com/certification/cloud-security-engineer)

[Cisco Security Certifications](https://www.cisco.com/c/en/us/training-events/training-certifications/certifications/security.html)

[The Red Hat Certified Specialist in Security: Linux](https://www.redhat.com/en/services/training/ex415-red-hat-certified-specialist-security-linux-exam)

[Linux Professional Institute LPIC-3 Enterprise Security Certification](https://www.lpi.org/our-certifications/lpic-3-303-overview)

[Cybersecurity Training and Courses from IBM Skills](https://www.ibm.com/skills/topics/cybersecurity/)

[Cybersecurity Courses and Certifications by Offensive Security](https://www.offensive-security.com/courses-and-certifications/)

[RSA Certification Program](https://community.rsa.com/community/training/certification)

[Check Point Certified Security Expert(CCSE) Certification](https://training-certifications.checkpoint.com/#/courses/Check%20Point%20Certified%20Expert%20(CCSE)%20R80.x)

[Check Point Certified Security Administrator(CCSA) Certification](https://training-certifications.checkpoint.com/#/courses/Check%20Point%20Certified%20Admin%20(CCSA)%20R80.x)

[Check Point Certified Security Master (CCSM) Certification](https://training-certifications.checkpoint.com/#/courses/Check%20Point%20Certified%20Master%20(CCSM)%20R80.x)

[Certified Cloud Security Professional(CCSP) Certification](https://www.isc2.org/Certifications/CCSP)

[Certified Information Systems Security Professional (CISSP) Certification](https://www.isc2.org/Certifications/CISSP)

[CCNP Routing and Switching](https://learningnetwork.cisco.com/s/ccnp-enterprise)

[Certified Information Security Manager(CISM)](https://www.isaca.org/credentialing/cism)

[Wireshark Certified Network Analyst (WCNA)](https://www.wiresharktraining.com/certification.html)

[Juniper Networks Certification Program Enterprise (JNCP)](https://www.juniper.net/us/en/training/certification/)

[Security Training Certifications and Courses from Udemy](https://www.udemy.com/courses/search/?src=ukw&q=secuirty)

[Security Training Certifications and Courses from Coursera](https://www.coursera.org/search?query=security&)

[Security Certifications Training from Pluarlsight](https://www.pluralsight.com/browse/information-cyber-security/security-certifications)

# Differential Privacy
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
<img src="https://user-images.githubusercontent.com/45159366/103486337-ff238480-4db1-11eb-9895-f7f49cc5715a.png">
  <br />
  Above is a simple diagram of how Differential Privacy-Preserving Data Sharing and Data Mining protects a User's Data
</p>

## Differential Privacy Learning Resources

[Differential Privacy](https://www.microsoft.com/en-us/ai/ai-lab-differential-privacy) is a system that simultaneously enables researchers and analysts to extract useful insights from datasets containing personal information and offers stronger privacy protections. This is achieved by introducing "statistical noise".

[Statistical Noise](https://news.microsoft.com/on-the-issues/2020/08/27/statistical-noise-data-differential-privacy/) is a process that small aletrations to masked datasets. The statistical noise hides identifiable characteristics of individuals, ensuring that the privacy of personal information is protected, but it's small enough to not materially impact the accuracy of the answers extracted by analysts and researchers.

[Laplacian Noise](https://en.wikipedia.org/wiki/Laplace_distribution) is a mechanism that adds Laplacian-distributed noise to a function.

[Differential Privacy Blog Series by the National Institute of Standards and Technology(NIST)](https://www.nist.gov/itl/applied-cybersecurity/privacy-engineering/collaboration-space/focus-areas/de-id/dp-blog)

[Apple's Differential Privacy Overview](https://www.apple.com/privacy/docs/Differential_Privacy_Overview.pdf)

[Learning with Privacy at Scale with Apple Machine Learning](https://machinelearning.apple.com/research/learning-with-privacy-at-scale)

[Microsoft Research Differential Privacy Overview](https://www.microsoft.com/en-us/research/publication/differential-privacy/)

[Responsible Machine Learning with Microsoft Azure](https://azure.microsoft.com/en-us/services/machine-learning/responsibleml/)

[Responsible AI Resources with Microsoft AI](https://www.microsoft.com/en-us/ai/responsible-ai-resources)

[Preserve data privacy by using differential privacy and the SmartNoise package](https://docs.microsoft.com/en-us/azure/machine-learning/concept-differential-privacy)

[Open Differential Privacy(OpenDP) Initiative by Microsoft and Harvard](https://projects.iq.harvard.edu/opendp)

[Google's Differential Privacy Library](https://github.com/google/differential-privacy)

[Computing Private Statistics with Privacy on Beam from Google Codelabs](https://codelabs.developers.google.com/codelabs/privacy-on-beam/#0)

[Introducing TensorFlow Privacy: Learning with Differential Privacy for Training Data](https://blog.tensorflow.org/2020/06/introducing-new-privacy-testing-library.html)

[TensorFlow Federated: Machine Learning on Decentralized Data](https://www.tensorflow.org/federated/)

[Federated Analytics: Collaborative Data Science without Data Collection](https://ai.googleblog.com/2020/05/federated-analytics-collaborative-data.html)

[Differentially-Private Stochastic Gradient Descent(DP-SGD)](https://github.com/tensorflow/privacy/blob/master/tutorials/walkthrough/README.md)

[Learning Differential Privacy from Harvard University Privacy Tools Project](https://privacytools.seas.harvard.edu/differential-privacy)

[Harvard University Privacy Tools Project Courses & Educational Materials](https://privacytools.seas.harvard.edu/courses-educational-materials)

[The Weaknesses of Differential Privacy course on Coursera](https://www.coursera.org/lecture/data-results/weaknesses-of-differential-privacy-50Y9k)

[The Differential Privacy of Bayesian Inference](https://privacytools.seas.harvard.edu/publications/differential-privacy-bayesian-inference)

[Simultaneous private learning of multiple concepts](https://privacytools.seas.harvard.edu/publications/simultaneous-private-learning-multiple-concepts)

[The Complexity of Computing the Optimal Composition of Differential Privacy](https://privacytools.seas.harvard.edu/publications/complexity-computing-optimal-composition-differential-privacy)

[Order revealing encryption and the hardness of private learning](https://privacytools.seas.harvard.edu/publications/order-revealing-encryption-and-hardness-private-learning)

[SAP HANA data anonymization using SAP Software Solutions](https://www.sap.com/cmp/dg/crm-xt17-ddm-data-anony/index.html)

[SAP HANA Security using their In-Memory Database](https://www.sap.com/products/hana/features/security.html)

[DEFCON Differential Privacy Training Launch](https://opensource.googleblog.com/2020/08/defcon-differential-privacy-training.html)

[Secure and Private AI course on Udacity](https://www.udacity.com/course/secure-and-private-ai--ud185)

[Differential Privacy - Security and Privacy for Big Data - Part 1 course on Coursera](https://www.coursera.org/learn/security-privacy-big-data)

[Differential Privacy - Security and Privacy for Big Data - Part 2 course on Coursera](https://www.coursera.org/learn/security-privacy-big-data-protection)

[Certified Ethical Emerging Technologist Professional Certificate course on Coursera](https://www.coursera.org/professional-certificates/certified-ethical-emerging-technologist)


## Differential Privacy Tools

[PySyft](https://github.com/OpenMined/PySyft) is a Python library for secure and private Deep Learning. PySyft decouples private data from model training, using [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://www.microsoft.com/en-us/ai/ai-lab-differential-privacy), and Encrypted Computation (like [Multi-Party Computation (MPC)](https://multiparty.org) and [Homomorphic Encryption (HE)](https://www.microsoft.com/en-us/research/project/homomorphic-encryption/) within the main Deep Learning frameworks like [PyTorch](https://pytorch.org/) and [TensorFlow](https://www.tensorflow.org/).

[TensorFlow Privacy](https://github.com/tensorflow/privacy) is a  Python library that includes implementations of TensorFlow optimizers for training machine learning models with differential privacy. The library comes with tutorials and analysis tools for computing the privacy guarantees provided.

[TensorFlow Federated (TFF)](https://github.com/tensorflow/federated) is an open-source framework for machine learning and other computations on decentralized data. TFF has been developed to facilitate open research and experimentation with [Federated Learning (FL)](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), an approach to machine learning where a shared global model is trained across many participating clients that keep their training data locally. 

[Privacy on Beam](https://github.com/google/differential-privacy/tree/main/privacy-on-beam) is an end-to-end differential privacy solution built on [Apache Beam](https://beam.apache.org/documentation/). It is intended to be usable by all developers, regardless of their differential privacy expertise.

[PyDP](https://github.com/OpenMined/PyDP) is a Python wrapper for Google's Differential Privacy project.

[PennyLane](https://pennylane.ai) is a cross-platform Python library for [differentiable programming](https://en.wikipedia.org/wiki/Differentiable_programming) of quantum computers. By training a quantum computer the same way as a neural network.

[BoTorch](https://botorch.org) is a library for Bayesian Optimization built on PyTorch.

[PyTorch Geometric (PyG)](https://github.com/rusty1s/pytorch_geometric) is a geometric deep learning extension library for [PyTorch](https://pytorch.org/).

[Skorch](https://github.com/skorch-dev/skorch) is a scikit-learn compatible neural network library that wraps PyTorch.

[Diffprivlib](https://github.com/IBM/differential-privacy-library) is the IBM Differential Privacy Library for experimenting with, investigating and developing applications in, differential privacy.

[Opacus](https://opacus.ai/) is a library that enables training PyTorch models with differential privacy. It supports training with minimal code changes required on the client, has little impact on training performance and allows the client to online track the privacy budget expended at any given moment.

[Smart Noise](https://github.com/opendifferentialprivacy/smartnoise-sdk) is a toolkit that uses state-of-the-art differential privacy (DP) techniques to inject noise into data, to prevent disclosure of sensitive information and manage exposure risk.

# Machine Learning
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<img src="https://user-images.githubusercontent.com/45159366/108111395-756e0480-7049-11eb-85ca-b87315e9d3ef.jpeg">

## ML frameworks & applications

[TensorFlow](https://www.tensorflow.org) is an end-to-end open source platform for machine learning. It has a comprehensive, flexible ecosystem of tools, libraries and community resources that lets researchers push the state-of-the-art in ML and developers easily build and deploy ML powered applications.

[Tensorman](https://github.com/pop-os/tensorman) is a utility for easy management of Tensorflow containers by developed by [System76]( https://system76.com).Tensorman allows Tensorflow to operate in an isolated environment that is contained from the rest of the system. This virtual environment can operate independent of the base system, allowing you to use any version of Tensorflow on any version of a Linux distribution that supports the Docker runtime.

[Keras](https://keras.io) is a high-level neural networks API, written in Python and capable of running on top of TensorFlow, CNTK, or Theano.It was developed with a focus on enabling fast experimentation. It is capable of running on top of TensorFlow, Microsoft Cognitive Toolkit, R, Theano, or PlaidML.

[PyTorch](https://pytorch.org) is a library for deep learning on irregular input data such as graphs, point clouds, and manifolds. Primarily developed by Facebook's AI Research lab.

[Amazon SageMaker](https://aws.amazon.com/sagemaker/) is a fully managed service that provides every developer and data scientist with the ability to build, train, and deploy machine learning (ML) models quickly. SageMaker removes the heavy lifting from each step of the machine learning process to make it easier to develop high quality models.

[Azure Databricks](https://azure.microsoft.com/en-us/services/databricks/) is a fast and collaborative Apache Spark-based big data analytics service designed for data science and data engineering. Azure Databricks, sets up your Apache Spark environment in minutes, autoscale, and collaborate on shared projects in an interactive workspace. Azure Databricks supports Python, Scala, R, Java, and SQL, as well as data science frameworks and libraries including TensorFlow, PyTorch, and scikit-learn.

[Microsoft Cognitive Toolkit (CNTK)](https://docs.microsoft.com/en-us/cognitive-toolkit/) is an open-source toolkit for commercial-grade distributed deep learning. It describes neural networks as a series of computational steps via a directed graph. CNTK allows the user to easily realize and combine popular model types such as feed-forward DNNs, convolutional neural networks (CNNs) and recurrent neural networks (RNNs/LSTMs). CNTK implements stochastic gradient descent (SGD, error backpropagation) learning with automatic differentiation and parallelization across multiple GPUs and servers.

[Apache Airflow](https://airflow.apache.org) is an open-source workflow management platform created by the community to programmatically author, schedule and monitor workflows. Install. Principles. Scalable. Airflow has a modular architecture and uses a message queue to orchestrate an arbitrary number of workers. Airflow is ready to scale to infinity.

[Open Neural Network Exchange(ONNX)](https://github.com/onnx) is an open ecosystem that empowers AI developers to choose the right tools as their project evolves. ONNX provides an open source format for AI models, both deep learning and traditional ML. It defines an extensible computation graph model, as well as definitions of built-in operators and standard data types.

[Apache MXNet](https://mxnet.apache.org/) is a deep learning framework designed for both efficiency and flexibility. It allows you to mix symbolic and imperative programming to maximize efficiency and productivity. At its core, MXNet contains a dynamic dependency scheduler that automatically parallelizes both symbolic and imperative operations on the fly. A graph optimization layer on top of that makes symbolic execution fast and memory efficient. MXNet is portable and lightweight, scaling effectively to multiple GPUs and multiple machines. Support for Python, R, Julia, Scala, Go, Javascript and more.

[AutoGluon](https://autogluon.mxnet.io/index.html) is toolkit for Deep learning that automates machine learning tasks enabling you to easily achieve strong predictive performance in your applications. With just a few lines of code, you can train and deploy high-accuracy deep learning models on tabular, image, and text data.

[Anaconda](https://www.anaconda.com/) is a very popular Data Science platform for machine learning and deep learning that enables users to develop models, train them, and deploy them.

[PlaidML](https://github.com/plaidml/plaidml) is an advanced and portable tensor compiler for enabling deep learning on laptops, embedded devices, or other devices where the available computing hardware is not well supported or the available software stack contains unpalatable license restrictions.

[OpenCV](https://opencv.org) is a highly optimized library with focus on real-time computer vision applications. The C++, Python, and Java interfaces support Linux, MacOS, Windows, iOS, and Android.

[Scikit-Learn](https://scikit-learn.org/stable/index.html) is a Python module for machine learning built on top of SciPy, NumPy, and matplotlib, making it easier to apply robust and simple implementations of many popular machine learning algorithms.

[Weka](https://www.cs.waikato.ac.nz/ml/weka/) is an open source machine learning software that can be accessed through a graphical user interface, standard terminal applications, or a Java API. It is widely used for teaching, research, and industrial applications, contains a plethora of built-in tools for standard machine learning tasks, and additionally gives transparent access to well-known toolboxes such as scikit-learn, R, and Deeplearning4j. 

[Caffe](https://github.com/BVLC/caffe) is a deep learning framework made with expression, speed, and modularity in mind. It is developed by Berkeley AI Research (BAIR)/The Berkeley Vision and Learning Center (BVLC) and community contributors.

[Theano](https://github.com/Theano/Theano) is a Python library that allows you to define, optimize, and evaluate mathematical expressions involving multi-dimensional arrays efficiently including tight integration with NumPy.

[nGraph](https://github.com/NervanaSystems/ngraph) is an open source C++ library, compiler and runtime for Deep Learning. The nGraph Compiler aims to accelerate developing AI workloads using any deep learning framework and deploying to a variety of hardware targets.It provides the freedom, performance, and ease-of-use to AI developers.

[NVIDIA cuDNN](https://developer.nvidia.com/cudnn) is a GPU-accelerated library of primitives for [deep neural networks](https://developer.nvidia.com/deep-learning). cuDNN provides highly tuned implementations for standard routines such as forward and backward convolution, pooling, normalization, and activation layers. cuDNN accelerates widely used deep learning frameworks, including [Caffe2](https://caffe2.ai/), [Chainer](https://chainer.org/), [Keras](https://keras.io/), [MATLAB](https://www.mathworks.com/solutions/deep-learning.html), [MxNet](https://mxnet.incubator.apache.org/), [PyTorch](https://pytorch.org/), and [TensorFlow](https://www.tensorflow.org/).

[Jupyter Notebook](https://jupyter.org/) is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text. Jupyter is used widely in industries that do data cleaning and transformation, numerical simulation, statistical modeling, data visualization, data science, and machine learning.

[Apache Spark](https://spark.apache.org/) is a unified analytics engine for large-scale data processing. It provides high-level APIs in Scala, Java, Python, and R, and an optimized engine that supports general computation graphs for data analysis. It also supports a rich set of higher-level tools including Spark SQL for SQL and DataFrames, MLlib for machine learning, GraphX for graph processing, and Structured Streaming for stream processing.

[Apache Spark Connector for SQL Server and Azure SQL](https://github.com/microsoft/sql-spark-connector) is a high-performance connector that enables you to use transactional data in big data analytics and persists results for ad-hoc queries or reporting. The connector allows you to use any SQL database, on-premises or in the cloud, as an input data source or output data sink for Spark jobs.

[Apache PredictionIO](https://predictionio.apache.org/) is an open source machine learning framework for developers, data scientists, and end users. It supports event collection, deployment of algorithms, evaluation, querying predictive results via REST APIs. It is based on scalable open source services like Hadoop, HBase (and other DBs), Elasticsearch, Spark and implements what is called a Lambda Architecture.

[Cluster Manager for Apache Kafka(CMAK)](https://github.com/yahoo/CMAK) is a tool for managing [Apache Kafka](https://kafka.apache.org/) clusters.

[BigDL](https://bigdl-project.github.io/) is a distributed deep learning library for Apache Spark. With BigDL, users can write their deep learning applications as standard Spark programs, which can directly run on top of existing Spark or Hadoop clusters.

[Koalas](https://pypi.org/project/koalas/) is project makes data scientists more productive when interacting with big data, by implementing the pandas DataFrame API on top of Apache Spark.

[Apache Spark™ MLflow](https://mlflow.org/) is an open source platform to manage the ML lifecycle, including experimentation, reproducibility, deployment, and a central model registry. MLflow currently offers four components:

**[MLflow Tracking](https://mlflow.org/docs/latest/tracking.html)**: Record and query experiments: code, data, config, and results.

**[MLflow Projects](https://mlflow.org/docs/latest/projects.html)**: Package data science code in a format to reproduce runs on any platform.

**[MLflow Models](https://mlflow.org/docs/latest/models.html)**: Deploy machine learning models in diverse serving environments.

**[Model Registry](https://mlflow.org/docs/latest/model-registry.html)**: Store, annotate, discover, and manage models in a central repository.

[Eclipse Deeplearning4J (DL4J)](https://deeplearning4j.konduit.ai/) is a set of projects intended to support all the needs of a JVM-based(Scala, Kotlin, Clojure, and Groovy) deep learning application. This means starting with the raw data, loading and preprocessing it from wherever and whatever format it is in to building and tuning a wide variety of simple and complex deep learning networks.

[Numba](https://github.com/numba/numba) is an open source, NumPy-aware optimizing compiler for Python sponsored by Anaconda, Inc. It uses the LLVM compiler project to generate machine code from Python syntax. Numba can compile a large subset of numerically-focused Python, including many NumPy functions. Additionally, Numba has support for automatic parallelization of loops, generation of GPU-accelerated code, and creation of ufuncs and C callbacks.

[Chainer](https://chainer.org/) is a Python-based deep learning framework aiming at flexibility. It provides automatic differentiation APIs based on the define-by-run approach (dynamic computational graphs) as well as object-oriented high-level APIs to build and train neural networks. It also supports CUDA/cuDNN using [CuPy](https://github.com/cupy/cupy) for high performance training and inference.

[cuML](https://github.com/rapidsai/cuml) is a suite of libraries that implement machine learning algorithms and mathematical primitives functions that share compatible APIs with other RAPIDS projects. cuML enables data scientists, researchers, and software engineers to run traditional tabular ML tasks on GPUs without going into the details of CUDA programming. In most cases, cuML's Python API matches the API from scikit-learn.

## Online ML Learning Resources

[Machine Learning by Stanford University from Coursera](https://www.coursera.org/learn/machine-learning)

[Machine Learning Courses Online from Coursera](https://www.coursera.org/courses?query=machine%20learning&)

[Machine Learning Courses Online from Udemy](https://www.udemy.com/topic/machine-learning/)

[Learn Machine Learning with Online Courses and Classes from edX](https://www.edx.org/learn/machine-learning)


# IoT Protocols
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

[DBus](https://www.freedesktop.org/wiki/Software/dbus/) is an open source software bus developed Red Hat for inter-process communication, and remote procedure call mechanism that allows communication between multiple processes running concurrently on the same machine.

[SOAP](https://www.soapui.org) is a messaging protocol specification for exchanging structured information in the implementation of web services in computer networks. SOAP can extend HTTP for XML messaging. SOAP provides data transport for Web services. SOAP can exchange complete documents or call a remote procedure. SOAP can be used for broadcasting a message.

[gRPC](https://grpc.io) is a modern, open source remote procedure call (RPC) framework developed by Google that can run anywhere. It enables client and server applications to communicate transparently, and makes it easier to build connected systems.It uses HTTP/2 for transport, Protocol Buffers as the interface description language, and provides features such as authentication, bidirectional streaming and flow control, blocking or nonblocking bindings, and cancellation and timeouts.

[LWM2M](https://www.omaspecworks.org/what-is-oma-specworks/iot/lightweight-m2m-lwm2m/) is a protocol from the Open Mobile Alliance for M2M or IoT device management. Lightweight M2M enabler defines the application layer communication protocol between a LWM2M Server and a LWM2M Client, which is located in a LWM2M Device.

 [Advanced Message Queuing Protocol (AMQP)](https://www.amqp.org) is an open standard for passing business messages between applications or organizations. It connects systems, feeds business processes with the information they need and reliably transmits onward the instructions that achieve their goals. The defining features of AMQP are message orientation, queuing, routing, reliability and security.

 [Constrained Application Protocol (CoAP)](https://coap.technology) is a specialized web transfer protocol for use with constrained nodes and constrained networks in the Internet of Things. The protocol is designed for machine-to-machine (M2M) applications such as smart energy and building automation."

 [Extensible Messaging and Presence Protocol (XMPP)](https://xmpp.org) is a communication protocol for message-oriented middleware based on XML (Extensible Markup Language). It enables the near real-time exchange of structured yet extensible data between any two or more network entities.

 [OASIS Message Queuing Telemetry Transport (MQTT)](https://www.oasis-open.org) is an open OASIS and ISO standard (ISO/IEC 20922) lightweight, publish-subscribe network protocol that transports messages between devices. The protocol usually runs over TCP/IP; however, any network protocol that provides ordered, lossless, bi-directional connections can support MQTT. 

 [Very Simple Control Protocol (VSCP)](https://vscp.org) is a free automation protocol suitable for all sorts of automation task where building- or home-automation is in the main focus. Its main advantage is that each VSCP-node can work completely autonomous, being part of distributed network of other nodes.

# Operating systems
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)


[Raspberry Pi OS](https://www.raspberrypi.org/software/operating-systems/)

[Hass.io(Home Assistant OS)](https://www.home-assistant.io/hassio/installation/)

[Manjaro Linux ARM](https://manjaro.org/download/#ARM)

[Arch Linux ARM](https://archlinuxarm.org/platforms/armv8/broadcom/raspberry-pi-4)

[Ubuntu MATE for Raspberry Pi](https://ubuntu-mate.org/ports/raspberry-pi/)

[Ubuntu Desktop for Raspberry Pi](https://ubuntu.com/raspberry-pi)

[Ubuntu Core on a Raspberry Pi](https://ubuntu.com/download/raspberry-pi-core)

[Ubuntu Server for ARM](https://ubuntu.com/download/server/arm)

[Debian](https://wiki.debian.org)

[Fedora ARM](https://arm.fedoraproject.org)

[openSUSE](https://en.opensuse.org/openSUSE)

[SUSE](https://documentation.suse.com/)

[Kali Linux for the Raspberry Pi](https://www.kali.org/docs/arm/kali-linux-raspberry-pi/)

[RetroArch](https://www.retroarch.com/?page=platforms)

[RetroPie](https://retropie.org.uk/)

[LibreELEC](https://libreelec.tv/)

[OSMC](https://osmc.tv)

[RISC OS](https://www.riscosopen.org/content/)

[Windows 10 IoT Core](https://docs.microsoft.com/en-us/windows/iot-core/windows-iot-core)

[HeliOS](https://www.arduino.cc/reference/en/libraries/helios/) is an embedded operating system that is free for anyone to use. While called an operating system for simplicity, HeliOS is better described as a multitasking kernel for embedded systems.

[Simba](https://simba-os.readthedocs.io/en/latest/getting-started.html) is a small OS for an Embedded Programming Platform like Arduino. It aims to make embedded programming easy and portable.

[Trampoline](https://github.com/TrampolineRTOS/) is a static RTOS for small embedded systems.

[DuinOS](https://github.com/DuinOS/DuinOS) is Framework (a wrapper) for use the FreeRTOSwith Arduino.

[VxWorks](https://www.windriver.com/products/vxworks) is an industry-leading real-time operating systems (RTOS) for building embedded devices and systems for more than 30 years.

[LynxOS](https://www.lynx.com/products/lynxos-posix-real-time-operating-system-rtos) is a native POSIX, hard real-time partitioning operating system developed by Lynx Software Technologies.

[Zephyr OS](https://www.zephyrproject.org/zephyr-rtos-featured-in-risc-v-getting-started-guide/) is a popular security-oriented RTOS with a small-footprint kernel designed for use on resource-constrained and embedded systems. Zephyr has a small-foorprint Kernel focusing on embedded devices compatible with x86, ARM, RISC-V, Xtensa and [others](https://docs.zephyrproject.org/latest/boards/index.html).

[FreeRTOS](https://freertos.org/) is an open source, real-time operating system for microcontrollers that makes small, low-power edge devices easy to program, deploy, secure, connect, and manage.

[Arm Mbed TLS](https://os.mbed.com) provides a comprehensive SSL/TLS solution and makes it easy for developers to include cryptographic and SSL/TLS capabilities in their software and embedded products. As an SSL library, it provides an intuitive API, readable source code and a minimal and highly configurable code footprint.

[Contiki-os](https://github.com/contiki-os) is an operating system for networked, memory-constrained systems with a focus on low-power wireless Internet of Things devices.


# Middleware
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

 [IoTSyS](https://iotsyst.com) is an integration middleware for the Internet of Things. It provides a communication stack for embedded devices based on IPv6, Web services, and OBIX to establish interoperable interfaces for smart objects.

 [OpenIoT](https://github.com/OpenIotOrg/openiot) is an open source middleware infrastructure will support flexible configuration and deployment of algorithms for collection, and filtering information streams stemming from the internet-connected objects, while at the same time generating and processing important business/applications events.

 [OpenRemote](https://github.com/openremote/openremote) is an open source middleware project, which integrates many different protocols and solutions available for smart building, and smart city automation, and offers visualization tools. 

 [Kaa](https://www.kaaproject.org/platform/) is a Enterprise IoT Platform has been designed with heavy-duty, enterprise-grade IoT solutions in mind. It banishes a monolithic approach to architecture in favour of highly portable microservices, which allow for flexible rearrangement and customization even in the middle of the solution's lifecycle.

# Node flow editors
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

 [Node-RED](https://nodered.org) is a programming tool for wiring together hardware devices, APIs and online services in new and interesting ways. It provides a browser-based editor that makes it easy to wire together flows using the wide range of nodes in the palette that can be deployed to its runtime in a single-click.

### Toolkits
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

 [KinomaJS](https://github.com/Kinoma/kinomajs) is a visual code editor designed to help developers build starter projects for Kinoma Create and Kinoma Element. The project is built on Angular 2(RC7) and runs in a web browser. The live version is hosted using Google App Engine, but you can modify and build it yourself by following the instructions in this document.

 [IoT Toolkit](https://www.segger.com/products/security-iot/iot-toolkit/) is a collection of libraries that enables communication with modern IoT based environments and devices. It is a high-performance collection of libraries optimized for minimum memory consumption in RAM, ROM, high speed, and versatility working on any device.

# Data Visualization
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

[Freeboard](https://github.com/Freeboard/freeboard) is an open source real-time dashboard builder for IOT and other web mashups. A free open-source alternative to Geckoboard.

[ThingSpeak](https://thingspeak.com) is an IoT analytics platform service that allows you to aggregate, visualize, and analyze live data streams in the cloud. You can send data to ThingSpeak from your devices, create instant visualization of live data, and send alerts.

# Search
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

 [Thingful](https://www.thingful.net) is a Search Engine for the Internet of Things Find & use open IoT data from around the world.

# Hardware
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

 [Arduino Ethernet Shield 2](https://www.arduino.cc/en/Guide/ArduinoEthernetShield) allows an Arduino board to connect to the internet using the Ethernet library and to read and write an SD card using the SD library.This shield is fully compatible with the former version, but relies on the newer W5500 chip.

 [Raspberry Pi](https://www.raspberrypi.org) is a series of small single-board computers developed in the United Kingdom by the Raspberry Pi Foundation to promote teaching of basic computer science in schools and in developing countries. Price range from $10-45 depending on model.

 [BeagleBone](https://beagleboard.org/bone) is a low-power open-source single-board computer produced by Texas Instruments. It runs Android, Ubuntu and other Linux flavors.

 [openPicus FlyportPro](https://www.open-electronics.org/flyport-professional-iot-modules-by-openpicus/) is a system on a module dedicated to IoT and M2M application, especially for professional use. Following some details on the solution: Why FlyportPRO SoM? A system-on-module is the best solution for those customers looking for flexibility and for development time and risk reduction.

 [Pinoccio](https://www.open-electronics.org/pinoccio-wifi-mesh-networking-for-arduino-and-iot-available-now/) is a solution to add mesh networking capability and WiFi-Internet access to all yout IoT devices, and it is Arduino compatible. Each board can assume the role of Scout in a Troop and one of the Scouts is the Lead to connect internet: Field Scouts talk to each other using a mesh network (called a Troop), using an extremely low-power radio.

### In-memory data grids
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

 [Ehcache](https://www.ehcache.org) is an open source, standards-based cache that boosts performance, offloads your database, and simplifies scalability. It's the most widely-used Java-based cache because it's robust, proven, full-featured, and integrates with other popular libraries and frameworks.

 [Hazelcast](https://hazelcast.com) is an open source in-memory data grid based on Java.

# Home automation
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

 [Home Assistant](https://github.com/home-assistant/core) is open source home automation that puts local control and privacy first. Powered by a worldwide community of tinkerers and DIY enthusiasts. Perfect to run on a Raspberry Pi or a local server.

 [openHAB](https://github.com/openhab) is a cross-platform software with the aim to integrate all kinds of Smart Home technologies, devices, etc. 

 [Eclipse SmartHome](https://www.eclipse.org/smarthome/) is a framework, not a ready-to-use solution. It offers a large set of features to choose from and leaves enough possibilities to design a Smart Home solution specific to your expectations. Its modular design brings millions of combinations and proves to be easily extensible by custom parts.

 [The Thing System](https://github.com/TheThingSystem) is a set of software components and network protocols that aims to fix the Internet of Things. Our steward software is written in node.js making it both portable and easily extensible. It can run on your laptop, or fit onto a small single board computer like the Raspberry Pi.

# Robotics
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/96352533-b55fb380-1078-11eb-874c-f165cbcce899.png">
  <br />
</p>

## Tools for Robotics

[Open Source Robotics Foundation](https://www.openrobotics.org/) works with industry, academia, and government to create and support open software and hardware for use in robotics, from research and education to product development.

[ROS](https://www.ros.org/) is robotics middleware. Although ROS is not an operating system, it provides services designed for a heterogeneous computer cluster such as hardware abstraction, low-level device control, implementation of commonly used functionality, message-passing between processes, and package management.

[ROS2](https://index.ros.org/doc/ros2/) is a set of [software libraries and tools](https://github.com/ros2) that help you build robot applications. From drivers to state-of-the-art algorithms, and with powerful developer tools, ROS has what you need for your next robotics project. And it’s all open source.

[Robot Framework](https://robotframework.org/) is a generic open source automation framework. It can be used for test automation and robotic process automation. It has easy syntax, utilizing human-readable keywords. Its capabilities can be extended by libraries implemented with Python or Java. 

[The Robotics Library (RL)](https://github.com/roboticslibrary/rl) is a self-contained C++ library for robot kinematics, motion planning and control. It covers mathematics, kinematics and dynamics, hardware abstraction, motion planning, collision detection, and visualization.RL runs on many different systems, including Linux, macOS, and Windows. It uses CMake as a build system and can be compiled with Clang, GCC, and Visual Studio.

[MoveIt](https://moveit.ros.org/) is the most widely used software for manipulation and has been used on over 100 robots. It provides an easy-to-use robotics platform for developing advanced applications, evaluating new designs and building integrated products for industrial, commercial, R&D, and other domains.

[AutoGluon](https://autogluon.mxnet.io/index.html) is toolkit for [Deep learning](https://gitlab.com/maos20008/intro-to-machine-learning) that automates machine learning tasks enabling you to easily achieve strong predictive performance in your applications. With just a few lines of code, you can train and deploy high-accuracy deep learning models on tabular, image, and text data.

[Gazebo](http://gazebosim.org/) accurately and efficiently simulates indoor and outdoor robots. You get a robust physics engine, high-quality graphics, and programmatic and graphical interfaces.

[Robotics System Toolbox](https://www.mathworks.com/products/robotics.html) provides tools and algorithms for designing, simulating, and testing manipulators, mobile robots, and humanoid robots. For manipulators and humanoid robots, the toolbox includes algorithms for collision checking, trajectory generation, forward and inverse kinematics, and dynamics using a rigid body tree representation. 
For mobile robots, it includes algorithms for mapping, localization, path planning, path following, and motion control. The toolbox provides reference examples of common industrial robot applications. It also includes a library of 
commercially available industrial robot models that you can import, visualize, and simulate.

[Intel Robot DevKit](https://github.com/intel/robot_devkit) is the tool to generate Robotics Software Development Kit (RDK) designed for autonomous devices, including the ROS2 core and capacibilities packages like perception, planning, control driver etc. It provides flexible build/runtime configurations to meet different autonomous requirement on top of diversity hardware choices, for example use different hareware engine CPU/GPU/VPU to accelerate AI related features.

[Arduino](https://www.arduino.cc/) is an open-source platform used for building electronics projects. Arduino consists of both a physical programmable circuit board (often referred to as a microcontroller) and a piece of software, or IDE (Integrated Development Environment) that runs on your computer, used to write and upload computer code to the physical board.

[ArduPilot](https://ardupilot.org/ardupilot/index.html) enables the creation and use of trusted, autonomous, unmanned vehicle systems for the peaceful benefit of all. ArduPilot provides a comprehensive suite of tools suitable for almost any vehicle and application.

[AirSim](https://github.com/Microsoft/AirSim) is a simulator for drones, cars and more, built on Unreal Engine (we now also have an experimental Unity release). It is open-source, cross platform, and supports hardware-in-loop with popular flight controllers such as PX4 for physically and visually realistic simulations.

[F´ (F Prime)](https://github.com/nasa/fprime) is a component-driven framework that enables rapid development and deployment of spaceflight and other embedded software applications. Originally developed at the Jet Propulsion Laboratory, F´ has been successfully deployed on several space applications.

[The JPL Open Source Rover](https://github.com/nasa-jpl/open-source-rover) is an open source, build it yourself, scaled down version of the 6 wheel rover design that JPL uses to explore the surface of Mars. The Open Source Rover is designed almost entirely out of consumer off the shelf (COTS) parts. This project is intended to be a teaching and learning experience for those who want to get involved in mechanical engineering, software, electronics, or robotics.

[Light Detection and Ranging(LiDAR)](https://en.wikipedia.org/wiki/Lidar) is a remote sensing method that uses light in the form of a pulsed laser at an object, and uses the time and wavelength of the reflected beam of light to estimate the distance and in some applications ([Laser Imaging](https://en.wikipedia.org/wiki/Laser_scanning)), to create a 3D representation of the object and its surface characteristics. This technology is commonly used in aircraft and self-driving vehicles.

[Neurorobotics Platform (NRP)](https://neurorobotics.net/) is an Internet-accessible simulation system that allows the simulation of robots controlled by spiking neural networks.

[ViSP](http://visp.inria.fr/) is an open-source visual servoing platform library, is able to compute control laws that can be applied to robotic systems.

[ROS Behavior Trees](https://github.com/miccol/ROS-Behavior-Tree) is an open-source library to create robot's behaviors in form of Behavior Trees running in ROS (Robot Operating System).

[g2core](https://github.com/synthetos/g2) is an open-source motion control software for CNC and Robotics, designed to run on Arduino Due class microcontrollers.

[ur5controller](https://github.com/roboticsleeds/ur5controller) is an open-source OpenRAVE controller for UR5 robot integrated with ROS.

[RBDL](https://github.com/rbdl/rbdl) is an open-source (zlib) C++ libray for both forward and inverse dynamics and kinematics. Also supports contacts and loops.

[Unity Robotics Hub](https://github.com/Unity-Technologies/Unity-Robotics-Hub) is a Central repository for open-source Unity packages, tutorials, and other resources demonstrating how to use Unity for robotics simulations. Includes new support for ROS integration.

[AliceVision](https://github.com/alicevision/AliceVision) is a Photogrammetric Computer Vision Framework which provides a 3D Reconstruction and Camera Tracking algorithms. AliceVision aims to provide strong software basis with state-of-the-art computer vision algorithms that can be tested, analyzed and reused. The project is a result of collaboration between academia and industry to provide cutting-edge algorithms with the robustness and the quality required for production usage.

[CARLA](https://github.com/carla-simulator/carla) is an open-source simulator for autonomous driving research. CARLA has been developed from the ground up to support development, training, and validation of autonomous driving systems. In addition to open-source code and protocols, CARLA provides open digital assets (urban layouts, buildings, vehicles) that were created for this purpose and can be used freely. The simulation platform supports flexible specification of sensor suites and environmental conditions.

[ROS bridge](https://github.com/carla-simulator/ros-bridge) is a package to bridge ROS for CARLA Simulator.

[ROS-Industrial](https://rosindustrial.org/) is an open source project that extends the advanced capabilities of ROS software to manufacturing.

[AWS RoboMaker](https://aws.amazon.com/robomaker/) is the most complete cloud solution for robotic developers to simulate, test and securely deploy robotic applications at scale. RoboMaker provides a fully-managed, scalable infrastructure for simulation that customers use for multi-robot simulation and CI/CD integration with regression testing in simulation.

[Microsoft Robotics Developer Studio](https://www.microsoft.com/en-us/download/details.aspx?id=29081)  is a free .NET-based programming environment for building robotics applications. 

[Visual Studio Code Extension for ROS](https://github.com/ms-iot/vscode-ros) is an extension provides support for Robot Operating System (ROS) development.

[Azure Kinect ROS Driver](https://github.com/microsoft/azure_kinect_ros_driver) is a node which publishes sensor data from the [Azure Kinect Developer Kit](https://azure.microsoft.com/en-us/services/kinect-dk/) to the [Robot Operating System (ROS)](http://www.ros.org/). Developers working with ROS can use this node to connect an Azure Kinect Developer Kit to an existing ROS installation.

[Azure IoT Hub for ROS](https://github.com/microsoft/ros_azure_iothub) is a ROS package works with the Microsoft Azure IoT Hub service to relay telemetry messages from the Robot to Azure IoT Hub or reflect properties from the Digital Twin to the robot using dynamic reconfigure.

[ROS 2 with ONNX Runtime](https://github.com/ms-iot/ros_msft_onnx) is a program that uses ROS 2 to run on different hardware platforms using their respective AI acceleration libraries for optimized execution of the ONNX model.

[Azure Cognitive Services LUIS ROS Node](https://github.com/ms-iot/ros_msft_luis) is a ROS node that bridges between ROS and the Azure Language Understanding Service. it can be configured to process audio directly from a microphone, or can subscribe to a ROS audio topic, then processes speech and generates "intent" ROS messages which can be processed by another ROS node to generate ROS commands. 

## Robotics Learning Resources

[Robotics courses from Coursera](https://www.edx.org/learn/robotics)

[Learn Robotics with Online Courses and Classes from edX](https://www.edx.org/learn/robotics)

[Top Robotics Courses Online from Udemy](https://www.udemy.com/topic/robotics/)

[Free Online AI & Robotics Courses](https://www.futurelearn.com/subjects/it-and-computer-science-courses/ai-and-robotics)

[REC Foundation Robotics Industry Certification](https://www.roboticseducation.org/industry-certifications/)

[Carnegie Mellon Robotics Academy](https://www.cmu.edu/roboticsacademy/Training/Certifications.html)

[RIA Robotic Integrator Certification Program](https://www.robotics.org/robotics/integrator-certification)

[AWS RoboMaker – Develop, Test, Deploy, and Manage Intelligent Robotics Apps](https://aws.amazon.com/blogs/aws/aws-robomaker-develop-test-deploy-and-manage-intelligent-robotics-apps/)

[Microsoft AI School](https://aischool.microsoft.com/en-us/home)

[Language Understanding (LUIS) for Azure Cognitive Services](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/what-is-luis)

[Azure VM templates to bootstrap ROS and ROS 2 environments](https://ms-iot.github.io/ROSOnWindows/ROSAtMS/AzureVM.html)

[Google Robotics Research](https://research.google/teams/brain/robotics/)

# Mesh networks
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

[Zigbee](https://csa-iot.org/all-solutions/zigbee/) is the full-stack, secure, reliable, and market-proven solution used by a majority of large smart home ecosystem providers, such as Amazon's Echo Plus, Samsung SmartThings, Signify (Philips Hue), and more.

 [Open Garden](https://opengarden.com) develops the FireChat mobile application, which enables peer-to-peer mobile Internet connection sharing with faster and more efficient data transmissions by automatically and actively choosing and switching to the best available network without requiring users to manually sift through available networks to find the best one available.

 [OpenWSN](https://github.com/openwsn-berkeley/) is a project created at the University of California Berkeley and extended at the INRIA and at the Open University of Catalonia which aims to build an open standard-based and open source implementation of a complete constrained network protocol stack for wireless sensor networks and Internet of Things.
 
# Blockchain Development
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/95128607-878c7d80-070e-11eb-8a0d-5f01b80eb478.png">
  <br />
</p>

## Blockchain Learning Resources

[Blockchain](https://www.blockchain.com/) is a distributed database meaning that the storage devices used for the database are not all connected to a common processor. It maintains a growing decentralized digital list of ordered records, called blocks. Each block has a timestamp and a link to a previous block. By the system being decentralization it allows for complete transparency in all shared information.

[IBM Blockchain Essentials](https://www.ibm.com/skills/topics/blockchain/)

[Getting started with Blockchain Development](https://docs.microsoft.com/en-us/learn/paths/ethereum-blockchain-development/)

[Blockchain Developer Nanodegree program | Udacity](https://www.udacity.com/course/blockchain-developer-nanodegree--nd1309)

[Blockchain Programming: Build a blockchain and cryptocurrency from scratch using Python | Udemy](https://www.udemy.com/course/build-your-own-cryptocurrency-in-48-hours/)

[Blockchain Courses by Coursera](https://www.coursera.org/courses?query=blockchain)

[Blockchain Courses by edX](https://www.edx.org/learn/blockchain)

[Blockchain Certifications](https://www.blockchain-council.org/)

## Blockchain Tools, Libraries and Frameworks

[Lightning Network (LN)](https://lightning.network/) is a decentralized network using smart contract functionality in the blockchain to enable instant payments across a network of participants. It was created in response to scalability issues with Bitcoin, namely the speed and cost of Bitcoin transactions. Bitcoin's current theoretical maximum transactions per second (TPS) is 10, though in reality it is between 3 and 7.

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/148870820-21722e8e-8fd3-4bd3-b755-d1e1cf006c29.png">
  <br />
</p>

[Hyperledger](https://www.hyperledger.org) is an open source community focused on developing a suite of stable frameworks, tools and libraries for enterprise-grade blockchain deployments. It serves as a neutral home for various distributed ledger frameworks including Hyperledger Fabric, Sawtooth, Indy, as well as tools like Hyperledger Caliper and libraries like Hyperledger Ursa.

[Hyperledger Caliper](https://www.hyperledger.org/use/caliper) is a blockchain benchmark tool, it allows users to measure the performance of a blockchain implementation with a set of predefined use cases. Hyperledger Caliper will produce reports containing a number of performance indicators to serve as a reference when using the following blockchain solutions: Hyperledger Besu, Hyperledger Burrow, Ethereum, Hyperledger Fabric, FISCO BCOS, Hyperledger Iroha and Hyperledger Sawtooth.

[Hyperledger Ursa](https://www.hyperledger.org/use/ursa) is a shared cryptographic library, it enables implementations to avoid duplicating other cryptographic work and hopefully increase security in the process. The library is an opt-in repository (for Hyperledger and non Hyperledger projects) to place and use crypto. Hyperledger Ursa consists of sub-projects, which are cohesive implementations of cryptographic code or interfaces to cryptographic code.

[Hyperledger Fabric](https://wiki.hyperledger.org/display/fabric) is an enterprise-grade permissioned distributed ledger framework for developing solutions and applications. Its modular and versatile design satisfies a broad range of industry use cases. It offers a unique approach to consensus that enables performance at scale while preserving privacy. 

[Geth](https://geth.ethereum.org/) is an implementation of an [Ethereum](https://ethereum.org/en/) node in the Go programming language. 

[Solidity](https://solidity.readthedocs.io/) is a purposefully slimmed down, loosely-typed language with a syntax very similar to ECMAScript (Javascript) that is used for the creation of smart contracts on the Ethereum blockchain. 

[GanacheCLI (NodeJS package)](https://www.trufflesuite.com/ganache) is a fast and customizable blockchain emulator. It simulates the Ethereum network on a single computer and allows you to make calls to the blockchain without any of the hassles of running a real Ethereum node.

[Truffle](https://trufflesuite.com/) is a development environment, testing framework and asset pipeline for Ethereum, aiming to make life as an Ethereum developer easier. 

[Ethers.js](https://github.com/ethers-io/ethers.js/) is a library which was made for and is used by ethers.io. It is designed to make it easier to write client-side JavaScript based wallets, keeping the private key on the owner’s machine at all times.

[OpenEthereum](https://github.com/openethereum/openethereum) is a fast and feature-rich multi-network Ethereum client.

[Quorum](https://www.goquorum.com/) is an Ethereum-based distributed ledger protocol with transaction/contract privacy and new consensus mechanisms.

[Diesel](https://diesel.rs/) is a safe, extensible ORM and Query Builder for [Rust](https://www.rust-lang.org/).

[BlockShell](https://github.com/daxeel/blockshell) is a minimal command line utility for learning Blockchain technical concepts like chaining & mining. 

[Tendermint Core](https://tendermint.com/) is [Byzantine Fault Tolerant (BFT)](https://en.wikipedia.org/wiki/Byzantine_fault_tolerance) middleware that takes a state transition machine written in any programming language and securely replicates it on many machines.

[inDEX](https://distribuyed.github.io/index/) is a comprehensive list of decentralized exchanges (DEX) of cryptocurrencies, tokens, derivatives and futures, and their protocols.

[Squeezer](https://squeezer.io/) is a platform that empowers new-entry blockchain developers to build serverless dApps easily. 
 
# Node.js Development
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/93719688-0becd700-fb39-11ea-9b87-3d52f1828aee.png">
  <br />
</p>

## Node.js Learning Resources

[Node.js](https://nodejs.org/) is a JavaScript runtime built on Chrome's V8 JavaScript engine that lets developers write command line tools and server-side scripts outside of a browser.

[Node.js Build Working Group](https://github.com/nodejs/build) maintains and controls infrastructure used for continuous integration (CI), releases, benchmarks, web hosting (of nodejs.org and other Node.js web properties) and more.

[The OpenJS Foundation](https://openjsf.org/) is made up of 32 open source JavaScript projects including Appium, Dojo, Electron, jQuery, Node.js, and webpack. The foundation's mission is to support the healthy growth of JavaScript and web technologies by providing a neutral organization to host and sustain projects, as well as collaboratively fund activities that benefit the ecosystem as a whole.

[Set up NodeJS on WSL 2](https://docs.microsoft.com/en-us/windows/nodejs/setup-on-wsl2)

[Getting started with Node.js in Google Cloud](https://cloud.google.com/nodejs/getting-started)

[Getting Started with Node.js in AWS](https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/getting-started-nodejs.html)

[Node.js App Hosting & Deployment in Microsoft Azure](https://azure.microsoft.com/en-us/develop/nodejs/)

[The Node.js best practices list ](https://github.com/goldbergyoni/nodebestpractices)

[Introduction to Node.js by W3Schools](https://www.w3schools.com/nodejs/nodejs_intro.asp)

[The Node.js Community Committee](https://github.com/nodejs/community-committee)

[Node.js Mentorship Program Initiative](https://github.com/nodejs/mentorship)

[Node.js tutorial in Visual Studio Code](https://code.visualstudio.com/docs/nodejs/nodejs-tutorial)

[Server-side Development with NodeJS, Express and MongoDB on Coursera](https://www.coursera.org/learn/server-side-nodejs)

## Node.js Tools

[NPM](https://www.npmjs.com/) is the company behind Node package manager, the npm Registry, and npm CLI. 

[node-gyp](https://github.com/nodejs/node-gyp) is a cross-platform command-line tool written in Node.js for compiling native addon modules for Node.js. It contains a vendored copy of the gyp-next project that was previously used by the Chromium team, extended to support the development of Node.js native addons.

[nvm ](https://github.com/nvm-sh/nvm) is a version manager for node.js, designed to be installed per-user, and invoked per-shell. nvm works on any POSIX-compliant shell (sh, dash, ksh, zsh, bash), in particular on these platforms: unix, macOS, and windows WSL.

[node-docker](https://hub.docker.com/_/node/) is the official Node.js docker image, made with love by the node community.

[Mocha](https://github.com/mochajs/mocha) is a simple, flexible, fun JavaScript test framework for Node.js & The Browser.

[AVA](https://github.com/avajs/ava) is a test runner for Node.js with a concise API, detailed error output, embrace of new language features and process isolation that lets you develop with confidence.

[egg](https://eggjs.org/) is a born to build better enterprise frameworks and apps with Node.js & Koa.

[mysqljs](https://github.com/mysqljs/mysql) is a pure node.js JavaScript Client implementing the MySQL protocol. 

[axios](https://github.com/axios/axios) is a promise based HTTP client for the browser and node.js.

[Fastify](https://www.fastify.io/) is a fast and low overhead web framework, for Node.js. 

[Express](https://expressjs.com/) is a fast, unopinionated, minimalist web framework for node.

[Meteor](https://www.meteor.com/) is an ultra-simple environment for building modern web applications with JavavScript. 

[NW.js](https://nwjs.io/) is an app runtime based on Chromium and node.js. You can write native apps in HTML and JavaScript with NW.js. It also lets you call Node.js modules directly from the DOM and enables a new way of writing native applications with all Web technologies.

[PM2](https://pm2.io/) is a production process manager for Node.js applications with a built-in load balancer. It allows you to keep applications alive forever, to reload them without downtime and to facilitate common system admin tasks.

[NestJS](https://nestjs.com/) is a framework for building efficient, scalable Node.js web applications. It uses modern JavaScript, is built with TypeScript and combines elements of OOP (Object Oriented Progamming), FP (Functional Programming), and FRP (Functional Reactive Programming).

[jenkins-nodejs](https://plugins.jenkins.io/nodejs/) is a Jenkins plugin for Node.js that provides the NodeJS auto-installer, allowing to create as many NodeJS installations "profiles" as you want.

[Strapi](https://strapi.io/) is an open source Node.js Headless CMS to easily build customisable APIs. 

[Standard](https://standardjs.com/) is a JavaScript Style Guide, with linter & automatic code fixer.

[React Starter Kit](https://www.reactstarterkit.com/) is an isomorphic web app boilerplate for web development built on top of [Node.js](https://nodejs.org/), [Express](http://expressjs.com/), [GraphQL](http://graphql.org/) and [React](https://facebook.github.io/react/), containing modern web development tools such as [Webpack](https://webpack.github.io/), [Babel](https://babeljs.io/) and [Browsersync](https://www.browsersync.io/). Helping you to stay productive following the best practices.

[Hexo](https://hexo.io/) is a A fast, simple & powerful blog framework, powered by Node.js. 

# C/C++ Development
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/115297894-961e0d80-a111-11eb-81c3-e2bd2ac9a7cd.png">
  <br />
</p>

## C/C++ Learning Resources

[C++](https://www.cplusplus.com/doc/tutorial/) is a cross-platform language that can be used to build high-performance applications developed by Bjarne Stroustrup, as an extension to the C language.

[C](https://www.iso.org/standard/74528.html) is a general-purpose, high-level language that was originally developed by Dennis M. Ritchie to develop the UNIX operating system at Bell Labs. It supports structured programming, lexical variable scope, and recursion, with a static type system. C also provides constructs that map efficiently to typical machine instructions, which makes it one was of the most widely used programming languages today.

[Embedded C](https://en.wikipedia.org/wiki/Embedded_C) is a set of language extensions for the C programming language by the [C Standards Committee](https://isocpp.org/std/the-committee) to address issues that exist between C extensions for different [embedded systems](https://en.wikipedia.org/wiki/Embedded_system). The extensions hep enhance microprocessor features such as fixed-point arithmetic, multiple distinct memory banks, and basic I/O operations. This makes Embedded C the most popular embedded software language in the world.

[C & C++ Developer Tools from JetBrains](https://www.jetbrains.com/cpp/)

[Open source C++ libraries on cppreference.com](https://en.cppreference.com/w/cpp/links/libs)

[C++ Graphics libraries](https://cpp.libhunt.com/libs/graphics)

[C++ Libraries in MATLAB](https://www.mathworks.com/help/matlab/call-cpp-library-functions.html)

[C++ Tools and Libraries Articles](https://www.cplusplus.com/articles/tools/)

[Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)

[Introduction C++ Education course on Google Developers](https://developers.google.com/edu/c++/)

[C++ style guide for Fuchsia](https://fuchsia.dev/fuchsia-src/development/languages/c-cpp/cpp-style)

[C and C++ Coding Style Guide by OpenTitan](https://docs.opentitan.org/doc/rm/c_cpp_coding_style/)

[Chromium C++ Style Guide](https://chromium.googlesource.com/chromium/src/+/master/styleguide/c++/c++.md)

[C++ Core Guidelines](https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md)

[C++ Style Guide for ROS](http://wiki.ros.org/CppStyleGuide)

[Learn C++](https://www.learncpp.com/)

[Learn C : An Interactive C Tutorial](https://www.learn-c.org/)

[C++ Institute](https://cppinstitute.org/free-c-and-c-courses)

[C++ Online Training Courses on LinkedIn Learning](https://www.linkedin.com/learning/topics/c-plus-plus)

[C++ Tutorials on W3Schools](https://www.w3schools.com/cpp/default.asp)

[Learn C Programming Online Courses on edX](https://www.edx.org/learn/c-programming)

[Learn C++ with Online Courses on edX](https://www.edx.org/learn/c-plus-plus)

[Learn C++ on Codecademy](https://www.codecademy.com/learn/learn-c-plus-plus)

[Coding for Everyone: C and C++ course on Coursera](https://www.coursera.org/specializations/coding-for-everyone)

[C++ For C Programmers on Coursera](https://www.coursera.org/learn/c-plus-plus-a)

[Top C Courses on Coursera](https://www.coursera.org/courses?query=c%20programming)

[C++ Online Courses on Udemy](https://www.udemy.com/topic/c-plus-plus/)

[Top C Courses on Udemy](https://www.udemy.com/topic/c-programming/)

[C++ For Programmers Course on Udacity](https://www.udacity.com/course/c-for-programmers--ud210)

[C++ Fundamentals Course on Pluralsight](https://www.pluralsight.com/courses/learn-program-cplusplus)

[Introduction to C++ on MIT Free Online Course Materials](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-096-introduction-to-c-january-iap-2011/)

[Introduction to C++ for Programmers | Harvard ](https://online-learning.harvard.edu/course/introduction-c-programmers)

[Online C Courses | Harvard University](https://online-learning.harvard.edu/subject/c)

## C/C++ Tools

[Visual Studio](https://visualstudio.microsoft.com/) is an integrated development environment (IDE) from Microsoft; which is a feature-rich application that can be used for many aspects of software development. Visual Studio makes it easy to edit, debug, build, and publish your app. By using Microsoft software development platforms such as Windows API, Windows Forms, Windows Presentation Foundation, and Windows Store.

[Visual Studio Code](https://code.visualstudio.com/) is a code editor redefined and optimized for building and debugging modern web and cloud applications.

[Vcpkg](https://github.com/microsoft/vcpkg) is a C++ Library Manager for Windows, Linux, and MacOS.

[ReSharper C++](https://www.jetbrains.com/resharper-cpp/features/) is a Visual Studio Extension for C++ developers developed by JetBrains.

[AppCode](https://www.jetbrains.com/objc/) is constantly monitoring the quality of your code. It warns you of errors and smells and suggests quick-fixes to resolve them automatically. AppCode provides lots of code inspections for Objective-C, Swift, C/C++, and a number of code inspections for other supported languages. All code inspections are run on the fly.

[CLion](https://www.jetbrains.com/clion/features/) is a cross-platform IDE for C and C++ developers developed by JetBrains.

[Code::Blocks](https://www.codeblocks.org/) is a free C/C++ and Fortran IDE built to meet the most demanding needs of its users. It is designed to be very extensible and fully configurable. Built around a plugin framework, Code::Blocks can be extended with plugins.

[CppSharp](https://github.com/mono/CppSharp) is a tool and set of libraries which facilitates the usage of native C/C++ code with the .NET ecosystem. It consumes C/C++ header and library files and generates the necessary glue code to surface the native API as a managed API. Such an API can be used to consume an existing native library in your managed code or add managed scripting support to a native codebase.

[Conan](https://conan.io/) is an Open Source Package Manager for C++ development and dependency management into the 21st century and on par with the other development ecosystems.

[High Performance Computing (HPC) SDK](https://developer.nvidia.com/hpc) is a comprehensive toolbox for GPU accelerating HPC modeling and simulation applications. It includes the C, C++, and Fortran compilers, libraries, and analysis tools necessary for developing HPC applications on the NVIDIA platform.

[Thrust](https://github.com/NVIDIA/thrust) is a C++ parallel programming library which resembles the C++ Standard Library. Thrust's high-level interface greatly enhances programmer productivity while enabling performance portability between GPUs and multicore CPUs. Interoperability with established technologies such as CUDA, TBB, and OpenMP integrates with existing software.

[Boost](https://www.boost.org/) is an educational opportunity focused on cutting-edge C++. Boost has been a participant in the annual Google Summer of Code since 2007, in which students develop their skills by working on Boost Library development.

[Automake](https://www.gnu.org/software/automake/) is a tool for automatically generating Makefile.in files compliant with the GNU Coding Standards. Automake requires the use of GNU Autoconf.

[Cmake](https://cmake.org/) is an open-source, cross-platform family of tools designed to build, test and package software. CMake is used to control the software compilation process using simple platform and compiler independent configuration files, and generate native makefiles and workspaces that can be used in the compiler environment of your choice.

[GDB](http://www.gnu.org/software/gdb/) is a debugger, that allows you to see what is going on `inside' another program while it executes or what another program was doing at the moment it crashed.

[GCC](https://gcc.gnu.org/) is a compiler Collection that includes front ends for C, C++, Objective-C, Fortran, Ada, Go, and D, as well as libraries for these languages.

[GSL](https://www.gnu.org/software/gsl/) is a numerical library for C and C++ programmers. It is free software under the GNU General Public License. The library provides a wide range of mathematical routines such as random number generators, special functions and least-squares fitting. There are over 1000 functions in total with an extensive test suite.

[OpenGL Extension Wrangler Library (GLEW)](https://www.opengl.org/sdk/libs/GLEW/) is a cross-platform open-source C/C++ extension loading library. GLEW provides efficient run-time mechanisms for determining which OpenGL extensions are supported on the target platform.

[Libtool](https://www.gnu.org/software/libtool/) is a generic library support script that hides the complexity of using shared libraries behind a consistent, portable interface. To use Libtool, add the new generic library building commands to your Makefile, Makefile.in, or Makefile.am.

[Maven](https://maven.apache.org/) is a software project management and comprehension tool. Based on the concept of a project object model (POM), Maven can manage a project's build, reporting and documentation from a central piece of information.

[TAU (Tuning And Analysis Utilities)](http://www.cs.uoregon.edu/research/tau/home.php) is capable of gathering performance information through instrumentation of functions, methods, basic blocks, and statements as well as event-based sampling. All C++ language features are supported including templates and namespaces.

[Clang](https://clang.llvm.org/) is a production quality C, Objective-C, C++ and Objective-C++ compiler when targeting X86-32, X86-64, and ARM (other targets may have caveats, but are usually easy to fix). Clang is used in production to build performance-critical software like Google Chrome or Firefox.

[OpenCV](https://opencv.org/) is a highly optimized library with focus on real-time applications. Cross-Platform C++, Python and Java interfaces support Linux, MacOS, Windows, iOS, and Android.

[Libcu++](https://nvidia.github.io/libcudacxx) is the NVIDIA C++ Standard Library for your entire system. It provides a heterogeneous implementation of the C++ Standard Library that can be used in and between CPU and GPU code.

[ANTLR (ANother Tool for Language Recognition)](https://www.antlr.org/) is a powerful parser generator for reading, processing, executing, or translating structured text or binary files. It's widely used to build languages, tools, and frameworks. From a grammar, ANTLR generates a parser that can build parse trees and also generates a listener interface that makes it easy to respond to the recognition of phrases of interest.

[Oat++](https://oatpp.io/) is a light and powerful C++ web framework for highly scalable and resource-efficient web application. It's zero-dependency and easy-portable.

[JavaCPP](https://github.com/bytedeco/javacpp) is a program that provides efficient access to native C++ inside Java, not unlike the way some C/C++ compilers interact with assembly language.

[Cython](https://cython.org/) is a language that makes writing C extensions for Python as easy as Python itself. Cython is based on Pyrex, but supports more cutting edge functionality and optimizations such as calling C functions and declaring C types on variables and class attributes.

[Spdlog](https://github.com/gabime/spdlog) is a very fast, header-only/compiled, C++ logging library.

[Infer](https://fbinfer.com/) is a static analysis tool for Java, C++, Objective-C, and C. Infer is written in [OCaml](https://ocaml.org/).

# Java Development
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/93925952-c0b6fd80-fccb-11ea-9f90-21c4148e3c86.png">
  <br />
</p>


## Java Learning Resources

[Java](https://www.oracle.com/java/) is a popular programming language and development platform(JDK). It reduces costs, shortens development timeframes, drives innovation, and improves application services. With millions of developers running more than 51 billion Java Virtual Machines worldwide.

[The Eclipse Foundation](https://www.eclipse.org/downloads/) is home to a worldwide community of developers, the Eclipse IDE, Jakarta EE and over 375 open source projects, including runtimes, tools and frameworks for Java and other languages.

[Getting Started with Java](https://docs.oracle.com/javase/tutorial/)

[Oracle Java certifications from Oracle University](https://education.oracle.com/java-certification-benefits)

[Google Developers Training](https://developers.google.com/training/)

[Google Developers Certification](https://developers.google.com/certification/)

[Java Tutorial by W3Schools](https://www.w3schools.com/java/)

[Building Your First Android App in Java](codelabs.developers.google.com/codelabs/build-your-first-android-app/)

[Getting Started with Java in Visual Studio Code](https://code.visualstudio.com/docs/java/java-tutorial)

[Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)

[AOSP Java Code Style for Contributors](https://source.android.com/setup/contribute/code-style)

[Chromium Java style guide](https://chromium.googlesource.com/chromium/src/+/master/styleguide/java/java.md)

[Get Started with OR-Tools for Java](https://developers.google.com/optimization/introduction/java)

[Getting started with Java Tool Installer task for Azure Pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/tool/java-tool-installer)

[Gradle User Manual](https://docs.gradle.org/current/userguide/userguide.html)

## Java Tools & Frameworks

[Java SE](https://www.oracle.com/java/technologies/javase/tools-jsp.html) contains several tools to assist in program development and debugging, and in the monitoring and troubleshooting of production applications. 

[JDK Development Tools](https://docs.oracle.com/javase/7/docs/technotes/tools/) includes the Java Web Start Tools (javaws) Java Troubleshooting, Profiling, Monitoring and Management Tools (jcmd, jconsole, jmc, jvisualvm); and Java Web Services Tools (schemagen, wsgen, wsimport, xjc).

[Android Studio](https://developer.android.com/studio/) is the official integrated development environment for Google's Android operating system, built on JetBrains' IntelliJ IDEA software and designed specifically for Android development. Availble on Windows, macOS, Linux, Chrome OS.

[IntelliJ IDEA](https://www.jetbrains.com/idea/) is an IDE for Java, but it also understands and provides intelligent coding assistance for a large variety of other languages such as Kotlin, SQL, JPQL, HTML, JavaScript, etc., even if the language expression is injected into a String literal in your Java code.

[NetBeans](https://netbeans.org/features/java/index.html) is an IDE provides Java developers with all the tools needed to create professional desktop, mobile and enterprise applications. Creating, Editing, and Refactoring. The IDE provides wizards and templates to let you create Java EE, Java SE, and Java ME applications.

[Java Design Patterns ](https://github.com/iluwatar/java-design-patterns) is a collection of the best formalized practices a programmer can use to solve common problems when designing an application or system.

[Elasticsearch](https://www.elastic.co/products/elasticsearch) is a distributed RESTful search engine built for the cloud written in Java.

[RxJava](https://github.com/ReactiveX/RxJava) is a Java VM implementation of [Reactive Extensions](http://reactivex.io/): a library for composing asynchronous and event-based programs by using observable sequences. It extends the [observer pattern](http://en.wikipedia.org/wiki/Observer_pattern) to support sequences of data/events and adds operators that allow you to compose sequences together declaratively while abstracting away concerns about things like low-level threading, synchronization, thread-safety and concurrent data structures.

[Guava](https://github.com/google/guava) is a set of core Java libraries from Google that includes new collection types (such as multimap and multiset), immutable collections, a graph library, and utilities for concurrency, I/O, hashing, caching, primitives, strings, and more! It is widely used on most Java projects within Google, and widely used by many other companies as well.

[okhttp](https://square.github.io/okhttp/) is a HTTP client for Java and Kotlin developed by Square. 

[Retrofit](https://square.github.io/retrofit/) is a type-safe HTTP client for Android and Java develped by Square.

[LeakCanary](https://square.github.io/leakcanary/) is a memory leak detection library for Android develped by Square.

[Apache Spark](https://spark.apache.org/) is a unified analytics engine for large-scale data processing. It provides high-level APIs in Scala, Java, Python, and R, and an optimized engine that supports general computation graphs for data analysis. It also supports a rich set of higher-level tools including Spark SQL for SQL and DataFrames, MLlib for machine learning, GraphX for graph processing, and Structured Streaming for stream processing.

[Apache Flink](https://flink.apache.org/) is an open source stream processing framework with powerful stream- and batch-processing capabilities with elegant and fluent APIs in Java and Scala.

[Fastjson](https://github.com/alibaba/fastjson/wiki) is a Java library that can be used to convert Java Objects into their JSON representation. It can also be used to convert a JSON string to an equivalent Java object.

[libGDX](https://libgdx.com/) is a cross-platform Java game development framework based on OpenGL (ES) that works on Windows, Linux, Mac OS X, Android, your WebGL enabled browser and iOS.

[Jenkins](https://www.jenkins.io/) is the leading open-source automation server. Built with Java, it provides over 1700 [plugins](https://plugins.jenkins.io/) to support automating virtually anything, so that humans can actually spend their time doing things machines cannot.

[DBeaver](https://dbeaver.io/) is a free multi-platform database tool for developers, SQL programmers, database administrators and analysts. Supports any database which has JDBC driver (which basically means - ANY database). EE version also supports non-JDBC datasources (MongoDB, Cassandra, Redis, DynamoDB, etc).

[Redisson](https://redisson.pro/) is a Redis Java client with features of In-Memory Data Grid. Over 50 Redis based Java objects and services: Set, Multimap, SortedSet, Map, List, Queue, Deque, Semaphore, Lock, AtomicLong, Map Reduce, Publish / Subscribe, Bloom filter, Spring Cache, Tomcat, Scheduler, JCache API, Hibernate, MyBatis, RPC, and local cache.

[GraalVM](https://www.graalvm.org/) is a universal virtual machine for running applications written in JavaScript, Python, Ruby, R, JVM-based languages like Java, Scala, Clojure, Kotlin, and LLVM-based languages such as C and C++.

[Gradle](https://gradle.org/) is a build automation tool for multi-language software development. From mobile apps to microservices, from small startups to big enterprises, Gradle helps teams build, automate and deliver better software, faster. Write in Java, C++, Python or your language of choice. 

[Apache Groovy](http://www.groovy-lang.org/) is a powerful, optionally typed and dynamic language, with static-typing and static compilation capabilities, for the Java platform aimed at improving developer productivity thanks to a concise, familiar and easy to learn syntax. It integrates smoothly with any Java program, and immediately delivers to your application powerful features, including scripting capabilities, Domain-Specific Language authoring, runtime and compile-time meta-programming and functional programming. 

[JaCoCo](https://www.jacoco.org/jacoco/) is a free code coverage library for Java, which has been created by the EclEmma team based on the lessons learned from using and integration existing libraries for many years.

[Apache JMeter](http://jmeter.apache.org/) is  used to test performance both on static and dynamic resources, Web dynamic applications. It also used to simulate a heavy load on a server, group of servers, network or object to test its strength or to analyze overall performance under different load types.

[Junit](https://junit.org/) is a simple framework to write repeatable tests. It is an instance of the xUnit architecture for unit testing frameworks.

[Mockito](https://site.mockito.org/) is the most popular Mocking framework for unit tests written in Java.

[SpotBugs](https://spotbugs.github.io/) is a program which uses static analysis to look for bugs in Java code.

[SpringBoot](https://spring.io/projects/spring-boot) is a great tool that helps you to create Spring-powered, production-grade applications and services with absolute minimum fuss. It takes an opinionated view of the Spring platform so that new and existing users can quickly get to the bits they need.

[YourKit](https://www.yourkit.com/) is a technology leader, creator of the most innovative and intelligent tools for profiling Java & .NET applications.

# Python Development
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/93133273-ce490380-f68b-11ea-81d0-7f6a3debe6c0.png">
  <br />
  
</p>


## Python Learning Resources

[Python](https://www.python.org) is an interpreted, high-level programming language. Python is used heavily in the fields of Data Science and Machine Learning. 

[Python Developer’s Guide](https://devguide.python.org) is a comprehensive resource for contributing to Python – for both new and experienced contributors. It is maintained by the same community that maintains Python. 

[Azure Functions Python developer guide](https://docs.microsoft.com/en-us/azure/azure-functions/functions-reference-python) is an introduction to developing Azure Functions using Python. The content below assumes that you've already read the [Azure Functions developers guide](https://docs.microsoft.com/en-us/azure/azure-functions/functions-reference).

[CheckiO](https://checkio.org/) is a programming learning platform and a gamified website that teaches Python through solving code challenges and competing for the most elegant and creative solutions.

[Python Institute](https://pythoninstitute.org)

[PCEP – Certified Entry-Level Python Programmer certification](https://pythoninstitute.org/pcep-certification-entry-level/)

[PCAP – Certified Associate in Python Programming certification](https://pythoninstitute.org/pcap-certification-associate/)

[PCPP – Certified Professional in Python Programming 1 certification](https://pythoninstitute.org/pcpp-certification-professional/)

[PCPP – Certified Professional in Python Programming 2](https://pythoninstitute.org/pcpp-certification-professional/)

[MTA: Introduction to Programming Using Python Certification](https://docs.microsoft.com/en-us/learn/certifications/mta-introduction-to-programming-using-python)

[Getting Started with Python in Visual Studio Code](https://code.visualstudio.com/docs/python/python-tutorial)

[Google's Python Style Guide](https://google.github.io/styleguide/pyguide.html)

[Google's Python Education Class](https://developers.google.com/edu/python/)

[Real Python](https://realpython.com)

[The Python Open Source Computer Science Degree by Forrest Knight](https://github.com/ForrestKnight/open-source-cs-python)

[Intro to Python for Data Science](https://www.datacamp.com/courses/intro-to-python-for-data-science)

[Intro to Python by W3schools](https://www.w3schools.com/python/python_intro.asp)

[Codecademy's Python 3 course](https://www.codecademy.com/learn/learn-python-3)

[Learn Python with Online Courses and Classes from edX](https://www.edx.org/learn/python)

[Python Courses Online from Coursera](https://www.coursera.org/courses?query=python)

## Python Frameworks and Tools

[Python Package Index (PyPI)](https://pypi.org/) is a repository of software for the Python programming language. PyPI helps you find and install software developed and shared by the Python community. 

[PyCharm](https://www.jetbrains.com/pycharm/) is the best IDE I've ever used. With PyCharm, you can access the command line, connect to a database, create a virtual environment, and manage your version control system all in one place, saving time by avoiding constantly switching between windows.

[Python Tools for Visual Studio(PTVS)](https://microsoft.github.io/PTVS/) is a free, open source plugin that turns Visual Studio into a Python IDE. It supports editing, browsing, IntelliSense, mixed Python/C++ debugging, remote Linux/MacOS debugging, profiling, IPython, and web development with Django and other frameworks.

[Pylance](https://github.com/microsoft/pylance-release) is an extension that works alongside Python in Visual Studio Code to provide performant language support. Under the hood, Pylance is powered by Pyright, Microsoft's static type checking tool.

[Pyright](https://github.com/Microsoft/pyright) is a fast type checker meant for large Python source bases. It can run in a “watch” mode and performs fast incremental updates when files are modified.

[Django](https://www.djangoproject.com/) is a high-level Python Web framework that encourages rapid development and clean, pragmatic design.

[Flask](https://flask.palletsprojects.com/) is a micro web framework written in Python. It is classified as a microframework because it does not require particular tools or libraries. 
 
[Web2py](http://web2py.com/) is an open-source web application framework written in Python allowing allows web developers to program dynamic web content. One web2py instance can run multiple web sites using different databases.

[AWS Chalice](https://github.com/aws/chalice) is a framework for writing serverless apps in python. It allows you to quickly create and deploy applications that use AWS Lambda. 

[Tornado](https://www.tornadoweb.org/) is a Python web framework and asynchronous networking library. Tornado uses a non-blocking network I/O, which can scale to tens of thousands of open connections.

[HTTPie](https://github.com/httpie/httpie) is a command line HTTP client that makes CLI interaction with web services as easy as possible. HTTPie is designed for testing, debugging, and generally interacting with APIs & HTTP servers. 

[Scrapy](https://scrapy.org/) is a fast high-level web crawling and web scraping framework, used to crawl websites and extract structured data from their pages. It can be used for a wide range of purposes, from data mining to monitoring and automated testing.

[Sentry](https://sentry.io/) is a service that helps you monitor and fix crashes in realtime. The server is in Python, but it contains a full API for sending events from any language, in any application.

[Pipenv](https://github.com/pypa/pipenv) is a tool that aims to bring the best of all packaging worlds (bundler, composer, npm, cargo, yarn, etc.) to the Python world.

[Python Fire](https://github.com/google/python-fire) is a library for automatically generating command line interfaces (CLIs) from absolutely any Python object.

[Bottle](https://github.com/bottlepy/bottle) is a fast, simple and lightweight [WSGI](https://www.wsgi.org/) micro web-framework for Python. It is distributed as a single file module and has no dependencies other than the [Python Standard Library](https://docs.python.org/library/).

[CherryPy](https://cherrypy.org) is a minimalist Python object-oriented HTTP web framework.

[Sanic](https://github.com/huge-success/sanic) is a Python 3.6+ web server and web framework that's written to go fast. 

[Pyramid](https://trypyramid.com) is a small and fast open source Python web framework. It makes real-world web application development and deployment more fun and more productive.

[TurboGears](https://turbogears.org) is a hybrid web framework able to act both as a Full Stack framework or as a Microframework. 

[Falcon](https://falconframework.org/) is a reliable, high-performance Python web framework for building large-scale app backends and microservices with support for MongoDB, Pluggable Applications and autogenerated Admin.

[Neural Network Intelligence(NNI)](https://github.com/microsoft/nni) is an open source AutoML toolkit for automate machine learning lifecycle, including [Feature Engineering](https://github.com/microsoft/nni/blob/master/docs/en_US/FeatureEngineering/Overview.md), [Neural Architecture Search](https://github.com/microsoft/nni/blob/master/docs/en_US/NAS/Overview.md), [Model Compression](https://github.com/microsoft/nni/blob/master/docs/en_US/Compressor/Overview.md) and [Hyperparameter Tuning](https://github.com/microsoft/nni/blob/master/docs/en_US/Tuner/BuiltinTuner.md).

[Dash](https://plotly.com/dash) is a popular Python framework for building ML & data science web apps for Python, R, Julia, and Jupyter.

[Luigi](https://github.com/spotify/luigi) is a Python module that helps you build complex pipelines of batch jobs. It handles dependency resolution, workflow management, visualization etc. It also comes with Hadoop support built-in.

[Locust](https://github.com/locustio/locust) is an easy to use, scriptable and scalable performance testing tool. 

[spaCy](https://github.com/explosion/spaCy) is a library for advanced Natural Language Processing in Python and Cython. 

[NumPy](https://www.numpy.org/) is the fundamental package needed for scientific computing with Python.

[Pillow](https://python-pillow.org/) is a friendly PIL(Python Imaging Library) fork.

[IPython](https://ipython.org/) is a command shell for interactive computing in multiple programming languages, originally developed for the Python programming language, that offers enhanced introspection, rich media, additional shell syntax, tab completion, and rich history.

[GraphLab Create](https://turi.com/) is a Python library, backed by a C++ engine, for quickly building large-scale, high-performance machine learning models.

[Pandas](https://pandas.pydata.org/) is a fast, powerful, and easy to use open source data structrures, data analysis and manipulation tool, built on top of the Python programming language.

[PuLP](https://coin-or.github.io/pulp/) is an Linear Programming modeler written in python. PuLP can generate LP files and call on use highly optimized solvers, GLPK, COIN CLP/CBC, CPLEX, and GUROBI, to solve these linear problems.

[Matplotlib](https://matplotlib.org/) is a 2D plotting library for creating static, animated, and interactive visualizations in Python. Matplotlib produces publication-quality figures in a variety of hardcopy formats and interactive environments across platforms.

[Scikit-Learn](https://scikit-learn.org/stable/index.html) is a simple and efficient tool for data mining and data analysis. It is built on NumPy,SciPy, and mathplotlib.

# Rust Development
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/93025405-8dc98700-f5b2-11ea-93f9-12b4a0ef3001.png">
  <br />
</p>


## Rust Learning Resources

[Rust](https://www.rust-lang.org) is a multi-paradigm programming language focused on performance and safety. Rust has a comparable amount of runtime to C and C++, and has set up its standard library to be amenable towards OS development. Specifically, the standard library is split into two parts: core and std. Core is the lowest-level aspects only, and doesn't include things like allocation, threading, and other higher-level features.

[The Rust Language Reference](https://doc.rust-lang.org/nightly/reference/)

[The Rust Programming Language Book](https://doc.rust-lang.org/book/)

[Learning Rust](https://www.rust-lang.org/learn)

[Why AWS loves Rust](https://aws.amazon.com/blogs/opensource/why-aws-loves-rust-and-how-wed-like-to-help/)

[Rust Programming courses on Udemy](https://www.udemy.com/courses/search/?src=ukw&q=Rust)

[Safety in Systems Programming with Rust at Standford by Ryan Eberhardt](https://reberhardt.com/blog/2020/10/05/designing-a-new-class-at-stanford-safety-in-systems-programming.html)

[WebAssembly meets Kubernetes with Krustlet using Rust](https://cloudblogs.microsoft.com/opensource/2020/04/07/announcing-krustlet-kubernetes-rust-kubelet-webassembly-wasm/)

[Microsoft's Project Verona](https://github.com/microsoft/verona/blob/master/docs/explore.md)

## Rust Tools

[Cargo](https://github.com/rust-lang/cargo) is a package manager that downloads your Rust project’s dependencies and compiles your project.

[Crater](https://crater.rust-lang.org/) is a tool to run experiments across parts of the Rust ecosystem. Its primary purpose is to detect regressions in the Rust compiler, and it does this by building a large number of crates, running their test suites and comparing the results between two versions of the Rust compiler. It can operate locally (with Docker as the only dependency) or distributed on the cloud.

[VSCode-Rust](https://github.com/rust-lang/vscode-rust) is plugin that adds language support for Rust to Visual Studio Code. Rust support is powered by a separate language server - either by the official Rust Language Server (RLS) or rust-analyzer, depending on the user's preference. If you don't have it installed, the extension will install it for you (with permission). This extension is built and maintained by the Rust IDEs and editors team with the focus on providing a stable, high quality extension that makes the best use of the respective language server. 

[Apache Arrow](https://github.com/apache/arrow) is a development platform for in-memory analytics. It contains a set of technologies that enable big data systems to process and move data fast. Arrow's libraries are available for C, C++, C#, Go, Java, JavaScript, MATLAB, Python, R, Ruby, and Rust.

[Wasmer](https://wasmer.io/) enables super lightweight containers based on [WebAssembly](https://webassembly.org/) that can run anywhere such as the Desktop to the Cloud and IoT devices, and also embedded in [any programming language](https://github.com/wasmerio/wasmer#language-integrations).

[Firecracker](https://firecracker-microvm.github.io) is an open source virtualization technology that is purpose-built for creating and managing secure, multi-tenant container and function-based services that provide serverless operational models. Firecracker runs workloads in lightweight virtual machines, called microVMs, which combine the security and isolation properties provided by hardware virtualization technology with the speed and flexibility of containers. Firecracker has also been integrated in container runtimes, for example [Kata Containers](https://github.com/kata-containers/documentation/wiki/Initial-release-of-Kata-Containers-with-Firecracker-support) and [Weaveworks Ignite](https://github.com/weaveworks/ignite).

[Tokio](https://github.com/tokio-rs/tokio) is an event-driven, non-blocking I/O platform for writing asynchronous applications with the Rust programming language.

[TiKV](https://github.com/tikv/tikv) is an open-source distributed transactional key-value database that also provides classical key-vlue APIs, but also transactional APIs with ACID compliance.

[Sonic](https://crates.io/crates/sonic-server) is a fast, lightweight and schema-less search backend similar to Elasticsearch in some use-cases.

[Hyper](https://github.com/hyperium/hyper) is a fast and correct HTTP library for Rust.

[Rocket](https://github.com/SergioBenitez/Rocket) is an async web framework for Rust with a focus on usability, security, extensibility, and speed.

[Clippy](https://rust-lang.github.io/rust-clippy/) is a collection of lints to catch common mistakes and improve your Rust code.

[Servo](https://github.com/servo/servo) is a prototype web browser engine written in the Rust language.

[Vector](https://vector.dev/) is a high-performance, end-to-end (agent & aggregator) observability data platform that puts the user in control of their observability data.

[RustPython](https://github.com/RustPython/RustPython) is a Python Interpreter written in Rust.

[Miri](https://github.com/rust-lang/miri) is an interpreter for Rust's mid-level intermediate representation. It can run binaries and test suites of cargo projects and detect certain classes of undefined behavior. Miri will alsowill also tell you about memory leaks: when there is memory still allocated at the end of the execution, and that memory is not reachable from a global static, Miri will raise an error.

[Chalk](https://rust-lang.github.io/chalk/book/) is an implementation and definition of the Rust trait system using a PROLOG-like logic solver.

[stdarch](https://doc.rust-lang.org/stable/core/arch/) is Rust's standard library vendor-specific APIs and run-time feature detection.

[Simpleinfra](https://github.com/rust-lang/simpleinfra) is rep that contains the tools and automation written by the Rust infrastructure team to manage our services. Using some of the tools in this repo require privileges only infra team members have.

[Rustlings](https://github.com/rust-lang/rustlings) is a small set of exercises to get you used to reading and writing Rust code.

[Krustlet](https://krustlet.dev/) acts as a Kubernetes Kubelet(written in Rust) by listening on the event stream for new pods that the scheduler assigns to it based on specific Kubernetes [tolerations](https://kubernetes.io/docs/concepts/configuration/taint-and-toleration/). The project is currently experimental.

## Operating System

[Redox](https://www.redox-os.org) is a Unix-like Operating System written in Rust, aiming to bring the innovations of Rust to a modern microkernel and full set of applications. Acitvely being developed by [Jeremy Soeller](https://gitlab.redox-os.org/jackpot51).

[Bottlerocket OS](https://github.com/bottlerocket-os/bottlerocket) is an open-source Linux-based operating system meant for hosting containers. Bottlerocket focuses on security and maintainability, providing a reliable, consistent, and safe platform for container-based workloads.

[Tock](https://www.tockos.org) is an embedded operating system designed for running multiple concurrent, mutually distrustful applications on Cortex-M and RISC-V based embedded platforms. Tock's design centers around protection, both from potentially malicious applications and from device drivers. Tock uses two mechanisms to protect different components of the operating system. First, the kernel and device drivers are written in Rust, a systems programming language that provides compile-time memory safety, type safety and strict aliasing. Tock uses Rust to protect the kernel (the scheduler and hardware abstraction layer) from platform specific device drivers as well as isolate device drivers from each other. Second, Tock uses memory protection units to isolate applications from each other and the kernel.

[Rust on Chrome OS](https://chromium.googlesource.com/chromiumos/docs/+/master/rust_on_cros.md) is a document that provides information on creating Rust projects for installation within Chrome OS and Chrome OS SDK. 

[Writing an OS in Rust ](https://os.phil-opp.com) is a blog series creates a small operating system in the Rust programming language by [Philipp Oppermann](https://github.com/phil-opp). 

# Swift Development
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/93719675-03949c00-fb39-11ea-8f81-bf4cd544c17f.png">
</p>


## Swift Learning Resources

[Swift](https://developer.apple.com/swift/) is Apple's main programming language for iOS, macOS, watchOS, and tvOS app development. Though, many parts of Swift will be familiar to developers from their experience of developing in C and Objective-C.

[Swift Evolution](https://github.com/apple/swift-evolution) maintains proposals for changes and user-visible enhancements to the Swift Programming Language.

[Xcode + Swift](https://developer.apple.com/swift/resources/) makes developing applications for MacOS and iOS fast and fun.

[Swift 5.3 Basics](https://docs.swift.org/swift-book/LanguageGuide/TheBasics.html)

[Start Developing iOS Apps with Swift](https://developer.apple.com/library/archive/referencelibrary/GettingStarted/DevelopiOSAppsSwift/)

[Apple Developer Documentation](https://developer.apple.com/documentation)

[Apple Foundation Framework](https://developer.apple.com/documentation/foundation)

[Apple Core Animation Framework](https://developer.apple.com/documentation/quartzcore)

[Apple Core Graphics Framework](https://developer.apple.com/documentation/coregraphics)

[Getting Started with LLDB](https://developer.apple.com/library/archive/documentation/IDEs/Conceptual/gdb_to_lldb_transition_guide/document/lldb-basics.html)

[Mac Catalyst - iOS - Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines/ios/overview/mac-catalyst/)

[Amazon EC2 Mac Instances](https://aws.amazon.com/ec2/instance-types/mac/)

[Swift GitHub](https://github.com/apple/swift) 

[Apple Developer Forums](https://developer.apple.com/forums/)

[Swift Forums](https://forums.swift.org/)

[Google's Swift Style Guide](https://google.github.io/swift/)

[Swift Courses Online from Coursera](https://www.coursera.org/courses?query=swift)

[Swift Courses Online from Udemy](https://www.udemy.com/topic/swift/)

[Learning Swift course from Codecademy](https://www.codecademy.com/learn/learn-swift)

## Swift Tools

[Xcode](https://developer.apple.com/xcode/) includes everything developers need to create great applications for Mac, iPhone, iPad, Apple TV, and Apple Watch. Xcode provides developers a unified workflow for user interface design, coding, testing, and debugging. Xcode 12 is built as an Universal app that runs 100% natively on Intel-based CPUs and Apple Silicon. It includes a unified macOS SDK that features all the frameworks, compilers, debuggers, and other tools you need to build apps that run natively on Apple Silicon and the Intel x86_64 CPU.

[SwiftUI](https://developer.apple.com/documentation/swiftui) is a user interface toolkit that provides views, controls, and layout structures for declaring your app's user interface. The SwiftUI framework provides event handlers for delivering taps, gestures, and other types of input to your application.

[UIKit](https://developer.apple.com/documentation/uikit) is a framework provides the required infrastructure for your iOS or tvOS apps. It provides the window and view architecture for implementing your interface, the event handling infrastructure for delivering Multi-Touch and other types of input to your app, and the main run loop needed to manage interactions among the user, the system, and your app.

[AppKit](https://developer.apple.com/documentation/appkit) is a graphical user interface toolkit that contains all the objects you need to implement the user interface for a macOS app such as windows, panels, buttons, menus, scrollers, and text fields, and it handles all the details for you as it efficiently draws on the screen, communicates with hardware devices and screen buffers, clears areas of the screen before drawing, and clips views.

[ARKit](https://developer.apple.com/augmented-reality/arkit/) is a set set of software development tools to enable developers to build augmented-reality apps for iOS developed by Apple. The latest version ARKit 3.5 takes advantage of the new LiDAR Scanner and depth sensing system on iPad Pro(2020) to support a new generation of AR apps that use Scene Geometry for enhanced scene understanding and object occlusion.

[RealityKit](https://developer.apple.com/documentation/realitykit) is a framework to implement high-performance 3D simulation and rendering with information provided by the ARKit framework to seamlessly integrate virtual objects into the real world.

[SceneKit](https://developer.apple.com/scenekit/) is a high-level 3D graphics framework that helps you create 3D animated scenes and effects in your iOS apps.

[Mac Catalyst](https://developer.apple.com/mac-catalyst/) is a set of Apple APIs that developers can use to rapidly port their iOS apps to [Apple Silicon M1 Chip](https://www.apple.com/mac/m1/) and take full advantage of the new capabilities on the new Apple hardware.

[Instruments](https://help.apple.com/instruments/mac/current/#/dev7b09c84f5) is a powerful and flexible performance-analysis and testing tool that’s part of the Xcode tool set. It’s designed to help you profile your iOS, watchOS, tvOS, and macOS apps, processes, and devices in order to better understand and optimize their behavior and performance.

[Cocoapods](https://cocoapods.org/) is a dependency manager for Swift and Objective-C used in Xcode projects by specifying the dependencies for your project in a simple text file. CocoaPods then recursively resolves dependencies between libraries, fetches source code for all dependencies, and creates and maintains an Xcode workspace to build your project. 

[AppCode](https://www.jetbrains.com/objc/) is constantly monitoring the quality of your code. It warns you of errors and smells and suggests quick-fixes to resolve them automatically. AppCode provides lots of code inspections for Objective-C, Swift, C/C++, and a number of code inspections for other supported languages.

[Vapor](https://github.com/vapor/vapor) is a web framework for Swift. It provides a beautifully expressive and easy to use foundation for your next website, API, or cloud project.

[Hero](https://github.com/HeroTransitions/Hero) is a library for building iOS view controller transitions. It provides a declarative layer on top of the UIKit's cumbersome transition APIs—making custom transitions an easy task for developers.

[Kingfisher](https://github.com/onevcat/Kingfisher) is a powerful, pure-Swift library for downloading and caching images from the web. It provides you a chance to use a pure-Swift way to work with remote images in your next app.

[Realm](https://github.com/realm/realm-cocoa) is a mobile database that runs directly inside phones, tablets or wearables. This repository holds the source code for the iOS, macOS, tvOS & watchOS versions of Realm Swift & Realm Objective-C.

[Perfect](https://github.com/PerfectlySoft/Perfect) is a complete and powerful toolbox, framework, and application server for Linux, iOS, and macOS (OS X). It provides everything a Swift engineer needs for developing lightweight, maintainable, and scalable apps and other REST services entirely in the Swift programming language for both client-facing and server-side applications.

[Alamofire](https://github.com/Alamofire/Alamofire) is an HTTP networking library written in Swift.

[Eureka](https://github.com/xmartlabs/Eureka) is an elegant iOS form builder in Swift 

[Carthage](https://github.com/Carthage/Carthage) is intended to be the simplest way to add frameworks to your Cocoa application. Carthage builds your dependencies and provides you with binary frameworks, but you retain full control over your project structure and setup. Carthage does not automatically modify your project files or your build settings.

[ReactiveCocoa](https://github.com/ReactiveCocoa/ReactiveCocoa) is reactive extensions to Cocoa frameworks, built on top of ReactiveSwift.

# XML Development
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/102813607-f8424e00-437d-11eb-81fa-27a83b4329d3.png">
  <br />
</p>

## XML Learning Resources

[XML(Extensible Markup Language)](https://www.w3.org/XML/) is a markup language that is similar to HTML but without predefined tags. Instead, the user define their own tags designed specifically for their needs. 

[XAML](https://docs.microsoft.com/en-us/dotnet/desktop/wpf/fundamentals/xaml) is a declarative XML-based markup language that is applied to the .NET Core programming model, which XAML simplifies creating a UI for a [.NET Core app](https://docs.microsoft.com/en-us/windows/uwp/xaml-platform/xaml-overview).

[Using XML editor in Visual Studio](https://docs.microsoft.com/en-us/visualstudio/xml-tools/xml-editor)

[XMLmind XML Editor Tutorial](https://www.xmlmind.com/xmleditor/tutorial.html)

[XMLReader for Android Developers](https://developer.android.com/reference/org/xml/sax/XMLReader)

[Adding app configuration policies for managed iOS/iPadOS devices](https://docs.microsoft.com/en-us/mem/intune/apps/app-configuration-policies-use-ios)

[XML Processing Modules for Python 3](https://docs.python.org/3/library/xml.html)

[PHP: XML Parser Manual](https://www.php.net/manual/en/book.xml.php)

[Introduction to XML on W3Schools](https://www.w3schools.com/xml/)

[Introduction to XML by IBM](https://www.ibm.com/developerworks/xml/tutorials/xmlintro/xmlintro.html)

[XML Fundamentals Training Program from Oracle University](https://education.oracle.com/xml-fundamentals/courP_1492)

[XML Online Training Courses on Udemy](https://www.udemy.com/topic/xml/)

[XML Schema (XSD) Crash Course for Beginners on Udemy](https://www.udemy.com/course/xml-schema-xsd-crash-course-for-beginners/)

[XML Online Training Courses on Coursera](https://www.coursera.org/search?query=XML&)

[XML Online Training Courses on LinkedIn Learning](https://www.linkedin.com/learning/topics/xml)

[Introduction to Microsoft Office Open XML on Pluralsight](https://www.pluralsight.com/courses/introduction-microsoft-office-open-xml)

[XML Fundamentals in C# on Pluralsight](https://www.pluralsight.com/courses/csharp-xml-fundamentals)

[Working with XML in Java Using JAXB](https://www.pluralsight.com/courses/xml-java-using-jaxb)

[Querying JSON, XML, and Temporal Data with T-SQL](https://www.pluralsight.com/courses/querying-json-xml-temporal-data-tsql)

[XML Training Courses on NobleProg](https://www.nobleprog.com/xml-training)

## XML Tools and Frameworks

[Visual Studio](https://visualstudio.microsoft.com/) is an integrated development environment (IDE) from Microsoft; which is a feature-rich application that can be used for many aspects of software development. Visual Studio makes it easy to edit, debug, build, and publish your app. By using Microsoft software development platforms such as Windows API, Windows Forms, Windows Presentation Foundation, and Windows Store.

[MSBuild](https://github.com/dotnet/msbuild) is the build platform for .NET and Visual Studio. MSBuild, provides an XML schema for a project file that controls how the build platform processes and builds software. Visual Studio uses MSBuild to perform team builds through Azure DevOps Server, but MSBuild can run without Visual Studio.

[WebStorm](https://www.jetbrains.com/webstorm/) is a professional IDE for JavaScript(including support for both HTML and CSS) developed by JetBrains. WebStorm comes with intelligent code completion, on-the-fly error detection, powerful navigation and refactoring for JavaScript, TypeScript, stylesheet languages, and all the most popular frameworks([Angular](https://angular.io/), [React](https://reactjs.org/), [Vue.js](https://vuejs.org/), [Ionic](https://ionicframework.com/), [Apache Cordova](https://cordova.apache.org/), [React Native](https://reactnative.dev/), [Node.js](https://nodejs.org/), [Meteor](https://www.meteor.com/#!), and [Electron](https://www.electronjs.org/)).

[Uno Platform](https://platform.uno/) is a Universal Windows Platform Bridge that allows UWP-based code (C# and XAML) to run on iOS, Android, macOS, WebAssembly, Linux and Windows. It provides the full definitions of the UWP [Windows 10 2004 (19041)](https://docs.microsoft.com/en-us/windows/uwp/whats-new/windows-10-build-19041), and the implementation of a growing number of parts of the UWP API, such as Windows.UI.Xaml, to enable UWP and WinUI applications to run on these platforms.

[Android Studio](https://developer.android.com/studio/) is the official integrated development environment for Google's Android operating system, built on JetBrains' IntelliJ IDEA software and designed specifically for Android development. Availble on Windows, macOS, Linux, Chrome OS.

[Oxygen XML Editor](https://www.oxygenxml.com/) is a cross platform tool setting the standard in XML editing. The advanced XML editor provides the most intuitive tools for XML editing, authoring, and development. It is availble on Windows, macOS, and Linux.

[XMLmind XML Editor](https://www.xmlmind.com/xmleditor/) is a strictly validating XML editor. It has Extensive DITA 1.3 support, and includes lightweight DITA, XDITA, HDITA, MDITA.

[Refit](https://github.com/reactiveui/refit) is the automatic type-safe REST library for .NET Core,.NET and Xamarin.

[Pugixml](https://github.com/zeux/pugixml) is a C++ XML processing library, which consists of a DOM-like interface with rich traversal/modification capabilities, an extremely fast XML parser which constructs the DOM tree from an XML file/buffer, and an XPath 1.0 implementation for complex data-driven tree queries. 

[Serializer](https://symfony.com/serializer) is a component that makes it easier to handle serializing data structures, including object graphs, into array structures or other formats like XML and JSON. It can also handle deserializing XML and JSON back to object graphs.

[Erlsom](https://github.com/willemdj/erlsom) is an XML parser for Erlang.

[REST-assured](https://github.com/rest-assured/rest-assured) is a Java DSL for easy testing of REST services.

## Contribute

- [x] If would you like to contribute to this guide simply make a [Pull Request](https://github.com/mikeroyal/Self-Hosting-Guide/pulls).


## License
[Back to the Top](https://github.com/mikeroyal/Self-Hosting-Guide#table-of-contents)

Distributed under the [Creative Commons Attribution 4.0 International (CC BY 4.0) Public License](https://creativecommons.org/licenses/by/4.0/).
