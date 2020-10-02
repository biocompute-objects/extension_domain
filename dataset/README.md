# Extension to External References: Additional Licenses and Dataset Catagories

The external references example extension to list additional licenses and dataset catagories .
```json
    "extension_schema": "http://www.w3id.org/biocompute/extension_domain/1.0.0/dataset/dataset_extension.json",
    
    "extension_domain": {
        "additional_license": {
            "data_license": "https://creativecommons.org/licenses/by/4.0/",
            "script_license": "https://www.gnu.org/licenses/gpl-3.0.en.html"
        },
            "dataset_categories": [
            {
                "category_value": "Homo sapiens",
                "category_name": "species"
            },
            {
                "category_value": "Protein",
                "category_name": "molecule"
            },
            {
                "category_value": "Protein Canonical Accessions",
                "category_name": "tags"
            },
            {
                "category_value": "csv",
                "category_name": "file_type"
            },
            {
                "category_value": "Reviewed",
                "category_name": "status"
            },
            {
                "category_value": "internal",
                "category_name": "scope"
            }
        ]
    }
```

## **additional_license**
The additional license property contains the details about the licenses applied to the dataset and the script or tool/software used to process the given dataset. Licenses ensure the permissions are clear to use, modify, and share one’s work by other users.

  **data_license**:  The license applied to the data or the dataset by the author. Usually, most organizations and academic settings widely use Creative Commons licenses that allow open access to knowledge with no or limited restrictions. The most popular license is the [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/) license that allows users to use, share, transform, and distribute the data as per their requirement provided attribution is given to the original author.
 eg. ```
 "data_license": "https://creativecommons.org/licenses/by/4.0/" ```
 
 **script_license**: The license applied to the computational script or the tool/software developed to process (parse, QC, align) the input dataset for a final output dataset. There are 5 types of commonly used software licenses for publishing the code. Four of these licenses are open-source allowing reuse of the code to some extent while proprietary licenses are the most restrictive license in terms of code reuse. For most dataset scripts, open-source license such as [GNU General Public License v3](http://www.gnu.org/licenses/gpl-3.0.html) is used.
eg. ``` "script_license": "https://www.gnu.org/licenses/gpl-3.0.en.html"```

## dataset_categories
Dataset categories describe and provide more information about the dataset which can be used to classify, group, sort and filter datasets. Currently, there are six categories for describing a dataset: species, molecule, tags, file_type, status, and scope. Each category has a distinct value.

**species**: This category provides information about the species to which the data belongs. The values can be a single scientific name of any species in NCBI taxonomy. When the datasets contain data from multiple species the value can be left blank

eg.  ```{
                "category_value": "Homo sapiens",
                "category_name": "species"
            } ```
  

**molecule**: This category provides information about the biological macromolecules to which the data belongs. The value of the category can be either protein, glycan, nucleic acid, lipids, and proteoform. Other molecule values can be used if the molecule category is different than the above.
eg.  ``` {
                "category_value": "Protein",
                "category_name": "molecule"
            }```

**tags**:  This category adds a tag to a dataset. The values for the tag category can be a dataset name, resource name, data types, etc.
eg.  ```{
                "category_value": "Protein Canonical Accessions",
                "category_name": "tags"
            } ```

**file_type**: This category describes the file format type of the dataset. The values of the file_type category can be csv, txt, fasta, tsv, nt, gpff, etc
eg.  ```{
                "category_value": "csv",
                "category_name": "file_type"
            } ```

**status**: This category provides information about the current status of the dataset. The values of the status category can be: reviewed and retired.
eg.  ``` {
                "category_value": "Reviewed",
                "category_name": "status"
            }```

**scope**: This category provides information about the usage scope of the dataset. The values of the scope category are internal and external. Datasets with the internal scope are used for internal purposes whereas datasets with the external scope are custom processed for use by external people or resources.
eg.  ```{
                "category_value": "Reviewed",
                "category_name": "status"
            } ```

The external references **example** extension to list additional licenses and dataset catagories .


