# <a href="http://ozan.io/california-academic-performance-index-data/">California API Data</a>

> The Academic Performance Index (API) is a measurement of academic performance and progress of individual schools in California.

This repository contains the <a href="http://ozan.io/california-academic-performance-index-data/">site</a> containing the
2000-2013 California API data files along with a script to automatically download and generate them.

## Generating the data
After intalling [Node.js](https://nodejs.org/), execute the following commands in your terminal:

```sh
git clone https://github.com/unsetbit/california-academic-performance-index-data.git;
cd california-academic-performance-index-data;
npm install;
node ./scripts/download.js
```

The script will download the data from [http://www.cde.ca.gov/ta/ac/ap/apidatafiles.asp](http://www.cde.ca.gov/ta/ac/ap/apidatafiles.asp),
process them (unzip, etc...), then put them in the ./data folder.
