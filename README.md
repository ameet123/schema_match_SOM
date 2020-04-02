## SChema Matching
BAsed on repo: https://github.com/TanviSahay/Schema-Matching-using-Machine-Learning 

Trying to reproduce results.


### HowTo
Collect the data from : https://www.cms.gov/Research-Statistics-Data-and-Systems/Research-Statistics-Data-and-Systems 
Two files,
+ . Hospital measures
+ . state measures

1. These files are loaded into a postgres database
2. A python program fetches the data and extracts features
3. The `Jupyter` notebook is run,

### Results
test to train attribute match is captured as follows in the generated file,
Top 2 attributes based on EDIT distance and avg probability are selected.
The highlighted rows contain 2 attributes indicating not a perfect match, while the others are perfect matches.

 ![results](image/results.jpg)
 
 ### Changes
 1. migrated to python 3
 2. simplified functions
 3. added a mechanism to rank the selections based on 2 metrics - distance and avg probability.