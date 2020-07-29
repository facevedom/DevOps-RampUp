# Basic concepts to deploy an application 

Now that you understand the basics of how GNU/Linux works, it’s time to start playing with the application. The first thing we need to understand is how to convert the application code into something that you can use and install on a system.

---
To complete this challenge, you are required to:

1. **Create a GNU/Linux virtual machine.** The decision of what distro to use is up to you. For applications with a multitier architecture (e.g., applications where presentation (frontend), processing (backend), and data management (database, cache server, etc), are separated services), you can also choose whether to create one VM for all services or one for each service. If you have a little bit of knowledge on any cloud provider and want to save the time to install and configure a VM, you can also set up an instance there, but keep in mind that it will cost more money.

    **Bonus points:** Use Vagrant to set up your VMs. It will serve the purpose of introducing you to the `* as code` principle, which will become very important in this RampUp and your professional career.

2. **Install everything you need to run the application.** The application may require some software to be installed in the system to run properly (e.g., to run a Java server application, you will need JRE and an application server such as Tomcat), or maybe you need to run a database system or configure some environment variables.

3. **Run the application with best practices.** There are many ways to run an application, some of them better suited for testing environments, others for production.  Find what are the best practices to do for a **production environment**. Maybe you need to configure an NGINX server, or use Tomcat, etc. Find what works best for the application you have. Keep in mind what happens if you restart your machine, do you need to start the service manually again or it happens automatically? On which port are you going to expose the application? And remember, everything you do must be done on a terminal! We want you to learn how things work on the inside.

**Note:** Write down every step or command you execute. You’ll need that later in this RampUp.
