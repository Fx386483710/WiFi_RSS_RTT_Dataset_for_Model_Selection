open-data-template
==================

Provides a template for publishing a high quality open dataset. Each repository is designed to host a single dataset, consisting of one or more files.

To create a dataset with open data certificate

1) Upload data files into the data/ directory.

2) For each file uploaded you need to add a .data file in the data directory that specifies the metadata for the file, this file should look like the examples and contain the following fields. Note that the category <b>must not</b> be changed from data.

```
category: data
filename: filname.csv
weight: 2
title: June 2014
description: Transactions in June 2014
type: text/csv
```

Key:

```
weight: The position that the file is displayed on the page, 1 being first.

type: The IANA mime type of the file, e.g. text/csv, application/json etc.
```

2) Edit _config.yml and fill in all the values that describe this dataset, changing the examples

3) Point certificates.theodi.org at the front page of the site and let it automatically fill in values (then add the embed code to _config.yml)

4) Note that many of the certificate fields can be filled in by using the github features that are available under the "Data quality and accuracy" sections.


To customise the look and feel of your dataset site
===================================================

1) Replace logo.png in the img directory with your own company logo

2) edit css/style.css to change colour schemes of the site.
