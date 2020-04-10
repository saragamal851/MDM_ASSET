This code is mainly about how to use DataStage to execute a script on a secured remote UNIX / Linux Server by using SSH client. 
This can be used in several use-cases where a remote Unix/Linux application invocation is required to complete an ETL task

In this code, we will discuss a use-case of loading a physical Master Data Management system through the Batch Processor interface.
 This will be done by calling the batch processor command which is part of the Infopshere MDM distribution. A sample DataStage job implementing such functionality is attached. 
This example can be extended to call any remote unix/linux command.


There is a reusable and adjustable .dsx file attached for any similar requirements.
A .dsx file is a file that is created when using Datastage Manager to export jobs from a project.
There should be Datastage Server installed to run the executable jobs. 
You can import ETL datastage jobs by following below steps:
	Open Websphere Datastage Designer 
	Go to “Import” in the menu, Select “DataStage Components…”
	Then Browse for the .dsx file path and click “OK”.
  
After importing DS jobs, go to the main job sequence that contains steps required to run MDM batches on MDM server throught using DS designer client. And by reading the attached document, it will be easy to understand each stage in the sequence,how it works and the expected output from it.
