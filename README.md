# Example: Clear Watermark from ObjectStore

This Mule project is an example of how to clear the watermark from the object store that was set in a Poll wrapper. The project has a batch flow that selects records from a MySQL table and then sets the watermark for the last record ID. The second flow provides an API endpoint that provides a way to reset the watermark by opening a link to http://localhost:80801/clearwatermark

# Setup
  1. Run the 'records.sql' script against a MySQL database
  2. Modify the 'MySQL_Configuration' to point to your MySQL database with the newly created table.
  3. Run the project
  4. Navigate to http://localhost:8081/clearwatermark

# Versions
Project was built with the following versions.

  - Anypoint Studio 5.4
  - MySQL
  - Java SDK 7
  - Mule EE 3.7.3
  - ObjectStore 1.3.3

# Reference

Poll Reference
https://docs.mulesoft.com/mule-user-guide/v/3.7/poll-reference

ObjectStore
http://mulesoft.github.io/objectstore-connector/1.3.3/apidocs/mule/objectstore-config.html#retrieve-store

```
Updated: 12/11/2015 by dejim.juang@mulesoft.com
```
