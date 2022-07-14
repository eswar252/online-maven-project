git clone git@github.com:eswar252/online-maven-project.git
ls -lrth
cd online-maven-project/
touch sample1.txt
vi sample1.txt
git add .
git status
cat sample1.txt
git commit -m "sample1 file added"
git status
ls -lrth
git push git@github.com:eswar252/online-maven-project.git master
