|       |                           | main == feature OR feature --> main | main --> feature | root --> main<br>        \\--> feature |
| ----- | :-----------------------: | :---------------------------------: | :--------------: | -------------------------------------- |
| main* |     git merge feature     |         Already up to date.         |   Fast forward   | 3-way merge                            |
| main* |    git rebase feature     |         Already up to date.         |   Fast forward   | root --> feature --> delta-of-main     |
|       | git branch -f main HEAD~3 |                                     |                  |                                        |
|       |                           |                                     |                  |                                        |