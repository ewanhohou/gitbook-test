# Introduction

Git Book test

## Install

```
npm install -g gitbook-cli
```
## build

```
gitbook build
```

## Server

```
gitbook serve
```

## Publish
```
git checkout --orphan gh-pages

//clean
git rm --cached -r .
git clean -df

//gitignore _book
echo _book >> .gitignore
git add .gitignore
git commit -m "Ignore some files"

//copy
cp -r _book/* .
git add .
git commit -m "publish"

//push
git push -u origin gh-pages
```