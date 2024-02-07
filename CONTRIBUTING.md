# Contributing

Thank you for investing your time and effort into contributing to this project! Every little bit
helps, and credit will always be given. 

In this guide, you will get an overview of the contribution workflow:  
1. Setting up your development environment
2. Locally building the book and viewing the rendered HTML
3. Creating a PR (pull request)
4. Reviewing
5. Merging the PR (pull request)

## Getting Started

### Using Conda

Clone the repository.
```
git clone git@github.com:dna-witch/algorithms-wiki.git
```
From the command line, create a new Conda virtual environment with Python installed:
```
conda create -n <yourEnvironmentName> python
conda activate <yourEnvironmentName>
```
*The following steps should be performed inside the activated Conda virtual environment!*

Install required packages and modules to build the book:
```
pip install -r requirements.txt
```

Set the git remote repository.
```
git init
git remote add origin git@github.com:dna-witch/algorithms-wiki.git
```

## Creating Your Changes

Please do not edit and push files directly to the main branch. Create a branch for local development and make changes locally. Push your commits, then start a Pull Request for your changes. 

```
git checkout <yourLocalDevBranch>  # Git will create the branch if it does not already exist.
```

(Optional) Edit the books source files located in the `algo_book/` directory

## Build locally and review changes
1. Run `jupyter-book clean algo_book/` to remove any existing builds
2. Run `jupyter-book build algo_book/` to locally view the HTML

*Helpful Resources*: 
* [Supported file types for Jupyter Book Content](https://jupyterbook.org/en/stable/file-types/index.html)
* [Markdown Guide](https://markdownguide.offshoot.io/)

## Submitting Your Changes

1. Commit your changes and push your branch to GitHub.
```
git add .
git commit -m "short description of your changes"
git push origin <yourLocalDevBranch>
```
2. Submit a pull request through the GitHub website.
*Helpful Resource*: [Collaborating with Pull Requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests)

3. PRs can be reviewed and merged through the GitHub website.

## Additional Info

#### Report Bugs
Report bugs using GitHub issues.
If you are reporting a bug, please include:

* Your operating system name and version.
* Any details about your local setup that might be helpful in troubleshooting.
* Detailed steps to reproduce the bug.

## Code of Conduct

Please note that the Intro to Algorithms project is released with a [Contributor Code of Conduct](CONDUCT.md). By contributing to this project you agree to abide by its terms.
