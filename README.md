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

git rm --cached -r .

git clean -df

cp -r _book/* .

git add .

git commit -m "publish"

git push -u origin gh-pages
```