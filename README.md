# Bioinformatics help wanted: find open source repos seeking contributions

## Overview

The Jupyter notebook `bioinformatics-help-wanted.ipynb` searches the GitHub API for repositories matching search terms, and for open issues within those repositories matching an issue label. For example, use this code to find a list of all repositories matching the search term "bioinformatics", written in languages of your choice, with issues labeled "help wanted".

## Usage

#### Installing requirements
`pip install -r requirements.txt`

#### GitHub credentials
A GitHub account and associated OAuth token are required to run this notebook. See these [instructions](https://help.github.com/en/articles/creating-a-personal-access-token-for-the-command-line) to create a token.

#### GitHub search terms
Simply modify the "Parameters" section with your GitHub credentials and desired search terms. 

```
# GitHub credentials
gh_username = 'pamelarussell'
gh_oauth_file = 'gh_oauth_token.txt'

# GitHub search terms
topics = ['bioinformatics']
languages = ['scala', 'java']
issue_label = 'help wanted'
```

#### Results
The running notebook will print a summary of repos and open issues matching your search terms.
