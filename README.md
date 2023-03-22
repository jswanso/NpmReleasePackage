# NPM Release Package

This project is to test out publishing an NPM package to GitHub.

This sample was taken from [Quickstart for GitHub Packages](https://docs.github.com/en/packages/quickstart).

## Used Windows Commands

As part of the quickstart guide I had to use some additional commands instead of creating things from hand.

### .npmrc File Creation

Commands to create the .npmrc file

`npm config set @jswanso:registry=https://npm.pkg.github.com`

`mv C:\Users\<User Name>\.npmrc .npmrc`

## To Publish Locally

To publish locally the .npmrc file needed to be updated to add credentials.

`//npm.pkg.github.com/:_authToken=<Person Access Token>`

Then you can run `npm publish` from within this project and it will publish the package.

You might also want to increment the version. This can be done with a command similar to the following:

`npm version 0.0.7-alpha`

This will update the version in the package.json file and the package-lock.json file. It also will check in the files and create an annotated tag with the following value `v0.0.7-alpha`.

## Resources

The following video helped clarify some of the settings.

[How to use the GitHub Package Registry](https://www.youtube.com/watch?v=2-77KhGWlRg)
