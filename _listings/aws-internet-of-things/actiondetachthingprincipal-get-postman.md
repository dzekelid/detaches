{
  "info": {
    "name": "AWS Internet of Things API Detach Thing Principal",
    "_postman_id": "89002089-dc8f-4567-9515-e169f6873396",
    "description": "Detaches the specified principal from the specified thing.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Certificate Transfers",
      "item": [
        {
          "id": "846991cc-3779-4fe1-a376-4740edb81f37",
          "name": "acceptCertificateTransfer",
          "request": {
            "url": "http://example.com/api/?Action=AcceptCertificateTransfer?certificateId=certificateId&setAsActive=setAsActive",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts a pending certificate transfer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b026985-1b67-412f-bc61-2ea995459236"
            }
          ]
        },
        {
          "id": "3f953900-c802-411c-804e-640e02954fe7",
          "name": "cancelCertificateTransfer",
          "request": {
            "url": "http://example.com/api/?Action=CancelCertificateTransfer?certificateId=certificateId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a pending transfer for the specified certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e070783-504b-401d-bb7c-d04c019deb8d"
            }
          ]
        }
      ]
    },
    {
      "name": "Principal Policies",
      "item": [
        {
          "id": "585f00bd-6928-432c-a56b-e69513f9b230",
          "name": "attachPrincipalPolicy",
          "request": {
            "url": "http://example.com/api/?Action=AttachPrincipalPolicy?policyName=policyName&principal=principal",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified policy to the specified principal (certificate or other credential)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84d38b28-3feb-4614-a59f-c3d55fa9c81b"
            }
          ]
        },
        {
          "id": "ce0d744b-1222-498d-a4fe-0658f58624a6",
          "name": "detachPrincipalPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DetachPrincipalPolicy?policyName=policyName&principal=principal",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified policy from the specified certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e65a84a-9aa4-4900-8e17-e8d9dda137be"
            }
          ]
        }
      ]
    },
    {
      "name": "Thing Principals",
      "item": [
        {
          "id": "ada864a3-3a04-4bbd-877d-3fe88c050b07",
          "name": "attachThingPrincipal",
          "request": {
            "url": "http://example.com/api/?Action=AttachThingPrincipal?principal=principal&thingName=thingName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified principal to the specified thing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20e85329-074f-4843-a06d-c4a0919e08e0"
            }
          ]
        },
        {
          "id": "54488d52-201b-46f0-aed7-5b9b2f571337",
          "name": "detachThingPrincipal",
          "request": {
            "url": "http://example.com/api/?Action=DetachThingPrincipal?principal=principal&thingName=thingName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches the specified principal from the specified thing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14aaf48a-13b4-49e2-9214-e9700c2510eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "1240f8de-a1be-4ec7-a3dc-6a8da410ae35",
          "name": "createCertificateFromCsr",
          "request": {
            "url": "http://example.com/api/?Action=CreateCertificateFromCsr?certificateSigningRequest=certificateSigningRequest&setAsActive=setAsActive",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an X."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a563b25e-1a83-412e-9556-6f3b2bcd573d"
            }
          ]
        },
        {
          "id": "24c2628b-0eff-42de-bc41-c1c0b27f8023",
          "name": "deleteCertificate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCertificate?certificateId=certificateId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ab9a283-7097-4099-8225-04a81424a398"
            }
          ]
        },
        {
          "id": "41205a8a-b677-4306-bd86-702e6f26d55b",
          "name": "describeCertificate",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCertificate?certificateId=certificateId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the specified certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b68c5b9-35a6-4e43-8157-9de9d7082958"
            }
          ]
        }
      ]
    },
    {
      "name": "Keys And Certificates",
      "item": [
        {
          "id": "40c1d88a-87ac-4860-95ef-bfaae61fc950",
          "name": "createKeysAndCertificate",
          "request": {
            "url": "http://example.com/api/?Action=CreateKeysAndCertificate?setAsActive=setAsActive",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a 2048-bit RSA key pair and issues an X."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad7f5c0d-4940-4494-aa46-0548716d9dbb"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "1f0bc9cf-e3a6-4b5f-8303-a4c44bce9458",
          "name": "createPolicy",
          "request": {
            "url": "http://example.com/api/?Action=CreatePolicy?policyDocument=policyDocument&policyName=policyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an AWS IoT policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0c58830-ce56-48e0-91ad-f2f189d94d75"
            }
          ]
        },
        {
          "id": "ba6694b1-3f8d-4408-84cf-339739540875",
          "name": "createPolicyVersion",
          "request": {
            "url": "http://example.com/api/?Action=CreatePolicyVersion?policyDocument=policyDocument&policyName=policyName&setAsDefault=setAsDefault",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new version of the specified AWS IoT policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8330fa25-4a43-4643-af84-6075fc240722"
            }
          ]
        },
        {
          "id": "c6bacb5e-213f-47fb-b1fd-d10498ee94d1",
          "name": "deletePolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeletePolicy?policyName=policyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90a3590b-78d5-45e7-baa2-9cdb80b6902f"
            }
          ]
        },
        {
          "id": "42ee0656-0c5c-4f2b-8339-817ec047fd02",
          "name": "deletePolicyVersion",
          "request": {
            "url": "http://example.com/api/?Action=DeletePolicyVersion?policyName=policyName&policyVersionId=policyVersionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified version of the specified policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04bd7631-5c8b-42ca-ba3d-ce169795637d"
            }
          ]
        }
      ]
    },
    {
      "name": "Things",
      "item": [
        {
          "id": "a83f4f76-1c6d-4feb-a554-33d51fe756bf",
          "name": "createThing",
          "request": {
            "url": "http://example.com/api/?Action=CreateThing?attributePayload=attributePayload&thingName=thingName&thingTypeName=thingTypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a thing record in the thing registry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b9ab5ef-7186-41a4-b1df-2f6053cdc575"
            }
          ]
        },
        {
          "id": "89b7cd22-d12a-48fd-b7bd-6b2ae73b2942",
          "name": "deleteThing",
          "request": {
            "url": "http://example.com/api/?Action=DeleteThing?expectedVersion=expectedVersion&thingName=thingName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified thing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e244ce2-3640-41de-9af2-8994f7b8d2d2"
            }
          ]
        },
        {
          "id": "714d9cb0-3783-4e6d-88e6-3a6f0c1a8784",
          "name": "describeThing",
          "request": {
            "url": "http://example.com/api/?Action=DescribeThing?thingName=thingName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the specified thing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be4fd167-8bcc-4f1d-ba65-1451934f28ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Thing Types",
      "item": [
        {
          "id": "dd732e44-410e-4363-9a5a-337db535b13e",
          "name": "createThingType",
          "request": {
            "url": "http://example.com/api/?Action=CreateThingType?thingTypeName=thingTypeName&thingTypeProperties=thingTypeProperties",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new thing type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9336ac6c-b77b-41ae-89eb-71869b5dcd08"
            }
          ]
        },
        {
          "id": "af843883-71fd-44bd-93b0-2d8eee23878a",
          "name": "deleteThingType",
          "request": {
            "url": "http://example.com/api/?Action=DeleteThingType?thingTypeName=thingTypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified thing type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90f5fdcb-a328-4ff2-b0c1-f4c09030556f"
            }
          ]
        },
        {
          "id": "4f2d2c4d-2c65-42c0-ac3c-194f4bbe07a6",
          "name": "deprecateThingType",
          "request": {
            "url": "http://example.com/api/?Action=DeprecateThingType?thingTypeName=thingTypeName&undoDeprecate=undoDeprecate",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deprecates a thing type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56a2abaa-cbfc-46b4-b6e2-778891e788d0"
            }
          ]
        },
        {
          "id": "c845d79d-b109-48ed-a1c5-2d663d849052",
          "name": "describeThingType",
          "request": {
            "url": "http://example.com/api/?Action=DescribeThingType?thingTypeName=thingTypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the specified thing type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55030bde-23ac-4318-882f-19a4a49a937a"
            }
          ]
        }
      ]
    },
    {
      "name": "Topic Rules",
      "item": [
        {
          "id": "0a3701a8-5b6f-41b2-bc72-998efd24c28b",
          "name": "createTopicRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateTopicRule?ruleName=ruleName&topicRulePayload=topicRulePayload",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a73f587c-393e-45a0-b96e-0126b595f09e"
            }
          ]
        },
        {
          "id": "506c812d-49d4-4e3c-ae2d-f16f85fd5988",
          "name": "deleteTopicRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTopicRule?ruleName=ruleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9106d5e2-dc40-43d9-98d4-ed98934a9b57"
            }
          ]
        }
      ]
    },
    {
      "name": "CA Certificates",
      "item": [
        {
          "id": "60a7e512-77ab-465c-b80d-73e196033af1",
          "name": "deleteCACertificate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCACertificate?certificateId=certificateId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a registered CA certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df9e6d6a-d5f9-4ff8-92f8-09ff8af460c6"
            }
          ]
        },
        {
          "id": "482dde7b-5a92-47f2-ae5f-753c6a99634a",
          "name": "describeCACertificate",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCACertificate?certificateId=certificateId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a registered CA certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c70da6a1-3352-410f-9bf1-d8cc7e40726a"
            }
          ]
        }
      ]
    },
    {
      "name": "Registration Codes",
      "item": [
        {
          "id": "500104f1-e254-472e-ba3c-ddc962dc4a86",
          "name": "deleteRegistrationCode",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRegistrationCode",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a CA certificate registration code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c9588b4-c7d9-4e3f-92db-75202aa65e76"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "4bfa1c51-e8e9-43ea-a9f1-5830112d9ad6",
          "name": "describeEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEndpoint?endpointAddress=endpointAddress",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a unique endpoint specific to the AWS account making the call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c69a2e2-588d-4785-bd45-b950f718441c"
            }
          ]
        }
      ]
    }
  ]
}