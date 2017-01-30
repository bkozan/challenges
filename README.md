# Challenges

##Gather Object Info
S3 PUT & DELETE trigger Lambda  
Lambda gathers information about the operation (Bucket, Key, UserID, etc)  
Any information not found from trigger, run 'List' operation on object, gather additional information, place into variables.  

##Pass info to Step Function  
Step function runs a Choice State, depending on the relevant information, it takes an action (or several)  
+Add or remove information from DynamoDB  
+Run SNS Topic if particular user deletes a file  
+Modify file properties  
+Move or Copy file to different bucket  

##PUT and Encrypt with KMS
Via CLI or AWS-Shell, PUT items into a bucket, and encrypt them using KMS  
--I was successful in this, however, I then removed my CLI user from the Key Users group, and the operation still succeeded.... Needs furhter investigation.  

##Other
Find a way for Git updates to update my Lambda functions without Console interaction. (Code Pipeline?)  

Query my CloudTrail or S3 logs with Athena.  
+What to do with the results?  

Find a way for all S3 Buckets to enforce mandatory logging to specific folder "/logs/".  

##Super Advanced
Convert some logs into Parque with Snappy? 
