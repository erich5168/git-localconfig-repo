# git-localconfig-repo

:key: Project dependent on this porject
* [limits-service](https://github.com/erich5168/edu.spring-cloud-docker/tree/main/03.microservices/limits-service)
* [spring-cloud-config-server](https://github.com/erich5168/edu.spring-cloud-docker/tree/main/03.microservices/spring-cloud-config-server)


## Simple steps creating local git repo

```
mkdir repo && cd repo
# Create local git repo
git init
# Display files not beed added to repo
git status

```

**Add and Commit file**
```
git add .
git commit -m "initial commit"
```

```
# Add remote url (github url)
git remote add origin <REMOTE_URL>
# Verifies the new remote URL
git remote -v
```

**Optional**
```
git show-ref

```
> Due to the recent "Replacing master with main in GitHub" action, you may notice that there is a `refs/heads/main`. As a result, the following command may change from git push origin `HEAD:master` to git push origin `HEAD:main`

```
❯ git show-ref                                                               ─╯
2bd4957242af34e01d8f35d82932fd65b367df2c refs/heads/master
2bd4957242af34e01d8f35d82932fd65b367df2c refs/remotes/origin/master
```

[**stackoverflow solution:** -> error: src refspec master does not match any.]('https://stackoverflow.com/a/4183856/2159680')


**Push to GitHub**
```
# 
$ git push -u origin main
# or 
$ git push -u origin master    <- if git show-ref returns head/master

```
***Resources of GIT***
[**stackoverflow solution:** -> error: src refspec master does not match any.]('https://stackoverflow.com/a/7572252/2159680')

[Git using command line ]('https://docs.github.com/en/github/importing-your-projects-to-github/importing-source-code-to-github/adding-an-existing-project-to-github-using-the-command-line')