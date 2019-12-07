# Generate NSF Collaborators and Other Affiliations Information from Your Publications

[NSF grant proposal guidelines](https://www.nsf.gov/pubs/policydocs/pappg18_1/pappg_2.jsp) require the listing of all possible reviewers who may have a conflict of interest with reviewing your application.

Some of these reviewers are relatively static (your Ph.D. advisor), but the bulk of them are people you've published with in the last 48 months. This notebook helps specifically with creating that section of the [COA form](https://www.nsf.gov/bfa/dias/policy/coa.jsp).

To start, you will either need:

1. A citation database of your publications

2. A Google Scholar profile ([see how to create](https://libguides.reading.ac.uk/boost/google-scholar-profile))

The output of the notebook will be tab-delimited data that can be copy/pasted into the NSF template

## Step 1: Get Citations in RIS format

### You have a citation database of your publications

These instructions are generic because there are many different types of citation database. The logical steps are:

1. Do a query to select all  publications that you are either an author of OR an editor of. In JabRef this would be, e.g., `author=olney or editor=olney`

2. Select the publications matching your query and then save/export in [RIS format](https://en.wikipedia.org/wiki/RIS_%28file_format%29). In JabRef this would be `File -> Export selected entries -> Save dialogue: enter file name and choose RIS file type`

### You have a Google Scholar profile

Note Google Scholar does not have gold-standard citation information but it is very likely to be correct for authors IF you have done some curation. It is not unusual to have to purge publications that aren't yours on initial set up.

1. Install [Publish or Perish](https://harzing.com/resources/publish-or-perish)

2. Do `Menu -> Query -> New Google Scholar Query -> input your name` followed by `Query pane -> Right click your name -> Save to File -> Save to RIS`

## Step 2: Run the Notebook

Run `nsf-coa-template.ipynb` using Jupyter or Azure Notebooks.
You will need to install [IFSharp](https://github.com/fsprojects/IfSharp) to run on Jupyter.
