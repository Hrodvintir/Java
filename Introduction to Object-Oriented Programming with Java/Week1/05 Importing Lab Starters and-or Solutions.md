# Importing Lab Starters and/or Solutions

For each of our projects, we provide starting points (where appropriate) and solutions.  The files can be found under ~/class-files/.  The Starters/ directory has projects that can be imported if you have not completed previous labs, which includes labs from earlier courses in the Core Java Specialization.  The Solutions/ directory has solutions for all of the labs.  FYI, the starters are, in almost all cases, a copy of the solution to the prior lab.

Labs are cumulative, so once you have imported a starting point, you should not need to repeat this process for subsequent labs if you complete them in order successfully.

In order to use them, we go into Eclipse, select Import..., select Existing Projects into Workspace, chose Select archive file, click Browse..., locate the desired .ZIP file (e.g., ~/class-files/Coursera Lab Files/starters/SUVLab-starter.  Eclipse will show the project(s) to be imported.  Click Finish.

HOWEVER, this will not work for projects that already exist, so read further to see how to resolve that issue.

![alt text](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/2ue1u9u8TDyntbvbvGw8Cg_58e33e87cb754f738616d7dbdd2ec7f1_image.png?expiry=1643068800000&hmac=xC1QG5-IoMsNWmNBqRuAkKbSU5LHLDOk8JREU-jag9o)

If there is already a project by that name in the workspace, the Finish button will remain greyed out, and there will be a warning message: "Some projects cannot be imported because they already exist in the workspace" at the top of the dialog.

![alt text](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/2W3bVo4NQmGt21aODZJhgg_475bed569c8b4f2c9461380003055323_image.png?expiry=1643068800000&hmac=yfLeXhT8s3F8Ckvk89YYWxb77NXDFi2AOCCHnAPY0tA)

In order to over-write an existing project, we must first delete the existing one from your workspace, and then import.  So cancel the import, right-click on the project we need to delete, AND BE SURE to select Delete project contents on disk before clicking OK.  That checkbox is vital.  Without it, only metadata is removed, and we still won't be able to re-import the project.

![alt text](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Gh30McS1Qoqd9DHEtRKKsw_42cc5de6cee444eca01d248d57b00852_image.png?expiry=1643068800000&hmac=EFLzNr1fXRiCY-WHvVQEnlSkrsiwk2Mzi4hPRTuxXKg)

Now that the project has been deleted, you can re-import as normal.

External Tutorial: [How to import existing Java projects into Eclipse workspace](https://www.codejava.net/ides/eclipse/import-existing-projects-into-eclipse-workspace)
