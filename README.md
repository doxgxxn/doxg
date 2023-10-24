# distribution for the first time

### describe: my first python package uploaded on https://pypi.org/ and uploaded on github for distribution
### PYPI에 package를 업로드하고 깃허브와 연동하여 배포


---

View at:
https://pypi.org/project/doxg

INSTALL

    $ pip install doxg
  
DEV

    $ git clone ...
    $ cd doxg
    $ pdm .venv create
    $ source .venv/bin/activate
    (doxg-3.8) $ pdm install
    
DEPLOY

    $ pdm publish
    
Contributing

    $ git branch 0.2.0/doxg
    
    $ git switch 0.2.0/doxg
    Switched to branch '0.2.0/doxg'
    
    $ vi pyproject.toml
    
    $ git status
    On branch 0.2.0/doxg
    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git restore <file>..." to discard changes in working directory)
            modified:   pyproject.toml
    
    no changes added to commit (use "git add" and/or "git commit -a")
    
    $ git add .
    
    $ git status
    On branch 0.2.0/doxg
    Changes to be committed:
      (use "git restore --staged <file>..." to unstage)
            modified:   pyproject.toml
    
    $ git commit -m "start dev 0.2.0"
    [0.2.0/doxg 4ed0751] start dev 0.2.0
     1 file changed, 1 insertion(+), 1 deletion(-)
     
    $ git push
    fatal: The current branch 0.2.0/doxg has no upstream branch.
    To push the current branch and set the remote as upstream, use
    
        git push --set-upstream origin 0.2.0/doxg
    
    $ git push --set-upstream origin 0.2.0/doxg
