# REDI Metadata and Data Assessment
This repository contains public documentation of the REDI metadata schema under ongoing development.  

**Please note**: field definitions will become more rigorous over time, and REDI controlled terms are expected to expand as lists or hierarchies of valid terms.   

This repository also contains working data assessment documentation undergoing development. REDI data standards will be established based on this documentation. Feedback from the community is encouraged to refine expectations.

## Metadata Organization
Within the current REDI model, "collections" contain "artifacts", "data layers", and "models." 
Data layers can also contain "features", and models can have an associated "configuration". 
Collections, artifacts, data layers, features, models, and configurations each have descriptive metadata associated with them.  

![REDI Model Diagram](https://github.com/In-For-Disaster-Analytics/metadata-schema/blob/main/visuals/redi-model-diagram.png)

Collections group one or more layers, artifacts and/or models together. 
For example, a complex geospatial database object would be represented as a collection containing multiple data layers.

Artifacts represent digital objects such as text and images within documents, data within spreadsheets, or other data made available via service endpoints. 
Artifacts do not contain geometry information (points, lines, or polygons) or images with spatial information. 

Data layers represent digital objects with intrinsic spatial characteristics and include (but are not limited to) streets, city boundaries, river gages, and imagery with geospatial information contained within files or made available via service endpoints. 

Features, as a part of a data layer, are a record-by-record description of each independent “row” in a geospatial attribute table or database. 

Models represent model software packages and configurations, which may be associated with input and/or output artifacts or data layers. 
Model configurations represent a unique way of running a model, exposing concrete inputs, outputs, and parameters. These metadata are under active development.

## Documentation in this Repository

For a human-readable description of metadata fields, see: [redi_metadata_field_documentation.md](https://github.com/In-For-Disaster-Analytics/metadata-schema/blob/main/fields_by_level/redi_metadata_field_documentation.md)

For CSV files containing metadata field definitions according to level, see: [fields_by_level](https://github.com/In-For-Disaster-Analytics/metadata-schema/tree/main/fields_by_level)

For CSV files containing controlled terms for particular metadata fields, see: [controlled_terms](https://github.com/In-For-Disaster-Analytics/metadata-schema/tree/main/controlled_terms)

For examples and templates showing use of REDI metadata fields, see: [examples_and_templates](https://github.com/In-For-Disaster-Analytics/metadata-schema/tree/main/examples_and_templates)
