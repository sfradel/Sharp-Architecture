#Contributing#

Any form of contribution is welcome, read below for different ways you can help.

Make sure to set AutoCRLF=true in your Git tool before cloning this repository. See [http://help.github.com/dealing-with-lineendings/](http://help.github.com/dealing-with-lineendings/) for more information.

##Documentation##

Documentation can be viewed on [docs.sharparchitecture.net](http://docs.sharparchitecture.net/) and gets generated from RST from the files in /Doc folder.

> An RST web editor can be found [here](http://rst.ninjs.org/)

If your changes require a change in the documentation (e.g. adding a feature or changing existing behaviour) then you will need to modfy documentation accordingly.
You can use the github webUI to do small changes like spelling mistakes and formatting. Feature or hotfix documentation changes should be included in the pull request.

##Bug reports and feature requsts##

- Ensure bug is reproducable with latest release.
- Look for existing github issue, create a new one if it doesn't exist.
- When reporting an issue, make sure you include:
  - What you did?
  - What happened?
  - What you expected to happen?

###New features###

Make sure to discuss new features on the [mailing first](http://groups.google.com/group/sharp-architecture "Sharp Architecture mailing list") before adding issues for them.

##Submitting code changes##

- Create [Github account](https://github.com/signup/free)
- [Setup git](https://help.github.com/articles/set-up-git)
- [Fork](https://help.github.com/articles/fork-a-repo "Fork") project
- Clone repostiory `git clone git@github.com:USER/Sharp-Architecture.git`
- Add upstream repository `git remote add upstream git@github.com:sharparchitecture/Sharp-Architecture.git`
- Initialize submodules

        git submodule init
        git submodule update
    
- S#arp Architecture uses Git-Flow branching model, read more about it [here](http://nvie.com/posts/a-successful-git-branching-model/ "git-flow") and follow [installation instructions](https://github.com/nvie/gitflow/wiki/Installation)
- Initialise git-glow `git flow init -d`
- Create new feature with `git flow feature start MEANINFUL_NAME`, for bug fixes create new branch with `git flow hotfix start VERSION_NUM` where VERSION_NUM is the current release version with the patch version incremented. For more information on versioning strategy, read up on [SemVer](http://semver.org/)
- Run Build/Build.bat to generate AssemblyInfo files required to build the solution.
- Make you changes, making sure your coding style and standards adhere to the code standards followed throughout the code, a [StyleCop](http://stylecop.codeplex.com/) rules file exists to highlight style problems.
- Run Build/BuildAndTest.bat to make sure all tests are still passing
- Update documentation
- Commit and push
- Open [pull request](https://help.github.com/articles/using-pull-requests) with the target branch being develop for features and master for hotfixes.
- Treat youself for whatever you fancy for a job well done.
