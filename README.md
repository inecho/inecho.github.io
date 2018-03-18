# inecho.github.io
Welcome to my gitpages doc..
## Initial steps
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
In order to check if a test page, created with AsciiDoctor, is suitable for GitPages, a `test.html` was pushed into the repo. Unfortunately the html page was not showing up as the main page while the README still got parsed. The solution was to rename `test.html` to `index.html`
> If the changes, made to the webpage, are applied, a delay of a minute needs to be considered to make an update visible

Commiting further changes made on the existing files, a handy push combo is:
```bash
git commit -am "update of existing files" && git push origin master
```
> Option -a stands for --all "commiting all changes files"

> Option -m stands for --message "commit message "
