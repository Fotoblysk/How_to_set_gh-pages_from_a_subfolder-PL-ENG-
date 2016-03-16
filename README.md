# How_to_set_gh-pages_from_a_subfolder-PL-ENG-
Useful for documentation (e.g. doxygen output).


###TO_DO
- [ ] Push gh-pages branch
- [ ] Add introduction.
- [x] Add ENG description.
- [ ] Add PL description.
- [x] Add commands.
- [ ] Add summary.

#ENG
1. **Introduction**
2. **Steps**
  1. **Create repository on github.com with README.md**
  2. **Open terminal/Git_Shell**
  3. **Commands**
    - Clone repository to local
    - Make html directory
    - Go to html directory
    - Clone to current directory with . (dot flag)
    - Create gh-pages branch on repository in html directory
    - Change branch to gh-pages on repository in html directory
    - Remove master branch from repository in html directory
    - We are done :grin: , now we can create index.html and push changes to GitHub
3. **Summary**

```bash
#Clone repository to local
#\GitHub> 
git clone https://github.com/Fotoblysk/How_to_set_gh-pages_from_a_subfolder-PL-ENG-

cd .\How_to_set_gh-pages_from_a_subfolder-PL-ENG-

#Make html directory
  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG- [master]>
mkdir html

#Go to html directory
  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\ [master]>
cd .\html

#Clone to current directory with . (dot flag)
  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\html [master]>
git clone https://github.com/Fotoblysk/How_to_set_gh-pages_from_a_subfolder-PL-ENG- .

#Create gh-pages branch on repository in html directory
  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\html [master]>
git branch gh-pages

#Change branch to gh-pages on repository in html directory
  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\html [master]>
git checkout gh-pages

#Remove master branch from repository in html directory
  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\html [gh-pages]>
git branch -d master

#We are done :grin: , now we can create index.html and push changes to GitHub
  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\html [gh-pages]> 
.\README.md

  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\html [gh-pages]> 
mv .\README.md index.html

  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\html [gh-pages +1 ~0 -1 !]>
     #cat .\index.html
     # <!DOCTYPE html>
     #<html>
     #<head>
     #<meta charset="UTF-8">
     #<title>Example title</title>
     #</head>
     #
     #<body>
     #This is our gh-page :) .
     #</body>
     #
     #</html>

  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\html [gh-pages +1 ~0 -1 !]>
git add .

  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\html [gh-pages +1 ~0 -1]> 
git commit -m "add  gh-page"


  #\GitHub\How_to_set_gh-pages_from_a_subfolder-PL-ENG-\html [gh-pages]>
git push --set-upstream origin gh-pages

```
#PL
