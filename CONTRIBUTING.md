# Contributing

If you're reading this, you're awesome! Thank you for helping us make this project great!Here are a few guidelines that will help you along the way.

## Submitting a Pull Request

Neptune is an open project with a large community(at least we hope), o any pull request is always welcome, but if you want to do big changes to the code, the best thing is to open a first issue and talk to us about those changes.
Make a different bundle the project and make a pull request for every bug you resolve!

When adding new features or modifying existing, please attempt to include tests to confirm the new behaviour.

When migrating a component to master, or submitting a new component, please add it to the alpha package.

## Branch Structure

All stable releases are tagged. Master isthe main branch with the latest stable release and stable "alpha" components and fixes.

Patches and hotfix and pull request are pushed to an indipendent branch and after in the `alpha` branch before getting released to `master`.
Follow the master flow to get your app safe and updated.

## Contributing Flow

1.  Fork the master or alpha(ifyou work with us).
2.  Clone the forked repo to your local machine
3.  Create a branch `git checkout -b my-topic-branch`
4.  Make your changes, lint, then push to to GitHub with `git push --set-upstream origin my-topic-branch` **(use prettier to make your code style better and similar to ours )**
5.  Make the pull request

If you have an existing local repository, please update it before you start, to minimise the chance of merge conflicts.

git remote add upstream git@github.com:knifesec/neptune.git
git checkout master
git pull upstream master
git checkout -b my-topic-branch
yarn

And this is all now your are active part to the neptune theme and community!!!!!!:tada::tada::tada::tada::tada::tada::tada:
