# Conventional Commits

## This repo demonstrates..
* The use of Conventional Commits to improve readability for your commit messages, and to make automations based on them. See the commits for examples
* Commitzen, a tool for git bash that helps you write conventional commit messages
* Standard version, a tool that uses conventional commits for automatically:
    * Increase the version of your app
    * Create a github release
    * Create a CHANGELOG.md file in your repo that contains a list all features and fixes

##  How i made this repo: TLDR

#### Create an empty repo
* Add a .gitignore-file (see ours)

#### Add commitizen
* Added a basic package.json file to hold the version
    * ` { "name": "conventionalcommits", "version": "0.0.0" }`
* Installed commitizen globally by running
    * `npm install -g commitizen`
* Enabled commitizen in the repo by running:
    * `commitizen init cz-conventional-changelog --save-dev --save-exact`


#### Automatically generate release and release notes when changes are made to main branch
See the .github/workflows/release.yml file for a github action that uses standard-version to bump the version, create a release and release notes


## Sources
* [Practice: Conventional commits](<https://www.conventionalcommits.org/en/v1.0.0/>)
* [Tool: commitizen](<https://github.com/commitizen/cz-cli>)
* [Tool: standard-version](<https://www.npmjs.com/package/standard-version>)
* [Practice: Semantic versioning](<https://semver.org/>)





