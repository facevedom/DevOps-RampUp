# CI/CD

In a real development project, usually, there are a bunch of people working to create new features or change the existing ones, developers, testers, project managers, stakeholders, etc. All those people are always focused on creating a product with good quality and in the faster way they can. But once that product is created, what do we do with it? How do we deliver it to the final client in the fastest and reliable way can? How do we make sure the product we are releasing is not broken or contains bugs?

---

## CI

We will break the challenges in two parts, the first part will be about continuous integration and the second part about continuous deployment/delivery. In the first part you’ll design and setup your CI pipeline:

1. **Design and create a diagram of your continuous integration pipeline.** In this stage is very important to internalize the concepts and terminology of CI, so, focus on that instead of searching about tools. Also, don’t think about deployment yet, this will come in a later stage

2. **Research and choose an automation server.** There is a big list to choose from (Travis, Jenkins, CircleCI, Gitlab, Bamboo, etc). Again, feel free to choose whatever you like the most.

3. **Implement the pipeline you created in the tool you chose.** If you feel something is not right with your diagram, make the necessary adjustment.

---

## CD

Hopefully and the end of point 3 you will end up with a fully tested artifact ready to be deployed. Now it’s time to deploy your artifact in your infrastructure:

1. **Design and implement your deployment process.** Every application is different, so choose the right tools and process to deploy your application in your infrastructure.

2. **Choose the policies of when you are going to deploy.** For example, you may need to trigger the build process automatically in case there’s a change in a specific branch, or maybe someone needs to press a button, etc. Also, imagine you are part of an organization, who is allowed to deploy? How are you going to enforce that?
  
3. **Research and learn about deployment strategies** and choose one to implement your project.

4. **Implement your deployment solution.** Maybe you want to choose a tool provided by your cloud provider or a third party, or maybe you want to implement your own solution based on the tools you already know. Be creative here!
