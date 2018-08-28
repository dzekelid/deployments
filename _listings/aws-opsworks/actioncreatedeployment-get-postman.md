{
  "info": {
    "name": "AWS OpsWorks API Create Deployment",
    "_postman_id": "7658828f-1905-4635-b0e7-7a1ba4b005e6",
    "description": "Runs deployment or stack commands.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Instances",
      "item": [
        {
          "id": "a3d93887-217c-4185-ac5b-eae34e3a35b7",
          "name": "assignInstance",
          "request": {
            "url": "http://example.com/api/?Action=AssignInstance?InstanceId=InstanceId&LayerIds=LayerIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assign a registered instance to a layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "608156bd-237c-4b39-86f2-cea701b535cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Volumes",
      "item": [
        {
          "id": "8cd345b8-94e0-4641-a04a-5428ff8e3998",
          "name": "assignVolume",
          "request": {
            "url": "http://example.com/api/?Action=AssignVolume?InstanceId=InstanceId&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assigns one of the stack's registered Amazon EBS volumes to a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bfe42f9-24da-421e-b5f2-ce38973b08e0"
            }
          ]
        }
      ]
    },
    {
      "name": "IP Addresses",
      "item": [
        {
          "id": "b8d98db0-c31f-4fff-b66f-6ead0304be26",
          "name": "associateElasticIp",
          "request": {
            "url": "http://example.com/api/?Action=AssociateElasticIp?ElasticIp=ElasticIp&InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates one of the stack's registered Elastic IP addresses with a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a0d22dc-a698-4e89-b147-6e1e40fdb3db"
            }
          ]
        }
      ]
    },
    {
      "name": "Load Balancers",
      "item": [
        {
          "id": "7aff31da-73e6-4f08-9977-276e2c02efc7",
          "name": "attachElasticLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=AttachElasticLoadBalancer?ElasticLoadBalancerName=ElasticLoadBalancerName&LayerId=LayerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches an Elastic Load Balancing load balancer to a specified layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ee6fe7d-94ea-4ca2-b278-1e589ffc9838"
            }
          ]
        }
      ]
    },
    {
      "name": "Stacks",
      "item": [
        {
          "id": "af453af5-1b4e-4629-b80d-ab99edc432ad",
          "name": "cloneStack",
          "request": {
            "url": "http://example.com/api/?Action=CloneStack?AgentVersion=AgentVersion&Attributes=Attributes&ChefConfiguration=ChefConfiguration&CloneAppIds=CloneAppIds&ClonePermissions=ClonePermissions&ConfigurationManager=ConfigurationManager&CustomCookbooksSource=CustomCookbooksSource&CustomJson=CustomJson&DefaultAvailabilityZone=DefaultAvailabilityZone&DefaultInstanceProfileArn=DefaultInstanceProfileArn&DefaultOs=DefaultOs&DefaultRootDeviceType=DefaultRootDeviceType&DefaultSshKeyName=DefaultSshKeyName&DefaultSubnetId=DefaultSubnetId&HostnameTheme=HostnameTheme&Name=Name&Region=Region&ServiceRoleArn=ServiceRoleArn&SourceStackId=SourceStackId&UseCustomCookbooks=UseCustomCookbooks&UseOpsworksSecurityGroups=UseOpsworksSecurityGroups&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a clone of a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79e5aa1c-a6ca-4e3e-ac73-d459fd257a10"
            }
          ]
        }
      ]
    },
    {
      "name": "Applications",
      "item": [
        {
          "id": "158e34c0-9bd8-4fb2-b2b8-e090f5ecc0f3",
          "name": "createApp",
          "request": {
            "url": "http://example.com/api/?Action=CreateApp?AppSource=AppSource&Attributes=Attributes&DataSources=DataSources&Description=Description&Domains=Domains&EnableSsl=EnableSsl&Environment=Environment&Name=Name&Shortname=Shortname&SslConfiguration=SslConfiguration&StackId=StackId&Type=Type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an app for a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1b7e91d-2167-4649-a923-f71be99258e9"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "4a1b3859-2551-4d11-a0e7-2f3e3604869c",
          "name": "createDeployment",
          "request": {
            "url": "http://example.com/api/?Action=CreateDeployment?AppId=AppId&Command=Command&Comment=Comment&CustomJson=CustomJson&InstanceIds=InstanceIds&LayerIds=LayerIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Runs deployment or stack commands."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "114a1713-b22c-41ed-aea1-dce1eb825381"
            }
          ]
        }
      ]
    }
  ]
}