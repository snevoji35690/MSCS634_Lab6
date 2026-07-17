# MSCS_634_Lab_6

## Student Information

**Name:** Srujana Nevoji
**Course:** MSCS 634 – Data Mining
**Lab:** Lab 6 – Frequent Itemset Mining and Association Rule Analysis

## Purpose

The purpose of this lab was to analyze transactional retail data using Apriori and FP-Growth. The lab identified frequent product combinations, generated association rules, compared algorithm execution times, and interpreted purchasing relationships using support, confidence, and lift.

## Dataset

The Online Retail dataset from the UCI Machine Learning Repository was used. It contains invoice-level transactions from a UK-based online retailer. A country-level subset was selected to make frequent-itemset mining more computationally manageable.

## Data Preparation

The dataset was cleaned by removing incomplete transaction records, cancelled invoices, nonpositive quantities, duplicate rows, and unnecessary spaces in product descriptions. The cleaned data was converted into a binary transaction basket in which each row represented an invoice and each column represented a product.

## Methods

The following techniques were applied:

* Transactional data cleaning
* Product-frequency visualization
* Item co-occurrence analysis
* Apriori frequent-itemset mining
* FP-Growth frequent-itemset mining
* Association-rule generation
* Support, confidence, and lift analysis
* Algorithm execution-time comparison

## Key Insights

Both Apriori and FP-Growth produced the same frequent itemsets when the same support threshold was used. The association rules identified products that customers frequently purchased together. Rules with high confidence and lift may be useful for cross-selling, recommendation systems, product bundling, and inventory planning.

FP-Growth was generally more efficient because it avoided the extensive candidate-generation process used by Apriori. The execution-time difference depended on the size and density of the selected transaction subset.

## Challenges and Decisions

A major challenge was selecting a useful minimum-support threshold. A high threshold returned only a few patterns, while a very low threshold generated too many itemsets and increased execution time. The dataset was filtered to one country to keep the basket size manageable.

Additional cleaning was required to remove cancelled transactions, incomplete descriptions, duplicate records, and nonpositive quantities before frequent-pattern mining.

## Conclusion

This lab demonstrated how frequent-itemset mining and association-rule analysis can reveal meaningful purchasing relationships in transactional retail data. Apriori provided an understandable candidate-based approach, while FP-Growth offered a more efficient alternative for larger transaction sets.
