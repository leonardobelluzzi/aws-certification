
There are three fundamental drivers of cost with AWS: compute, storage, and outbound data transfer.

![[Pasted image 20250716084410.png]]



### Data transfer between S3 and EC2 instances within the same region is not charged

There are three fundamental drivers of cost with AWS: compute, storage, and outbound data transfer. In most cases, there is no charge for inbound data transfer or data transfer between other AWS services within the same region. Outbound data transfer is aggregated across services and then charged at the outbound data transfer rate.

Per AWS pricing, data transfer between S3 and EC2 instances within the same region is not charged, so there would be no data transfer charge for moving 500 GB of data from an EC2 instance to an S3 bucket in the same region.