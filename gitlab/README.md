# Gitlab devops_mapping_contrib
This directory contains the following artifacts for mapping Gitlab events and Gitlab CI/CD data to our DevOps data models
1. `props.conf`: Contains eval statements for mapping important Gitlab fields to data model specific fields and naming
2. `transforms.conf`: Contains regex transform defintions for extracting DevOps related information from specific Gitlab fields.
3. `macros.conf`: Contains macros used to do more advanced transformations on on Gitlab data to align with data model specific fields
4. `eventtypes.conf` and `tags.conf`: Contains mappings for Gitlab data to event types and tags used by DevOps data models.

## DevOps Data Model Information
The DevOps data models provide a function similar to the Splunk Common Information Model (CIM) but for DevOps specific use cases. This DevOps data model data can then be used alongside traditional CIM data to enable more in depth use cases. Using this data helps investigate and answer questions more quickly when using Splunk with observability data in Splunk Enterprise/Cloud/Enterprise Security/ITSI/etc.

For a better understanding of these data models, the fields they contain, and how those fields can be used to link DevOps processes from issue creation all the way through to deployment and montioring check out [this Google Sheet](https://docs.google.com/spreadsheets/d/1ulrZuU1vpmgQBnctl7O0FiyaaV6l8wmfHaObG9q0z38)