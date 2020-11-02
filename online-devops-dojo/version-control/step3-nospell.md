## Understanding the user story

![Paulo](../../assets/online-devops-dojo/version-control/paulo.png)  

> **Paulo:** I created a user story, and it is visible in our backlog. We want to link the code changes to that user story, so that we can ensure traceability and make work visible.  

### Steps

- Go and check the pet clinic backlog (check the terminal window for a link to the issues module in your pet-clinic repository).  
- The backlog is being maintained as "Issues" in GitHub.  You should see an issue: Support veterinarians who handle horses #1  
- Identify the user story number (should be `1`)  

---

## Create a feature branch  

![Dan](../../assets/online-devops-dojo/version-control/dan.png)  

> **Dan:** To make sure we isolate the separate work being done on the various stories, we use feature branches. We name this short lived branch after the ID and name of the user story.  This helps everyone identify the work being done for each story.

### Steps  

- Change directory into the cloned repo: `cd pet-clinic`{{execute}}  
- Create `us-1-horse` branch to cover user story 1 about adding horses: `git checkout -b us-1-horse`{{execute}}  
> note:  branch naming convention - `us` is User Story - `1` is the story number - `horse` briefly describes the story.  

![Dan](../../assets/online-devops-dojo/version-control/dan.png)  

> This branch is a short lived feature branch. We use this feature branch to get feedback from continuous integration (automated checks and gates) and from peers and stakeholders. This allows us to work in isolation (without impacting others), yet sharing the work in progress.  

---

## Make changes  

![Dan](../../assets/online-devops-dojo/version-control/dan.png)  

> Now, let's implement the user story by making some changes in the code. We will first start by adding `horse` as a pet type.  

### Steps  

- In the editor to the right, navigate to `src/main/resources/db/hsqldb` folder and  open `data.sql`  
- In the data, below `INSERT INTO types VALUES (6, 'hamster');` (around line 23), add a new line to insert the horse entry: `INSERT INTO types VALUES (7, 'horse');`{{copy}}  

> Note that your changes are saved automatically.  

- Check the branch in which you are working: `git branch`{{execute}}  
- Check the status of the file changed: `git status`{{execute}}  

![Dan](../../assets/online-devops-dojo/version-control/dan.png)  

> Good! I can see that you are working in the context of the feature branch and that the file has changed and is ready to be added: Git reports that changes are not staged for commit yet.  
