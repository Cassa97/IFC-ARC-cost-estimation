# IFC-ARC-cost-estimation
Case study for conference paper CIB 78 &amp; buildingSMART 2024

The research aims to compare the 5D BIM cost estimation method with a newly proposed approach implemented through a code in IfcOpenShell. This innovative method utilizes structured cost items in IFC and establishes the relationship between cost and geometric IFC entities. The results indicate that the new approach is more agile and effective than the traditional 5D BIM method, which relies on cost assignment via attributes. The new method allows for querying cost items based on information contained within geometric entities and verifying the plausibility of the links between these entities and the cost estimates.

The FlowChart is:

<img src="https://github.com/Cassa97/IFC-ARC-cost-estimation/assets/115898053/8ef2f2b0-fdba-4ed2-abaf-70721c2903d0" width="500" >  

IFC Model:

<img src="https://github.com/Cassa97/IFC-ARC-cost-estimation/assets/115898053/614d2fb1-001f-436f-a6a2-601f16c4e912" width="500" >  



## Advantages and Disadvantages of 5D BIM and Proposed Method

### 5D BIM Method

| **Advantages**                                                                                      | **Disadvantages**                                                                                                     |
|-----------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| Automated Quantity Extraction: Quantities are automatically extracted from the input model if present. | Reliance on Unstructured Data: Associations between cost items and geometric objects rely on unstructured data, leading to potential errors. |
| Automatic Quantity Updates: Quantities are updated automatically when changes are made.              | Lack of Validation: Inability to validate the associations between cost items and geometric objects.                   |
| IFC Model Import and Reading: Seamless importation of IFC models.                                    | Manual Cost Item Selection: The process of selecting cost items and preparing cost estimates remains manual, increasing the risk of human errors. |
| Graphical Interface for Object Visualization and Selection: Allows for intuitive visualization and selection of geometric objects through a graphical interface. | Dependence on Input Model Quality: Accurate quantity extraction depends on the quality and completeness of the input model. |
| Multiple Object Selection: Facilitates the selection of multiple geometric objects simultaneously.    | Limited Interoperability: Challenges in achieving interoperability across different domains due to reliance on unstructured data. |
|                                                                                                     | Association of Cost Items via Alphanumeric Codes: Cost items are associated solely through alphanumeric codes inserted in the attributes of geometric objects. |
|                                                                                                     | Insertion of Multiple Codes in a Single Attribute: If an object involves multiple tasks and cost items (e.g., casting, formwork, reinforcement), different codes must be inserted into the same attribute. |
|                                                                                                     | Human Error in Cost Item Selection: There is a risk of human error in selecting unit cost items to associate with objects. |
|                                                                                                     | Manual Measurement Rule Entry/Selection: Measurement rules must be manually entered or selected.                         |
|                                                                                                     | Manual Group Selection: Groups of geometric objects to which cost items are associated must be manually selected.       |
|                                                                                                     | Lack of Automatic/Semi-Automatic Data Validation: There is no capability for automatic or semi-automatic validation of the coherence between cost items and associated geometric objects. |
|                                                                                                     | Static Cost Estimate Documents: Cost estimate documents are generated in static formats (Excel and PDF), limiting flexibility and dynamism. |

### Proposed Method

| **Advantages**                                                                                      | **Disadvantages**                                                                                                     |
|-----------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| Automatic Quantity Extraction: Quantities are automatically extracted from the input model, if present. | Application Through Programming Language: The method is only applicable through a programming language, limiting accessibility to users who are not proficient in programming. |
| Automatic Quantity Updates: Quantities are automatically updated when modifications are made.         | Lack of a Graphic Viewer: Currently, there is no graphical viewer for the model, making it more challenging to visualize and interact with the data. |
| IFC Model Import and Reading: The method facilitates easy import and reading of IFC models.           | Need to Validate the Input Model: It is necessary to validate the input model to ensure the presence of required information, such as quantities in geometric objects, which can be a complex and time-consuming process. |
| Data Consistency Validation: The ability to validate the consistency of data between cost-object relationships, reducing errors. |                                                                                                                       |
| Structured Relationships between IFC Entities: Utilizes structured relationships between IFC entities characterized by specific architectures and attributes, enhancing data organization and analysis. |                                                                                                                       |
| Semi-Automatic Cost Entity Suggestions: Provides semi-automatic suggestions for appropriate cost entities for the geometric object's cost estimation. |                                                                                                                       |
| IFC Model Update: The method allows for the processing of an updated IFC model with the insertion of cost entities. |                                                                                                                       |
| IFC Model Querying and Data Analysis: Enables querying and in-depth analysis of the IFC model data.  |                                                                                                                       |
| Exporting Multiple Cost Estimate Views: Allows for the exportation of multiple cost estimate views, offering greater flexibility and dynamism. |                                                                                                                       |
