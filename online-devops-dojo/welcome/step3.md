
The **Unicorn Online DevOps Dojo** has been designed to ensure that as you progress through each module in the curriculum, you will be using your own dedicated copy of the "Pet Clinic" application.  

As you work through the labs, your progress will be saved to your own copy of the Pet Clinic Git repository. You can consider this copy a sandbox, where you can learn, evaluate, and try things out -  hopefully having some fun, safe in the knowledge that you can't impact any other learners.  

However, with great power comes great responsibility. There is a process we need you to follow to set up your environment. The setup process is, in itself, a learning opportunity - that of learning about GitHub repositories.  

---

### Creat a HitHub Account  

You need to have a GitHub account before you continue.  If you already have a GitHub account, you can skip this step.  If not, please follow the instructions below.  

1. Create a personal [github.com](https://github.com) account (Sign Up)  
1. Log in to [github.com](https://github.com)  

---  

### Generate Personal Access Token  

1. On any GitHub page (after you log on), click your profile icon at the top right and then click Settings.  
1. On the sidebar menu, click Developer settings and then click Personal access tokens.  
1. Click Generate new token.  
1. Enter a Token description of your choice. example: `unicorn-dojo-token`  
1. Select `repo` so that the token can read/write in your repository and `admin:repo_hook` so that it can update GitHub repository web hooks. **Make sure to select everything within those scopes.**
1. Click Generate token.
1. Click the clipboard icon to copy the token in your clipboard.
1. **Make note of the personal access token**. This token will be used throughout the Unicorn Online DevOps Dojo. Note that it is OK if you lose it, as you can always generate a new one.

---

### Copy the Pet Clinic application  

In order to isolate yourself from the original pet clinic repository, we will create a disconnected copy of the repository under your GitHub user account.  

* Run the following script to copy the Pet Clinic repository.  
(just click on the text below and the command will be run into the Katacoda window - there's no need to copy/paste or type it out yourself; though you might find that manually typing the commands helps build familiarity [and refine troubleshooting skills when you make typos])  

  `./copy-pet-clinic.sh`{{execute}}  

The script will ask you for your github.com Personal Access Token that you created earlier.   

Once the script has completed, you will see: `You are all set! Click on 'CONTINUE'.`  
Click CONTINUE.

---

<div style="text-align: left">💡 **NOTE**:  Usually, when you want to make a copy of a GitHub repository for you to edit, you use the **Fork** function. Forking is the process of making a copy of a Git repository into another account (in this case your account) so that you can add, edit or delete the content in your copy of the repository without impacting any users of the source repository. Meanwhile, your copy of the repository maintains a relationship back to the source repository, so that changes can be pushed "upstream" using the **Pull Request** function. </div>  

---


💡 **TIP**: 🦊 Firefox user? Use <kbd>CTRL</kbd>+<kbd>INS</kbd> / <kbd>SHIFT</kbd>+<kbd>INS</kbd> to copy/paste your Personal Access Token in the window.
