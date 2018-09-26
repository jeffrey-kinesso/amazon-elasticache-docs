# Data Security<a name="encryption"></a>

To help keep your data secure, Amazon ElastiCache and Amazon EC2 provide mechanisms to guard against unauthorized access of your data on the server\.

Amazon ElastiCache for Redis also provides optional encryption features for data on clusters running Redis version 3\.2\.6:
+ In\-transit encryption encrypts your data whenever it is moving from one place to another, such as between nodes in your cluster or between your cluster and your application\.
+ At\-rest encryption encrypts your on\-disk data during sync and backup operations\.

If you want to enable in\-transit or at\-rest encryption, you must meet the following conditions\.
+ Your cluster or replication group must be running Redis version 3\.2\.6\.
+ Your cluster or replication group must be created in a Amazon VPC\.
+ Optionally, you can also use AUTH and the AUTH token \(password\) needed to perform operations on this cluster or replication group\.

![\[Image: ElastiCache for Redis Security Diagram\]](http://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/./images/ElastiCache-Redis-Secure-Compliant.png)

*ElastiCache for Redis Security Diagram*

**Topics**
+ [ElastiCache for Redis In\-Transit Encryption \(TLS\)](in-transit-encryption.md)
+ [ElastiCache for Redis At\-Rest Encryption](at-rest-encryption.md)
+ [Authenticating Users with Redis AUTH](auth.md)