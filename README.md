# Challenges

S3 PUT & DELETE trigger Lambda

Lambda gathers information about the operation (Bucket, Key, UserID, etc)

Passes the relevant information to a Step Function

Step function runs a Choice State, depending on the relevant information, it takes an action (or several)

*Add or remove information from DynamoDB

*Run SNS Topic if particular user deletes a file

*Modify file properties

*Move or Copy file to different bucket

