# Scripting

One of the most important principles on the DevOps culture is automation (look up what `CAMS` means 😊). Your goal should be automating *almost* everything. Every time you make a manual task you need to ask yourself, “What do I need to do if I don’t want to do this again”. And to automate we need to know how to code, at least, in one programming language.

---
It’s time to automate everything you did on the first challenge. For this challenge you will be required to:

1. **Choose one (or several) programming language(s).** You are free to choose the language you like, but also keep in mind there are some languages that are preferred in the Sysadmin world (for example, Emojicode might not be a good choice). There’s no need to stick to a single language, you can use as many as you want. (if you want suggestions, Python has a small learning curve and great scripting capabilities, and Go will give you more powerful features).

2. **Create one (or several) script(s) to automate the provisioning for the VM’s that you created.** The most important requirement is that for a new fresh VM with nothing else installed, the execution of that script must install and configure everything necessary to run the application. After the script finishes its execution, the application and all its dependencies must be up and running.  

    **Note:** There’s an alternative to this which we will work on the configuration management challenge.  

3. **Try to make your scripts as idempotent (term to keep in mind) as you can**, that way it doesn’t matter how many times you execute the script, it will only do the necessary steps and nothing more.


4. **Use a VCS for all the code you write.** We will talk more about this later in this RampUp. (refer to SCM)


## Recommended readings

* https://medium.com/@brunodelb/the-cams-model-to-better-understand-the-devops-movement-ffe6713c3fd7
