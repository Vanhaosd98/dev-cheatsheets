## What is CI/CD?
<description>
CI/CD stands for Continuous Integration and Continuous Delivery (or Deployment). Continuous Integration is the practice of frequently merging code changes into a shared repository. It involves automating the build, unit testing, and code quality checks to detect issues early. Continuous Delivery focuses on automating the deployment process to make software releases ready for production at any time.
</description>

<description>

![jenkin1](../public/jenkin/jenkin1.avif)

</description>

## What Is a Build Job?
<description>
A Jenkins build job contains the configuration for automating a specific task or step in the application building process. These tasks include gathering dependencies, compiling, archiving, or transforming code, and testing and deploying code in different environments.

Jenkins supports several types of build jobs, such as freestyle projects, pipelines, multi-configuration projects, folders, multibranch pipelines, and organization folders.

What is Freestyle Projects ??
A Freestyle Project in Jenkins allows you to create a job without adhering to a strict pipeline structure. It provides a graphical user interface (GUI) where you can configure various build steps, triggers, post-build actions, and more. This approach is especially useful for projects that don't follow a standard build and deployment process or for teams that prefer a more manual and ad-hoc approach to setting up their automation tasks.
<description>

### Task-01
<summary>
create a agent for your app. which you deployed from docker in earlier task

#### 1.In your Jenkins instance, go to "Manage Jenkins" > "Nodes".

![jenkin2](../public/jenkin/jenkin2.avif)

#### 2.Click on "New Node" or "New Agent" to create a new agent.

![jenkin3](../public/jenkin/jenkin3.avif)

#### 3.Provide a name for the agent and select "Permanent Agent".

![jenkin4](../public/jenkin/jenkin4.avif)

#### 4.Configure the agent settings, such as the number of executors and remote root directory.

![jenkin5](../public/jenkin/jenkin5.avif)

#### 5.Optionally, configure labels to associate with this agent and select "Use WebSocket" Save the configuration.

![jenkin6](../public/jenkin/jenkin6.avif)

#### 6.the agent is created.

![jenkin7](../public/jenkin/jenkin7.avif)

### Create a new Jenkins freestyle project for your app.

#### 1.From the Jenkins dashboard, click on "New Item" to create a new project.

![jenkin8](../public/jenkin/jenkin8.avif)

#### 2.Enter a project name and select "Freestyle project" Click "OK" to create the project.

![jenkin9](../public/jenkin/jenkin9.avif)

### In the "Build" section of the project, add a build step to run the "docker build" command to build the image for the container.

#### 1.In the project configuration, navigate to the "Build" section.

![jenkin10](../public/jenkin/jenkin10.avif)

#### 2.Click on "Add build step" and select "Execute shell" (or the relevant option for your environment).

![jenkin11](../public/jenkin/jenkin11.avif)

#### 3.In the "Execute shell" build step, add the command to build the Docker image for your app. Replace with the actual directory of your app

![jenkin12](../public/jenkin/jenkin12.avif)

#### 4.Save the project configuration.

![jenkin13](../public/jenkin/jenkin13.avif)

</summary>