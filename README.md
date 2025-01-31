## DataPower Domain Analysis Tool


### Description

This tool can be used to analyze the set of policies used across one or more DataPower domains. 
This is useful for migration purposes as it helps to understand and categorize the existing functionality. 

For example, if you are migrating from DataPower to Apigee, you can use the analysis tool to figure the set
of shared flows that would need to be implemented in Apigee.

### How it works

The tool assumes that you have created a domain backup/export from one or more domains in your DataPower box. 
This export is a zip file, which itself will contain other zip files for each domain that was exported.

Once you have the domain(s) exported, you can run the following command:

```shell script
dp-migrate analyze -b /path/to/domain/export.zip -o /path/to/output.xlsx
```

This will inspect the domains within the zip file and produce an Excel spreadsheet with a summary of
the policies used across the domains.

## Not Google Product Clause

This is not an officially supported Google product.
