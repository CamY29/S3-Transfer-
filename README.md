<h1>S3 Transfer of Files</h1>


<h2>Description</h2>
Using AWS platform I was able to create a bucket (or folder) in which I filled with files. After filling the bucket I then procided to make a lifecycle rule. In the rule I stated that after 30 days the file would be moved to Standard-IA storage for short-term. After 90 days the file will then be moved to Glaicer Flexible Retrieval for long-term storage. The next part of the lifecycle is to permanently delete files after they have been in the bucket for 120 days.
<br />


<h2>Languages and Utilities Used</h2>

- <b>CloudShell</b> 

<h2>Environments Used </h2>

- <b>AWS</b>

<h2>Program walk-through:</h2>

<p align="center">
This shows that the file was successfully uploaded to the bucket. <br/>
<img src="https://i.imgur.com/Ia8Lfku.png" height="80%" width="80%" alt="S3 Transfer steps"/>
<br /> 
<br />
This shows the first couple parts of the lifecycle. First you give the lifecycle a name for example in this case we named it delete unneeded files. After you chose whether you want the rule to limit the rule with specific filters or have the rule affect everything in the bucket.   <br/>
<img src="https://i.imgur.com/IuNELmC.png" height="80%" width="80%" alt="S3 Transfer steps"/>
<br />
<br />
In this second set of steps you start with determine rule actions you wish to apply. In this case we want to move current files between different storage classes. The next step is to determine where and when you want the files to move. For this instance we are having the files move to standard-IA after 30 days, then too Glacier Flexible Retrieval after 90 days. <br/>
<img src="https://i.imgur.com/E1KHqnU.png" height="80%" width="80%" alt="S3 Transfer steps"/>
<br />
<br />
In the last step determine when you want files in which haven't been used for a specific amount of time to be deleted. In our example we chose to delete files after 120 days.  <br/>
<img src="https://i.imgur.com/PNRG8IQ.png" height="80%" width="80%" alt="S3 Transfer steps"/>
<br />
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
