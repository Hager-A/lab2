GI ensure that the repository is not currently on the branch to be deleted
<br>
1-delete branch locally
<br>
git branch -d branch-to-delete
<br>
2-delete branch remotely
<br>
git push remote-name --delete branch-to-delete
<br>
annotated tags vs lightweights tags
<br>
Description: Annotated tags are full objects in Git's database. They contain metadata such as the tagger's name, email, date, and a message.
<br>
Creation Command: Created using git tag -a <tagname> -m "message".
<br>
Use Case: Ideal for marking release points because they provide additional context.
<br>
Storage: Stored as full objects in the repository, which makes them more robust.
<br>
Verification: Can be signed with GPG for verification, enhancing security.
<br>
git tag -a v1.0 -m "Release version 1.0"
<br>
Description: Lightweight tags are simply pointers to a specific commit. They do not contain any additional metadata.
<br>
Creation Command: Created using git tag <tagname>.
<br>
Use Case: Useful for quick, informal tagging when no additional information is needed.
<br>
Storage: Stored as just a reference to a commit; they are not full objects.
<br>
git tag v1.0
<br>
when to use rebase:
<br>
Keeping Feature Branches Updated:
<br>
git checkout feature-branch
<br>
git rebase main
<br>


git tag v1.0
<br>
when to use rebase:
<br>
how to list tags:
<br>
git tag
<br>
Delete a Local Tag: git tag -d tagname
<br>
Delete a remote Tag: git push --delete remote-name tagname
<br>




![Purple Flower](https://wallpapercave.com/wp/PSpoeP1.jpg)
