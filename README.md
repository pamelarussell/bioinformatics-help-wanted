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

## Results

The running notebook will print a summary of repos and open issues matching your search terms.

Example results:

```
Repo: hail-is/hail
Description: Scalable genomic data analysis.
Language: Scala
URL: https://github.com/hail-is/hail
Open issues with label "help wanted":
	- Improve nCubeOfVolumeAtMost (https://github.com/hail-is/hail/issues/1998)
	- Hail's Matrix Multiply Should Perform Better When Massively Reducing Size (https://github.com/hail-is/hail/issues/1975)


Repo: biojava/biojava
Description: :book::microscope::coffee: BioJava is an open-source project dedicated to providing a Java library for processing biological data.
Language: Java
URL: https://github.com/biojava/biojava
Open issues with label "help wanted":
	- Extend dssp implementation to also support the promotif standard (https://github.com/biojava/biojava/issues/764)
	- Use Protonation Variants Companion Dictionary (https://github.com/biojava/biojava/issues/686)
	- Secondary structure assignment could be done taking all symmetry partners into account (https://github.com/biojava/biojava/issues/454)
	- Add Bird parsing functionality (https://github.com/biojava/biojava/issues/436)
	- Add support for parsing secondary structure in mmCIFF (https://github.com/biojava/biojava/issues/333)
	- New StructuralAlignment Algorithms (https://github.com/biojava/biojava/issues/307)
	- Introduction of semiglobal alignments (https://github.com/biojava/biojava/issues/243)
	- Add ability to create a Profile from a multiple sequence alignment file  (https://github.com/biojava/biojava/issues/223)
	- MrBayes Parser (https://github.com/biojava/biojava/issues/123)
	- Balibase (https://github.com/biojava/biojava/issues/119)
	- Add a SCOP2 parser (https://github.com/biojava/biojava/issues/82)


Repo: openwdl/wdl
Description: Workflow Description Language - Specification and Implementations
Language: Java
URL: https://github.com/openwdl/wdl
Open issues with label "help wanted":
	- map contains_key() function (https://github.com/openwdl/wdl/issues/305)
	- Allow passthrough of inputs from the `inputs.json` to a subworkflow (https://github.com/openwdl/wdl/issues/262)
 
 
.
.
.
```