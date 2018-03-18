# inecho.github.io
The first steps of publishing the website were:
```bash
mkdir -p gitpages #in order to create a seperate folder
echo '# inecho.github.io' >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:inecho/inecho.github.io.git
git push -u origin master
```
The result is just a headline parsed from the `README.md`.
In order to check if a testpage, created with AsciiDoctor, is suitable for GitPages a `test.html` was pushed onto the repo. Unfortunately this page was not displayed while the README still got parsed. The solution was to rename `test.html` to `index.html`
>> If the changes made to the webpage are applied, a delay of a minute need to be considered to make an update visible
