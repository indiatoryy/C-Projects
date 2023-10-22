# Autocomplete
Autocomplete is a high-performance implementation designed to quickly retrieve top terms matching a query string from a dataset of terms, each associated with an importance weight.

## How it Works
When dealing with large datasets of terms, Autocomplete provides an efficient way to find relevant suggestions based on user input. It operates in the following steps:
### 1. Data Preparation:
* Read in a file containing a large number of terms, each associated with an importance weight.
* Sort the terms in lexicographic order. This sorted list will be reused for multiple queries.
### 2. Autocomplete Process:
* Use binary search to find the location of the first term in lexicographic ordering that matches the query string.
* Find the last term in lexicographic ordering that matches the query string.
* Extract the terms that match the query string and sort them by weight.
### 3. Result Generation:
* Extract the top matching terms based on their weight.
* Display the top terms as autocomplete suggestions for the given query.

## Example
For example, given the query string "Com", the matching terms might be "Computer", "Computation", and "Complete". Autocomplete will efficiently identify and display these terms based on their importance weight.
