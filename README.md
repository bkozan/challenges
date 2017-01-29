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
-Lets see what happens without two spaces
*The above line has a minus, and this line has a star  
The above line received dual spaces
