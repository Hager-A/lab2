GI ensure that the repository is not currently on the branch to be deleted
1-delete branch locally
git branch -d branch-to-delete
2-delete branch remotely
git push remote-name --delete branch-to-delete
annotated tags vs lightweights tags
Description: Annotated tags are full objects in Git's database. They contain metadata such as the tagger's name, email, date, and a message.
Creation Command: Created using git tag -a <tagname> -m "message".
Use Case: Ideal for marking release points because they provide additional context.
Storage: Stored as full objects in the repository, which makes them more robust.
Verification: Can be signed with GPG for verification, enhancing security.
git tag -a v1.0 -m "Release version 1.0"
Description: Lightweight tags are simply pointers to a specific commit. They do not contain any additional metadata.
Creation Command: Created using git tag <tagname>.
Use Case: Useful for quick, informal tagging when no additional information is needed.
Storage: Stored as just a reference to a commit; they are not full objects.
git tag v1.0
when to use rebase:
Keeping Feature Branches Updated:
git checkout feature-branch
git rebase main


git tag v1.0
when to use rebase:
how to list tags:
git tag
Delete a Local Tag: git tag -d tagname
Delete a remote Tag: git push --delete remote-name tagname
