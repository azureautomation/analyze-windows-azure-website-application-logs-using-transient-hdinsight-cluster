Analyze Windows Azure Website application logs using transient HDInsight cluster
================================================================================

            

[Windows Azure Scripting Center](http://www.windowsazure.com/en-us/documentation/scripts) |
[Get Started with Windows Azure PowerShell](http://go.microsoft.com/fwlink/?linkid=320929&clcid=0x409) |
[Windows Azure Big Data Scripts](http://www.windowsazure.com/en-us/documentation/scripts/index/?solution=big-data&service=all)

Description

Analyze Windows Azure Website application logs using transient HDInsight cluster.


If azure web site is configured to store application logs in azure blob storage this script can be used to generate performance metrics of the web site based on the following pattern in application log message: 'Perf: <perfmetricname> took <number>'.
 The script will calculate for each perf metric found in the logs its average value and CSV formatted table of the metric values for each time-stamp. Processing of the data is performed on the transient HDInsight cluster which is provisioned for the duration
 of the script execution. The script also creates new storage account to store output of the analysis. The output files can be imported into Excel or other graphing tool to build graphic chart of values.


**Note:** This script uses AzCopy utility downloadable form here: http://go.microsoft.com/fwlink/?LinkId=287086

Example

Scenario
You want to analyze performance of Azure Web Site based on application logs.
Requirements

  *  PowerShell Version 3.0 
  *  Windows Azure PowerShell December 2013 
  *  AzCopy 
See Also

  *  Set-AzureSubscription 
  *  [Windows Azure Big Data Scripts](http://www.windowsazure.com/en-us/documentation/scripts/index/?solution=big-data&service=all)

Script Content

The content of the script is reproduced below

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
