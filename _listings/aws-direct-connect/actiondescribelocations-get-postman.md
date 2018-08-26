{
  "info": {
    "name": "AWS Direct Connect API Describe Locations",
    "_postman_id": "c39d5cd2-1658-4a1d-9e49-da152ece5291",
    "description": "Returns the list of AWS Direct Connect locations in the current AWS region.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Connections",
      "item": [
        {
          "id": "4084a065-b6b2-4123-a5bb-937f00f77464",
          "name": "allocateConnectionOnInterconnect",
          "request": {
            "url": "http://example.com/api/?Action=AllocateConnectionOnInterconnect?bandwidth=bandwidth&connectionName=connectionName&interconnectId=interconnectId&ownerAccount=ownerAccount&vlan=vlan",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a hosted connection on an interconnect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93cfe573-1edf-4f9d-a7bd-5a810712edae"
            }
          ]
        },
        {
          "id": "0b4294c5-c6f6-48ed-8994-eae2b5ace68e",
          "name": "confirmConnection",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmConnection?connectionId=connectionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirm the creation of a hosted connection on an interconnect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0eb8e26a-19ef-4878-b1c1-086e4c57f0ab"
            }
          ]
        },
        {
          "id": "07545854-bc8f-4df1-a4e9-722a1e40cc22",
          "name": "createConnection",
          "request": {
            "url": "http://example.com/api/?Action=CreateConnection?bandwidth=bandwidth&connectionName=connectionName&location=location",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new connection between the customer network and a specific AWS Direct Connect location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c708c476-ed12-4c9a-a645-b71f70057bec"
            }
          ]
        },
        {
          "id": "3b12f909-bb3a-4567-9ce4-e19545d96a44",
          "name": "deleteConnection",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConnection?connectionId=connectionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the connection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00433f23-ef82-494f-abbf-77c64917a9ab"
            }
          ]
        },
        {
          "id": "74b50af8-c226-43c7-afa1-3e03df5b5156",
          "name": "describeConnectionLoa",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConnectionLoa?connectionId=connectionId&loaContentType=loaContentType&providerName=providerName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the LOA-CFA for a Connection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6273132-23d9-459b-9b6f-e82cb4304344"
            }
          ]
        },
        {
          "id": "ceea51ba-15f2-43e3-b53b-cc663468eb08",
          "name": "describeConnections",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConnections?connectionId=connectionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Displays all connections in this region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2461d77a-f58d-4d32-8e9a-2b6fe48764b2"
            }
          ]
        },
        {
          "id": "cd93814b-578b-40bf-b1f4-9e4be16a62f6",
          "name": "describeConnectionsOnInterconnect",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConnectionsOnInterconnect?interconnectId=interconnectId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of connections that have been provisioned on the given interconnect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf3aa640-6742-47a4-bdb9-6a9b5cacaa5f"
            }
          ]
        }
      ]
    },
    {
      "name": "Private Virtual Interfaces",
      "item": [
        {
          "id": "fe77595a-2e3a-4e22-a3e6-ae129a786e0b",
          "name": "allocatePrivateVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=AllocatePrivateVirtualInterface?connectionId=connectionId&newPrivateVirtualInterfaceAllocation=newPrivateVirtualInterfaceAllocation&ownerAccount=ownerAccount",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provisions a private virtual interface to be owned by a different customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88be6152-6f7f-4c69-8173-3eb945bc6fbc"
            }
          ]
        },
        {
          "id": "dd48f75b-5fbf-488d-99d4-9bb1945507fb",
          "name": "allocatePublicVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=AllocatePublicVirtualInterface?connectionId=connectionId&newPublicVirtualInterfaceAllocation=newPublicVirtualInterfaceAllocation&ownerAccount=ownerAccount",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provisions a public virtual interface to be owned by a different customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70922f03-11b8-4015-86fd-4c9010fe8da9"
            }
          ]
        },
        {
          "id": "6322382d-e2f7-42ab-bf13-07130c1aa846",
          "name": "confirmPrivateVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmPrivateVirtualInterface?virtualGatewayId=virtualGatewayId&virtualInterfaceId=virtualInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accept ownership of a private virtual interface created by another customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97da290c-b067-4079-9633-60731bfd4996"
            }
          ]
        },
        {
          "id": "e2fc7bc4-a5a7-413b-bf11-e9ea17866a5e",
          "name": "confirmPublicVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmPublicVirtualInterface?virtualInterfaceId=virtualInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accept ownership of a public virtual interface created by another customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5beb4ba7-f489-4823-80d1-7f036f4f44cf"
            }
          ]
        },
        {
          "id": "2694506e-4953-4cb3-beb4-2841dd09c3d3",
          "name": "createPrivateVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=CreatePrivateVirtualInterface?connectionId=connectionId&newPrivateVirtualInterface=newPrivateVirtualInterface",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new private virtual interface."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "676a81c6-a6bd-4048-8c77-293dae21f645"
            }
          ]
        },
        {
          "id": "96686cbc-6567-4aa0-ab37-c127f3388b73",
          "name": "createPublicVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=CreatePublicVirtualInterface?connectionId=connectionId&newPublicVirtualInterface=newPublicVirtualInterface",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new public virtual interface."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba3dd768-0f0d-4c53-8b1d-c046356341cd"
            }
          ]
        }
      ]
    },
    {
      "name": "BGP Peer",
      "item": [
        {
          "id": "30a54921-3e61-4b56-9b33-5486fb0b3570",
          "name": "createBGPPeer",
          "request": {
            "url": "http://example.com/api/?Action=CreateBGPPeer?newBGPPeer=newBGPPeer&virtualInterfaceId=virtualInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new BGP peer on a specified virtual interface."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "992e274f-ffab-4ac7-b1dc-efd00f13bce4"
            }
          ]
        },
        {
          "id": "9fe063a5-0752-489d-9cd5-4cd56107c7ac",
          "name": "deleteBGPPeer",
          "request": {
            "url": "http://example.com/api/?Action=DeleteBGPPeer?asn=asn&customerAddress=customerAddress&virtualInterfaceId=virtualInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a BGP peer on the specified virtual interface that matches the specified customer address and ASN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22923e1d-533c-4796-b9cd-2a9f44831e3c"
            }
          ]
        }
      ]
    },
    {
      "name": "Interconnects",
      "item": [
        {
          "id": "7d09db19-5fa7-4ef5-b146-40cefe0d09aa",
          "name": "createInterconnect",
          "request": {
            "url": "http://example.com/api/?Action=CreateInterconnect?bandwidth=bandwidth&interconnectName=interconnectName&location=location",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new interconnect between a AWS Direct Connect partner's network and a specific AWS Direct Connect location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b587bebf-e3b1-4d58-8471-b861a941b8d7"
            }
          ]
        },
        {
          "id": "7d2435aa-eb04-4c40-a3e7-29f640a25c6b",
          "name": "deleteInterconnect",
          "request": {
            "url": "http://example.com/api/?Action=DeleteInterconnect?interconnectId=interconnectId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified interconnect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6747098d-6be7-4b49-9f6b-bab62fd68dcf"
            }
          ]
        },
        {
          "id": "1ab15c39-ffad-42a8-b8d1-6ebc2dee6c11",
          "name": "describeInterconnectLoa",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInterconnectLoa?interconnectId=interconnectId&loaContentType=loaContentType&providerName=providerName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the LOA-CFA for an Interconnect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bae09a38-5920-4e0a-b833-0e20fe1c871a"
            }
          ]
        },
        {
          "id": "42887fdb-5686-4071-bdd4-8ed4b332c6bc",
          "name": "describeInterconnects",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInterconnects?interconnectId=interconnectId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of interconnects owned by the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47e1ee99-1462-434a-a1e2-b42b92418741"
            }
          ]
        }
      ]
    },
    {
      "name": "Virtual Interfaces",
      "item": [
        {
          "id": "d765bd60-c406-4463-b102-bba71b49682d",
          "name": "deleteVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVirtualInterface?virtualInterfaceId=virtualInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a virtual interface."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85fb1fca-55cb-4d39-82d9-2a319b5f76e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Locations",
      "item": [
        {
          "id": "fdfe22e8-59c2-43a3-b978-a5d0ecf0cf03",
          "name": "describeLocations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLocations?locations=locations",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of AWS Direct Connect locations in the current AWS region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "083e5e1f-0776-417c-820f-656f355b8536"
            }
          ]
        }
      ]
    }
  ]
}