# Incremental Load Design


## Objective

Process only new or modified records instead of loading complete datasets.


## Incremental Strategy


Watermark Based Loading


Example:


Source Column:

LastModifiedDate


Logic:

Load records where:


LastModifiedDate > Previous Watermark



## Process Flow


1. Read previous watermark value

2. Extract changed records

3. Load into Bronze

4. Transform into Silver

5. Update watermark


## Merge Logic


Matching Key:

Primary Key / Business Key


When Match:

Update existing record


When Not Match:

Insert new record



## Benefits

- Reduced processing time
- Reduced compute cost
- Improved scalability
