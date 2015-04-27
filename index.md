# California Academic Performance Index (API) Data

The Academic Performance Index data can be updated by running npm install; node ./scripts/crawling/getAPIFiles.js;. The data will be automatically crawled and put inside the tmp folder.

The files are retrieved from http://www.cde.ca.gov/ta/ac/ap/apidatafiles.asp. The data files are converted to CSV and the layout html pages are converted to JSON files. For convenience, a header line is added to the CSV which is the names of the fields from the layout file.

There are scripts in scripts/mongo which can be used to load this data to a mongodb instance and clean it up a bit for running map/reduce on.
