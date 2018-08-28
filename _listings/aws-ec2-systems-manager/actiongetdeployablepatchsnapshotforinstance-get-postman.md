{
  "info": {
    "name": "Amazon EC2 Systems Manager API Get Deployable Patch Snapshot For Instance",
    "_postman_id": "ff3500fd-6273-4aa8-8b2b-90bdeea5d7f9",
    "description": "Retrieves the current snapshot for the patch baseline the instance uses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "df500396-5f28-4575-9aa3-8842687eedd6",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&ResourceType=ResourceType&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfe4749b-9c38-4686-bcd0-ad70f54688fc"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "f967cef7-0054-4536-8922-4625ddd1e4f3",
          "name": "cancelCommand",
          "request": {
            "url": "http://example.com/api/?Action=CancelCommand?CommandId=CommandId&InstanceIds=InstanceIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attempts to cancel the command specified by the Command ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cba4660-4f0d-4154-832f-4cd8a56007fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "273ca2a1-4948-4b84-94ba-da3db494cec7",
          "name": "createActivation",
          "request": {
            "url": "http://example.com/api/?Action=CreateActivation?DefaultInstanceName=DefaultInstanceName&Description=Description&ExpirationDate=ExpirationDate&IamRole=IamRole&RegistrationLimit=RegistrationLimit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers your on-premises server or virtual machine with Amazon EC2 so that you can manage\n   these resources using Run Command."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d3a9313-c38c-47d8-b290-7be894776b40"
            }
          ]
        },
        {
          "id": "58a2c22f-e634-4d13-bde2-f1ce919b6946",
          "name": "deleteActivation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteActivation?ActivationId=ActivationId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an activation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9921ee40-329b-45eb-b433-360d17f6583d"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "1a92e61b-0969-40cd-88e1-aa86be99d863",
          "name": "createAssociation",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociation?DocumentVersion=DocumentVersion&InstanceId=InstanceId&Name=Name&OutputLocation=OutputLocation&Parameters=Parameters&ScheduleExpression=ScheduleExpression&Targets=Targets",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c00677a-adcb-4f0b-9d44-82063ba7ff65"
            }
          ]
        },
        {
          "id": "862fe6ed-6976-49e3-bd6e-823bf9392c3c",
          "name": "createAssociationBatch",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociationBatch?Entries=Entries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5a4d308-b962-4825-af16-b3c7de7d0ed6"
            }
          ]
        },
        {
          "id": "9f47cc34-ae8d-4207-85d1-dbd6ed0cc232",
          "name": "deleteAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates the specified SSM document from the specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6880828f-0893-4da0-9dfe-92ab5528e630"
            }
          ]
        },
        {
          "id": "e28b2eee-d5d7-40a3-979d-a6a8ff331f13",
          "name": "describeAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the associations for the specified SSM document or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d437cc45-5a46-47dd-ac6e-9610647fb56a"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "d506088f-7b2a-4647-a75a-36aa7ab479c5",
          "name": "createDocument",
          "request": {
            "url": "http://example.com/api/?Action=CreateDocument?Content=Content&DocumentType=DocumentType&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a932b16c-7d75-4637-9128-a4ad788756b4"
            }
          ]
        },
        {
          "id": "4e2737c9-199d-441a-8802-2314ead41c76",
          "name": "deleteDocument",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDocument?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the SSM document and all instance associations to the document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e86da90-9f98-4ef7-bce3-485534103603"
            }
          ]
        },
        {
          "id": "bf225e05-f5ae-4901-a509-ea1ba5aacfa8",
          "name": "describeDocument",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8adc373-b852-4947-ba78-c90dc2a2b784"
            }
          ]
        },
        {
          "id": "15c5ba56-db42-42d8-beea-2aa221bcc189",
          "name": "describeDocumentPermission",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocumentPermission?Name=Name&PermissionType=PermissionType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the permissions for an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44606ef5-2943-40bd-835d-ea2e400c5cb8"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "fb04113e-d702-4f6d-827e-f05298d69b84",
          "name": "createMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=CreateMaintenanceWindow?AllowUnassociatedTargets=AllowUnassociatedTargets&ClientToken=ClientToken&Cutoff=Cutoff&Duration=Duration&Name=Name&Schedule=Schedule",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2901dc5-7ff7-432b-ba02-aacba362d72d"
            }
          ]
        },
        {
          "id": "42f5df70-8a66-4b09-b329-028ed03c6eaa",
          "name": "deleteMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeleteMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bd8ce09-a9a9-428f-b8bf-86094637e609"
            }
          ]
        },
        {
          "id": "8f810a24-2673-4c1e-b445-b6fad6e3f70b",
          "name": "describeMaintenanceWindowExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the executions of a Maintenance Window (meaning, information about when the\n   Maintenance Window was scheduled to be active and information about tasks registered and run with\n   the Maintenance Window)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c133a125-f54c-4d96-923e-97d58d772d05"
            }
          ]
        },
        {
          "id": "40f71625-a96f-4039-b6d3-69d46840de5f",
          "name": "describeMaintenanceWindowExecutionTaskInvocations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTaskInvocations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&TaskId=TaskId&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the individual task executions (one per target) for a particular task executed\n   as part of a Maintenance Window execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cebd0a80-0543-4ae1-8a93-b310478d4de3"
            }
          ]
        },
        {
          "id": "e6959bb6-8656-4073-96d2-bdb61085acc5",
          "name": "describeMaintenanceWindowExecutionTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "For a given Maintenance Window execution, lists the tasks that were executed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08ef3cbe-6fd0-40d7-8d58-1513d688983d"
            }
          ]
        },
        {
          "id": "3ec9b486-ca94-40c5-b90f-a393577688cf",
          "name": "describeMaintenanceWindows",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindows?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the Maintenance Windows in an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1dc51325-be99-4eb7-b8b5-c5d73b6c5212"
            }
          ]
        },
        {
          "id": "48ff842e-a097-4b4b-a6d9-f0e3299a35c3",
          "name": "describeMaintenanceWindowTargets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTargets?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the targets registered with the Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e32d9933-6bf0-46f5-8b52-ad41f8b93b53"
            }
          ]
        },
        {
          "id": "1550c78c-112c-47eb-a6c9-9d0d19cf60b3",
          "name": "describeMaintenanceWindowTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the tasks in a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "919135d3-27e0-4fea-a7dd-83bb4d0cd2c9"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "30dd90c7-cf11-4df5-a885-49cd3022e7ad",
          "name": "createPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePatchBaseline?ApprovalRules=ApprovalRules&ApprovedPatches=ApprovedPatches&ClientToken=ClientToken&Description=Description&GlobalFilters=GlobalFilters&Name=Name&RejectedPatches=RejectedPatches",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1deaf76-7826-4d2d-9649-a5718d535fa8"
            }
          ]
        },
        {
          "id": "e1fcfff2-8d88-4d61-ae02-6925c3b80ded",
          "name": "deletePatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fd06b7f-54d3-4cf2-8531-6d9a82ba1326"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter",
      "item": [
        {
          "id": "24b6a1c8-5c71-4610-9387-654474b04bd1",
          "name": "deleteParameter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteParameter?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a parameter from the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "500fb207-63f8-4732-9208-d764496c38ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "5b3d4e78-2626-4583-94ff-9b121a97d92c",
          "name": "deregisterManagedInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterManagedInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the server or virtual machine from the list of registered servers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24acf984-ad78-42f2-a625-753ced7c3def"
            }
          ]
        },
        {
          "id": "260017ac-a844-44c6-913a-e75d4c043c61",
          "name": "deregisterPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a patch group from a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd89d60e-8e6c-48fd-9e40-84e822ccd1ff"
            }
          ]
        },
        {
          "id": "3dbc4d36-f4ae-4a12-a418-5d9eb068c6e8",
          "name": "deregisterTargetFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTargetFromMaintenanceWindow?WindowId=WindowId&WindowTargetId=WindowTargetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a target from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05bef791-17d5-4807-a0ad-6b58acd6935c"
            }
          ]
        },
        {
          "id": "ace6585e-5ce2-4549-9313-84f58af5ada6",
          "name": "deregisterTaskFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTaskFromMaintenanceWindow?WindowId=WindowId&WindowTaskId=WindowTaskId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a task from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a14fc52-4758-4d00-8040-922da6c822da"
            }
          ]
        }
      ]
    },
    {
      "name": "Activations",
      "item": [
        {
          "id": "902f399d-f381-4ab4-9ab6-2c9f45c0b7b6",
          "name": "describeActivations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActivations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about the activation, including: the date and time the activation was created,\n   the expiration date, the IAM role assigned to the instances in the activation, and the number of\n   instances activated by this registration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dccba444-d166-4c5e-8b7e-ddf3dc847d3b"
            }
          ]
        }
      ]
    },
    {
      "name": "Automation",
      "item": [
        {
          "id": "04302c39-878a-47b5-940a-414201be8f2b",
          "name": "describeAutomationExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutomationExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides details about all active and terminated Automation executions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15ed9947-7eaa-4bf2-b700-0171be62f3cc"
            }
          ]
        },
        {
          "id": "04c09b7f-9ea6-4f9f-befd-71a7b9b882a8",
          "name": "getAutomationExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetAutomationExecution?AutomationExecutionId=AutomationExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get detailed information about a particular Automation execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3a395cb-a216-42ac-9424-464fb86fc353"
            }
          ]
        }
      ]
    },
    {
      "name": "Available",
      "item": [
        {
          "id": "db141f33-3c70-4cdc-899e-c0b146836d38",
          "name": "describeAvailablePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailablePatches?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patches that could possibly be included in a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25485e5f-5396-4a2d-b2e4-726ea82b13fc"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "6425af85-7c6f-4366-9cad-c24d4968b547",
          "name": "describeEffectiveInstanceAssociations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectiveInstanceAssociations?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40c48eec-2be9-414b-9bca-d2d1c26607db"
            }
          ]
        },
        {
          "id": "6b790213-bfa6-4250-a37f-078a788cc08c",
          "name": "describeEffectivePatchesForPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectivePatchesForPatchBaseline?BaselineId=BaselineId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current effective patches (the patch and the approval state) for the specified patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d6c5ea0-e4d2-4581-a0f9-b5454063b109"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "88f35075-4339-44aa-9bd7-fd9bdd7cf852",
          "name": "describeInstanceAssociationsStatus",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceAssociationsStatus?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The status of the associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7c24cb0-f710-4dc1-a490-3746ea398283"
            }
          ]
        },
        {
          "id": "c32cc406-abb5-4e1e-9241-d904f8c5b67c",
          "name": "describeInstanceInformation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceInformation?Filters=Filters&InstanceInformationFilterList=InstanceInformationFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "822a483f-d92b-4c9e-9768-616524f2a683"
            }
          ]
        },
        {
          "id": "8235b793-92d6-4011-953f-55641a8ab6d0",
          "name": "describeInstancePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatches?Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the patches on the specified instance and their state relative to the patch baseline being used for the instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a2f1712-ce63-462f-9699-73f0c5dba897"
            }
          ]
        },
        {
          "id": "7856c30c-7341-4410-aa96-9acc1d595fa6",
          "name": "describeInstancePatchStates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStates?InstanceIds=InstanceIds&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state of one or more instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed112022-114c-4d29-bb7d-265d439e92c0"
            }
          ]
        },
        {
          "id": "4df6fd30-c223-411e-aae3-824339eefb15",
          "name": "describeInstancePatchStatesForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStatesForPatchGroup?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state for the instances in the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b8a23a1-583d-4345-8213-30204c100695"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "09f1f0a1-f5cd-480a-a1d5-c9cf8250c3ec",
          "name": "describeParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeParameters?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "718a743e-cfc4-48cc-abdd-a7d90dc96a39"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "906fbffb-8dbf-4dfc-b7ad-1007d86201ad",
          "name": "describePatchBaselines",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchBaselines?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the patch baselines in your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2893e2c2-3349-4755-a88f-d91cce5e7b02"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "4fc5ce22-f274-4099-9513-44718da8eb19",
          "name": "describePatchGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroups?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patch groups that have been registered with patch baselines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6538f01-ccce-4496-b684-03119e18512a"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "9cd6b49f-8a57-4d8c-9736-9583221d4ebf",
          "name": "describePatchGroupState",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroupState?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns high-level aggregated patch compliance state for a patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2e92488-1397-4009-bbfa-87eb55c59bbc"
            }
          ]
        }
      ]
    },
    {
      "name": "Command",
      "item": [
        {
          "id": "46e04211-f6eb-4405-a054-df17e11e25d9",
          "name": "getCommandInvocation",
          "request": {
            "url": "http://example.com/api/?Action=GetCommandInvocation?CommandId=CommandId&InstanceId=InstanceId&PluginName=PluginName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information about command execution for an invocation or plugin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78da20fe-3165-40ea-8440-a0129cc2cc40"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "abd8f0e9-3bae-4bd1-a9d2-507c0d72adf2",
          "name": "getDefaultPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetDefaultPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the default patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ef75210-ed84-4be7-af98-3e7da21686a9"
            }
          ]
        }
      ]
    },
    {
      "name": "Deployable",
      "item": [
        {
          "id": "1c0c8fd3-bd27-44f6-812f-288274c74acd",
          "name": "getDeployablePatchSnapshotForInstance",
          "request": {
            "url": "http://example.com/api/?Action=GetDeployablePatchSnapshotForInstance?InstanceId=InstanceId&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current snapshot for the patch baseline the instance uses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0cfe0ce-5c33-4862-8bf9-b02855e30533"
            }
          ]
        }
      ]
    }
  ]
}