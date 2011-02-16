HEllo git asdfasdf 1234 qwer asdfasdf 
asdf

git filter-branch --env-filter \
    'if [ $GIT_COMMIT = 3c88e45aea7c444a020e66ff5362da9e4a06dae7 ]
     then
         export GIT_AUTHOR_DATE="Fri Jan 2 21:38:53 2009 -0800"
         export GIT_COMMITTER_DATE="Sat May 19 01:01:01 2007 -0700"
     fi'