Testing git lfs support in different hosting alternatives:

* Assembla
* Github
* Azure DevOps

Overall the pipeline to checkout a blank repository and re-upload is:
  $ git clone URL-OF-REPOSITORY FOLDER
  $ cd FOLDER
  $ git lfs install
  $ git lfs fetch #This gets all the objects, not only the HEAD
  $ git remote add new-repo URL-OF-NEW-REPOSITORY
  $ git push rew-repo master
