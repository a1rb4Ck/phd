# How to convert from tex to html

```bash
pdf2htmlEX --embed cfij --dest-dir web Manuscrit.pdf
```

Then rename to `Manuscrit.html` to `index.html`.


# Using Git Worktree to Deploy GitHub Pages

From [sangsoonam](https://sangsoonam.github.io/2019/02/08/using-git-worktree-to-deploy-github-pages.html).

```branch
git branch gh-pages

git checkout --orphan gh-pages
git reset --hard
git commit --allow-empty -m "Init"
git checkout master
git worktree add web gh-pages
echo "web" >> .gitignore

git branch

cd web
git branch

# Deploy
cd web
git add --all
git commit -m "Deploy updates"
git push origin gh-pages

# To unmount the subdirectory
# git worktree remove _site
```
