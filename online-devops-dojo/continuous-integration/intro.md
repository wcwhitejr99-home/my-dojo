## Welcome

Welcome to the **Unicorn Online DevOps Dojo** lab on 

## Continuous Integration  

## In The Past

![Dan](../../assets/online-devops-dojo/continuous-integration/dan.png) **In the past**, Dan the developer and his peers on the team, worked away developing business features on separate branches for up to weeks at a time.  When the feature was complete they would commit their work to the central source code management system.  
Typically this was followed by 1 to 2 days of integration as the release manager was gathering and merging the changes from all the team members.  
This was taking time and involved a lot of rework, merge conflicts (which took time to be resolve), and often resulted in unplanned activities.  
To be able to produce deployable packages out of the code, they had to have a "code freeze" phase until a working build could be sent to QA/Testing.  

---

![Tina](../../assets/online-devops-dojo/continuous-integration/tina.png)  Testing led by Tina would then proceed.  They would identify issues, with the development team having to fix the bugs before they could release the application to the business.  

---

## Today

Dan's team now applies the principle of working in small batches and building quality with continuous integration supported by a high degree of automated testing.  All the developers are now continuously integrating to trunk (master branch). They use short lived (one to several days) feature branches which are quickly merged to master. Each and every commit triggers the continuous integration pipeline automatically, which builds the code and runs automated tests created by Tina and the testing team.  
The pass/fail results are made available as part of the feature branch / pull request, thus detecting regressions automatically, as well as providing accurate feedback to the development team.  
Dan (or the lead reviewing the pull request) will not merge the request to master if any of the checks run from the continuous integration pipeline are not passing.  

This is **Continuous Integration** and it is proven to be a game changer for the software industry.  
