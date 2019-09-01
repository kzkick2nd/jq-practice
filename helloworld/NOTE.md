# list all array
$ jq .

# return elements of array
$ jq .[]

# select with statement
$ jq '.[] | select(.id == "0002")' sample.json

# select with deep nest key-value
$ jq '.[] | select(.group1.subg01[].id == "1021")' sample.json
