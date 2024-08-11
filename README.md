# ci-testing

```
on push branch different from main:
  - test

create branch add_version:
  - echo "1.2.3" > version.txt
 2017  git add . && git commit -m "new feat testing" && git push
 2018  git push --set-upstream origin temp_branch_for_tagging
 
 
 on merge to master
 git switch main
 git merge temp_branch_for_tagging
 git push
 git tag 1.2.3
 git push origin 1.2.3
```
 


 ``` mermaid
    flowchart LR
    A[on git push\nget last version] --> B[get last version]


  ```