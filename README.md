# doc

aws s3 mb s3://bucket-name
aws s3 rb s3://bucket-name
aws s3 ls
aws s3 cp C:\Users\test\Desktop\test.png s3://areik - S3 bucket copy file
aws ec2 describe-instances --filters "Name=instance-type,Values=t2.micro"
aws ec2 create-key-pair --key-name mykeypair
aws ec2 terminate-instances --instance-ids i-5203422c
aws ec2 create-security-group --group-name my-sg --description "My security group
aws ec2 describe-security-groups --group-names my-sg
aws ec2 create-security-group --group-name my-sg --description "My security group" --vpc-id vpc-1a2b3c4d
aws ec2 authorize-security-group-ingress --group-name my-sg --protocol tcp --port 3389 --cidr 203.0.113.0/24
aws ec2 delete-security-group --group-name my-sg
aws ec2 delete-security-group --group-id sg-903004f8
aws ec2 describe-instance-status
aws ec2 run-instances --image-id ami-e90dc68a --count 1 --instance-type t2.micro --key-name qwikLABS-L117-359887 --security-groups my-sg
aws ec2 create-snapshot --volume-id vol-656f37bf --description "This is my root volume snapshot."
aws ec2 describe-volumes
aws ec2 describe-snapshots -snapshot-id snap-6ed73e7f
aws ec2 create-image --instance-id i-873f1723 --name "My server" --description "An AMI for my server" --no-reboot
aws ec2 run-instances --image-id ami-e90dc68a --count 1 --instance-type t2.micro --key-name qwikLABS-L117-359887 --security-group-ids sg-bb8048df --subnet-id subnet-3d076a58 (launch instance in specific subnet)
aws elb create-load-balancer --load-balancer-name my-load-balancer --listeners "Protocol=HTTP,LoadBalancerPort=80,InstanceProtocol=HTTP,InstancePort=80" --subnets subnet-15aaab61 --security-groups sg-a61988c3
aws elb create-load-balancer --load-balancer-name my-load-balancer --listeners --scheme internal "Protocol=HTTP,LoadBalancerPort=80,InstanceProtocol=HTTP,InstancePort=80" --subnets subnet-15aaab61 --security-groups sg-a61988c3
aws elb register-instances-with-load-balancer --load-balancer-name my-load-balancer --instances i-d6f6fae3
aws ec2 describe-instances --filters "Name=instance-type,Values=t2.micro,Name=instance-state-name,Values=terminated"
aws ec2 allocate-address
aws ec2 associate-address --instance-id i-873f1723 --public-ip 52.77.88.244
aws ec2 stop-instances --instance-ids i-1a2b3c4d
aws ec2 start-instances --instance-ids i-1a2b3c4d
aws ec2 terminate-instances --instance-ids i-1a2b3c4d
aws ec2 attach-volume --volume-id vol-1234abcd --instance-id i-abcd1234 --device /dev/sdf
aws ec2 detach-volume --volume-id vol-1234abcd
