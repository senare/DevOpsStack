
+++
title = "Ansible"
outputs = ["Reveal"]
+++

#### Ansible sales pitch

***Free*** Ansible is an open-source tool.

--- 

#### Ansible sales pitch

***Very simple to set up and use*** No special coding skills are necessary to use Ansible’s playbooks.

--- 

#### Ansible sales pitch

***Powerful*** Ansible lets you model even highly complex IT workflows.

--- 

#### Ansible sales pitch

***Flexible*** You can orchestrate the entire application environment no matter where it’s deployed. You can also customize it based on your needs.

--- 

#### Ansible sales pitch

***Agentless*** You don’t need to install any other software or firewall ports on the client systems you want to automate. You also don’t have to set up a separate management structure.


--- 

#### Ansible sales pitch

***Efficient*** Because you don’t need to install any extra software, there’s more room for application resources on your server.

---

#### What can ansible do 

***Configuration Management*** Ansible is designed to be very simple, reliable. Ansible configurations are simple data descriptions of infrastructure and are both readable by humans and parsable by machines. 

---

#### What can ansible do

***Application Deployment*** Ansible lets you quickly and easily deploy multitier apps. You won’t need to write custom code to automate your systems; you list the tasks required to be done by writing a playbook, and Ansible will figure out how to get your systems to the state you want them to be in.

---

#### What can ansible do

***Orchestration*** Bringing different elements into a cohesive whole. For example, with application deployment, you need to manage not just the front-end and backend services but the databases, networks, storage, and so on. You also need to make sure that all the tasks are handled in the proper order. Ansible uses automated workflows, provisioning, and more to make orchestrating tasks easy.

---

#### What can ansible do

***Security and Compliance*** As with application deployment, sitewide security policies (such as firewall rules or locking down users) can be implemented along with other automated processes. If you configure the security details on the control machine and run the associated playbook, all the remote hosts will automatically be updated with those details. That means you won’t need to monitor each machine for security compliance continually manually. And for extra security, an admin’s user ID and password aren’t retrievable in plain text on Ansible.

---

#### What can ansible do

***Cloud Provisioning*** The first step in automating your applications’ life cycle is automating the provisioning of your infrastructure. With Ansible, you can provision cloud platforms, virtualized hosts, network devices, and bare-metal servers.

---

#### Ansible Architecture

***Modules*** Modules are like small programs that Ansible pushes out from a control machine to all the nodes or remote hosts. The modules are executed using playbooks (see below), and they control things such as services, packages, and files. Ansible executes all the modules for installing updates or whatever the required task is, and then removes them when finished. Ansible provides more than 450 modules for everyday tasks.

---

#### Ansible Architecture

***Plugins*** As you probably already know from many other tools and platforms, plugins are extra pieces of code that augment functionality. Ansible comes with a number of its plugins, but you can write your own as well. Action, cache, and callback plugins are three examples.

---

#### Ansible Architecture

***Inventories*** All the machines you’re using with Ansible (the control machine plus nodes) are listed in a single simple file, along with their IP addresses, databases, servers, and so on. Once you register the inventory, you can assign variables to any of the hosts using a simple text file. You can also pull inventory from sources like EC2 (Amazon Elastic Compute Cloud).

---

#### Ansible Architecture

***Playbooks*** Ansible playbooks are like instruction manuals for tasks. They are simple files written in YAML, which stands for YAML Ain’t Markup Language, a human-readable data serialization language. Playbooks are really at the heart of what makes Ansible so popular is because they describe the tasks to be done quickly and without the need for the user to know or remember any particular syntax. Not only can they declare configurations, but they can orchestrate the steps of any manually ordered task, and can execute tasks at the same time or at different times.

Each playbook is composed of one or multiple plays, and the goal of a play is to map a group of hosts to well-defined roles, represented by tasks.

---

#### Ansible Architecture

***APIs*** Various APIs are available so you can extend Ansible’s connection types (meaning more than just SSH for transport), callbacks and more.

---

[![Redhat](/senare/images/redhat.svg)](https://www.ansible.com/)

---

#### What is Ansible Tower?
Ansible Tower is Red Hat’s commercial web-based solution for managing Ansible. Its best-known feature is an easy-to-use UI (user interface) for managing configurations and deployments, which is a significant improvement over the original UI. Ansible Tower contains the essential features of Ansible, especially those that are easier to see in a graphical format rather than a text-based format.

---

# Ansible doc's

[Documentation]({{% ref "https://docs.ansible.com/" %}})

---

# End

[return]({{% relref "/#" %}})


