# Create-an-IPv4-enabled-VPC-and-subnets-using-the-AWS-CLI

### Schritt 1
#### VPC erstellen - benutze den Folgen Code:

    aws ec2 create-vpc --cidr-block 10.0.0.0/16 --query Vpc.VpcId --output text 

#### er wirft dir dann folgendes als Beispiel zurück:

    vpc-1234f567h89
    
#### Subnet erstellen
#### Denk dran die folgene VPC ID mit deiner zu ersetzen 

        aws ec2 create-subnet --vpc-id vpc-2f09a348 --cidr-block 10.0.1.0/24
        
        aws ec2 create-subnet --vpc-id vpc-2f09a348 --cidr-block 10.0.0.0/24
