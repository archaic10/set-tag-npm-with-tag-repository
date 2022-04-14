# Set tag npm with tag repository

### Description
This action looks for the recently released version of the repository tag and checks if it meets the following:

- v1.0.0.1
- v1.0.0
- 1.0.0.1
- 1.0.0

This action too changes the package.json file version of the specified branch, if no branch is specified it will change the default branch file

### Example 

```yml
uses: archaic10/set-tag-npm-with-tag-repository@main
with:
    github-token: ${{ secrets.GITHUB_TOKEN }}
    branch: development
    path: '/src'
```
### Or

```yml
uses: archaic10/set-tag-npm-with-tag-repository@main
with:
    github-token: ${{ secrets.GITHUB_TOKEN }}
    path: '/src'
```
## Or
```yml
uses: archaic10/set-tag-npm-with-tag-repository@main
with:
    github-token: ${{ secrets.GITHUB_TOKEN }}
    branch: development
```
### Or

```yml
uses: archaic10/set-tag-npm-with-tag-repository@main
with:
    github-token: ${{ secrets.GITHUB_TOKEN }}
```