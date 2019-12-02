HEllo git asdfasdf 1234 qwer asdfasdf 
asdf

git filter-branch --env-filter \
    'if [ $GIT_COMMIT = ccca83e3aab02ebd0f4510bd2c54ddc7b7cb4bdc ]
     then
         export GIT_AUTHOR_DATE="Mon Dec 2 21:38:53 2019 -0800"
         export GIT_COMMITTER_DATE="Mon Dec 2 21:38:53 2010 -0800"
     fi'

GIT_COMMITTER_DATE="Mon Dec 2 18:00 2019" git commit --amend --date "Mon Dec 2 18:00 2019"
