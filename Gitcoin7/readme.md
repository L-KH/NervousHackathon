

This is the submission of "Gitcoin: 7) Port An Existing Ethereum DApp To Polyjuice"

### Screenshots or video of your application running on Godwoken.

![](https://github.com/L-KH/NervousHackathon/blob/main/Gitcoin7/application_running_on_Godwoken.png)

### Link to the GitHub repository with your application which has been ported to Godwoken. This must be a different application than the one covered in this guide.

https://github.com/L-KH/NervousHackathon/tree/main/Gitcoin7/repoGit7

### If you deployed any smart contracts as part of this tutorial, please provide the transaction hash of the deployment transaction, the deployed contract address, and the ABI of the deployed smart contract. (Provide all in text format.)



```
{
  "contractName": "SimpleStorage",
  "abi": [
    {
      "inputs": [],
      "stateMutability": "payable",
      "type": "constructor"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "x",
          "type": "uint256"
        }
      ],
      "name": "set",
      "outputs": [],
      "stateMutability": "payable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "get",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    }
  ],
  "metadata": "{\"compiler\":{\"version\":\"0.8.3+commit.8d00100c\"},\"language\":\"Solidity\",\"output\":{\"abi\":[{\"inputs\":[],\"stateMutability\":\"payable\",\"type\":\"constructor\"},{\"inputs\":[],\"name\":\"get\",\"outputs\":[{\"internalType\":\"uint256\",\"name\":\"\",\"type\":\"uint256\"}],\"stateMutability\":\"view\",\"type\":\"function\"},{\"inputs\":[{\"internalType\":\"uint256\",\"name\":\"x\",\"type\":\"uint256\"}],\"name\":\"set\",\"outputs\":[],\"stateMutability\":\"payable\",\"type\":\"function\"}],\"devdoc\":{\"kind\":\"dev\",\"methods\":{},\"version\":1},\"userdoc\":{\"kind\":\"user\",\"methods\":{},\"version\":1}},\"settings\":{\"compilationTarget\":{\"/C/Users/nervous/Desktop/test/blockchain-workshop-ethereum-simple/contracts/SimpleStorage.sol\":\"SimpleStorage\"},\"evmVersion\":\"istanbul\",\"libraries\":{},\"metadata\":{\"bytecodeHash\":\"ipfs\"},\"optimizer\":{\"enabled\":false,\"runs\":200},\"remappings\":[]},\"sources\":{\"/C/Users/nervous/Desktop/test/blockchain-workshop-ethereum-simple/contracts/SimpleStorage.sol\":{\"keccak256\":\"0x29c258c41da0efee217b856aee40bbd1bdfccedc47ead54a253bc56f8fbab614\",\"urls\":[\"bzz-raw://d393bfe335fb4c33d40855293f34ec69e470ab346c480d354f65631464fbc0ed\",\"dweb:/ipfs/QmVXYLdWEB5RDPuKG31FHZF5cwRXepHJsGPQbLDxQXWQ8M\"]}},\"version\":1}",
  "bytecode": "0x6080604052607b60008190555061012f8061001b6000396000f3fe60806040526004361060265760003560e01c806360fe47b114602b5780636d4ce63c146043575b600080fd5b60416004803603810190603d9190608f565b6069565b005b348015604e57600080fd5b5060556073565b6040516060919060c2565b60405180910390f35b8060008190555050565b60008054905090565b60008135905060898160e5565b92915050565b60006020828403121560a057600080fd5b600060ac84828501607c565b91505092915050565b60bc8160db565b82525050565b600060208201905060d5600083018460b5565b92915050565b6000819050919050565b60ec8160db565b811460f657600080fd5b5056fea26469706673582212202bb51a1f0363c4b0462c934684e1722ee344fe61b6fdc9016e00da7036d6526b64736f6c63430008030033",
  "deployedBytecode": "0x60806040526004361060265760003560e01c806360fe47b114602b5780636d4ce63c146043575b600080fd5b60416004803603810190603d9190608f565b6069565b005b348015604e57600080fd5b5060556073565b6040516060919060c2565b60405180910390f35b8060008190555050565b60008054905090565b60008135905060898160e5565b92915050565b60006020828403121560a057600080fd5b600060ac84828501607c565b91505092915050565b60bc8160db565b82525050565b600060208201905060d5600083018460b5565b92915050565b6000819050919050565b60ec8160db565b811460f657600080fd5b5056fea26469706673582212202bb51a1f0363c4b0462c934684e1722ee344fe61b6fdc9016e00da7036d6526b64736f6c63430008030033",
  "immutableReferences": {},
  "generatedSources": [],
  "deployedGeneratedSources": [
    {
      "ast": {
        "nodeType": "YulBlock",
        "src": "0:980:1",
        "statements": [
          {
            "body": {
              "nodeType": "YulBlock",
              "src": "59:87:1",
              "statements": [
                {
                  "nodeType": "YulAssignment",
                  "src": "69:29:1",
                  "value": {
                    "arguments": [
                      {
                        "name": "offset",
                        "nodeType": "YulIdentifier",
                        "src": "91:6:1"
                      }
                    ],
                    "functionName": {
                      "name": "calldataload",
                      "nodeType": "YulIdentifier",
                      "src": "78:12:1"
                    },
                    "nodeType": "YulFunctionCall",
                    "src": "78:20:1"
                  },
                  "variableNames": [
                    {
                      "name": "value",
                      "nodeType": "YulIdentifier",
                      "src": "69:5:1"
                    }
                  ]
                },
                {
                  "expression": {
                    "arguments": [
                      {
                        "name": "value",
                        "nodeType": "YulIdentifier",
                        "src": "134:5:1"
                      }
                    ],
                    "functionName": {
                      "name": "validator_revert_t_uint256",
                      "nodeType": "YulIdentifier",
                      "src": "107:26:1"
                    },
                    "nodeType": "YulFunctionCall",
                    "src": "107:33:1"
                  },
                  "nodeType": "YulExpressionStatement",
                  "src": "107:33:1"
                }
              ]
            },
            "name": "abi_decode_t_uint256",
            "nodeType": "YulFunctionDefinition",
            "parameters": [
              {
                "name": "offset",
                "nodeType": "YulTypedName",
                "src": "37:6:1",
                "type": ""
              },
              {
                "name": "end",
                "nodeType": "YulTypedName",
                "src": "45:3:1",
                "type": ""
              }
            ],
            "returnVariables": [
              {
                "name": "value",
                "nodeType": "YulTypedName",
                "src": "53:5:1",
                "type": ""
              }
            ],
            "src": "7:139:1"
          },
          {
            "body": {
              "nodeType": "YulBlock",
              "src": "218:196:1",
              "statements": [
                {
                  "body": {
                    "nodeType": "YulBlock",
                    "src": "264:16:1",
                    "statements": [
                      {
                        "expression": {
                          "arguments": [
                            {
                              "kind": "number",
                              "nodeType": "YulLiteral",
                              "src": "273:1:1",
                              "type": "",
                              "value": "0"
                            },
                            {
                              "kind": "number",
                              "nodeType": "YulLiteral",
                              "src": "276:1:1",
                              "type": "",
                              "value": "0"
                            }
                          ],
                          "functionName": {
                            "name": "revert",
                            "nodeType": "YulIdentifier",
                            "src": "266:6:1"
                          },
                          "nodeType": "YulFunctionCall",
                          "src": "266:12:1"
                        },
                        "nodeType": "YulExpressionStatement",
                        "src": "266:12:1"
                      }
                    ]
                  },
                  "condition": {
                    "arguments": [
                      {
                        "arguments": [
                          {
                            "name": "dataEnd",
                            "nodeType": "YulIdentifier",
                            "src": "239:7:1"
                          },
                          {
                            "name": "headStart",
                            "nodeType": "YulIdentifier",
                            "src": "248:9:1"
                          }
                        ],
                        "functionName": {
                          "name": "sub",
                          "nodeType": "YulIdentifier",
                          "src": "235:3:1"
                        },
                        "nodeType": "YulFunctionCall",
                        "src": "235:23:1"
                      },
                      {
                        "kind": "number",
                        "nodeType": "YulLiteral",
                        "src": "260:2:1",
                        "type": "",
                        "value": "32"
                      }
                    ],
                    "functionName": {
                      "name": "slt",
                      "nodeType": "YulIdentifier",
                      "src": "231:3:1"
                    },
                    "nodeType": "YulFunctionCall",
                    "src": "231:32:1"
                  },
                  "nodeType": "YulIf",
                  "src": "228:2:1"
                },
                {
                  "nodeType": "YulBlock",
                  "src": "290:117:1",
                  "statements": [
                    {
                      "nodeType": "YulVariableDeclaration",
                      "src": "305:15:1",
                      "value": {
                        "kind": "number",
                        "nodeType": "YulLiteral",
                        "src": "319:1:1",
                        "type": "",
                        "value": "0"
                      },
                      "variables": [
                        {
                          "name": "offset",
                          "nodeType": "YulTypedName",
                          "src": "309:6:1",
                          "type": ""
                        }
                      ]
                    },
                    {
                      "nodeType": "YulAssignment",
                      "src": "334:63:1",
                      "value": {
                        "arguments": [
                          {
                            "arguments": [
                              {
                                "name": "headStart",
                                "nodeType": "YulIdentifier",
                                "src": "369:9:1"
                              },
                              {
                                "name": "offset",
                                "nodeType": "YulIdentifier",
                                "src": "380:6:1"
                              }
                            ],
                            "functionName": {
                              "name": "add",
                              "nodeType": "YulIdentifier",
                              "src": "365:3:1"
                            },
                            "nodeType": "YulFunctionCall",
                            "src": "365:22:1"
                          },
                          {
                            "name": "dataEnd",
                            "nodeType": "YulIdentifier",
                            "src": "389:7:1"
                          }
                        ],
                        "functionName": {
                          "name": "abi_decode_t_uint256",
                          "nodeType": "YulIdentifier",
                          "src": "344:20:1"
                        },
                        "nodeType": "YulFunctionCall",
                        "src": "344:53:1"
                      },
                      "variableNames": [
                        {
                          "name": "value0",
                          "nodeType": "YulIdentifier",
                          "src": "334:6:1"
                        }
                      ]
                    }
                  ]
                }
              ]
            },
            "name": "abi_decode_tuple_t_uint256",
            "nodeType": "YulFunctionDefinition",
            "parameters": [
              {
                "name": "headStart",
                "nodeType": "YulTypedName",
                "src": "188:9:1",
                "type": ""
              },
              {
                "name": "dataEnd",
                "nodeType": "YulTypedName",
                "src": "199:7:1",
                "type": ""
              }
            ],
            "returnVariables": [
              {
                "name": "value0",
                "nodeType": "YulTypedName",
                "src": "211:6:1",
                "type": ""
              }
            ],
            "src": "152:262:1"
          },
          {
            "body": {
              "nodeType": "YulBlock",
              "src": "485:53:1",
              "statements": [
                {
                  "expression": {
                    "arguments": [
                      {
                        "name": "pos",
                        "nodeType": "YulIdentifier",
                        "src": "502:3:1"
                      },
                      {
                        "arguments": [
                          {
                            "name": "value",
                            "nodeType": "YulIdentifier",
                            "src": "525:5:1"
                          }
                        ],
                        "functionName": {
                          "name": "cleanup_t_uint256",
                          "nodeType": "YulIdentifier",
                          "src": "507:17:1"
                        },
                        "nodeType": "YulFunctionCall",
                        "src": "507:24:1"
                      }
                    ],
                    "functionName": {
                      "name": "mstore",
                      "nodeType": "YulIdentifier",
                      "src": "495:6:1"
                    },
                    "nodeType": "YulFunctionCall",
                    "src": "495:37:1"
                  },
                  "nodeType": "YulExpressionStatement",
                  "src": "495:37:1"
                }
              ]
            },
            "name": "abi_encode_t_uint256_to_t_uint256_fromStack",
            "nodeType": "YulFunctionDefinition",
            "parameters": [
              {
                "name": "value",
                "nodeType": "YulTypedName",
                "src": "473:5:1",
                "type": ""
              },
              {
                "name": "pos",
                "nodeType": "YulTypedName",
                "src": "480:3:1",
                "type": ""
              }
            ],
            "src": "420:118:1"
          },
          {
            "body": {
              "nodeType": "YulBlock",
              "src": "642:124:1",
              "statements": [
                {
                  "nodeType": "YulAssignment",
                  "src": "652:26:1",
                  "value": {
                    "arguments": [
                      {
                        "name": "headStart",
                        "nodeType": "YulIdentifier",
                        "src": "664:9:1"
                      },
                      {
                        "kind": "number",
                        "nodeType": "YulLiteral",
                        "src": "675:2:1",
                        "type": "",
                        "value": "32"
                      }
                    ],
                    "functionName": {
                      "name": "add",
                      "nodeType": "YulIdentifier",
                      "src": "660:3:1"
                    },
                    "nodeType": "YulFunctionCall",
                    "src": "660:18:1"
                  },
                  "variableNames": [
                    {
                      "name": "tail",
                      "nodeType": "YulIdentifier",
                      "src": "652:4:1"
                    }
                  ]
                },
                {
                  "expression": {
                    "arguments": [
                      {
                        "name": "value0",
                        "nodeType": "YulIdentifier",
                        "src": "732:6:1"
                      },
                      {
                        "arguments": [
                          {
                            "name": "headStart",
                            "nodeType": "YulIdentifier",
                            "src": "745:9:1"
                          },
                          {
                            "kind": "number",
                            "nodeType": "YulLiteral",
                            "src": "756:1:1",
                            "type": "",
                            "value": "0"
                          }
                        ],
                        "functionName": {
                          "name": "add",
                          "nodeType": "YulIdentifier",
                          "src": "741:3:1"
                        },
                        "nodeType": "YulFunctionCall",
                        "src": "741:17:1"
                      }
                    ],
                    "functionName": {
                      "name": "abi_encode_t_uint256_to_t_uint256_fromStack",
                      "nodeType": "YulIdentifier",
                      "src": "688:43:1"
                    },
                    "nodeType": "YulFunctionCall",
                    "src": "688:71:1"
                  },
                  "nodeType": "YulExpressionStatement",
                  "src": "688:71:1"
                }
              ]
            },
            "name": "abi_encode_tuple_t_uint256__to_t_uint256__fromStack_reversed",
            "nodeType": "YulFunctionDefinition",
            "parameters": [
              {
                "name": "headStart",
                "nodeType": "YulTypedName",
                "src": "614:9:1",
                "type": ""
              },
              {
                "name": "value0",
                "nodeType": "YulTypedName",
                "src": "626:6:1",
                "type": ""
              }
            ],
            "returnVariables": [
              {
                "name": "tail",
                "nodeType": "YulTypedName",
                "src": "637:4:1",
                "type": ""
              }
            ],
            "src": "544:222:1"
          },
          {
            "body": {
              "nodeType": "YulBlock",
              "src": "817:32:1",
              "statements": [
                {
                  "nodeType": "YulAssignment",
                  "src": "827:16:1",
                  "value": {
                    "name": "value",
                    "nodeType": "YulIdentifier",
                    "src": "838:5:1"
                  },
                  "variableNames": [
                    {
                      "name": "cleaned",
                      "nodeType": "YulIdentifier",
                      "src": "827:7:1"
                    }
                  ]
                }
              ]
            },
            "name": "cleanup_t_uint256",
            "nodeType": "YulFunctionDefinition",
            "parameters": [
              {
                "name": "value",
                "nodeType": "YulTypedName",
                "src": "799:5:1",
                "type": ""
              }
            ],
            "returnVariables": [
              {
                "name": "cleaned",
                "nodeType": "YulTypedName",
                "src": "809:7:1",
                "type": ""
              }
            ],
            "src": "772:77:1"
          },
          {
            "body": {
              "nodeType": "YulBlock",
              "src": "898:79:1",
              "statements": [
                {
                  "body": {
                    "nodeType": "YulBlock",
                    "src": "955:16:1",
                    "statements": [
                      {
                        "expression": {
                          "arguments": [
                            {
                              "kind": "number",
                              "nodeType": "YulLiteral",
                              "src": "964:1:1",
                              "type": "",
                              "value": "0"
                            },
                            {
                              "kind": "number",
                              "nodeType": "YulLiteral",
                              "src": "967:1:1",
                              "type": "",
                              "value": "0"
                            }
                          ],
                          "functionName": {
                            "name": "revert",
                            "nodeType": "YulIdentifier",
                            "src": "957:6:1"
                          },
                          "nodeType": "YulFunctionCall",
                          "src": "957:12:1"
                        },
                        "nodeType": "YulExpressionStatement",
                        "src": "957:12:1"
                      }
                    ]
                  },
                  "condition": {
                    "arguments": [
                      {
                        "arguments": [
                          {
                            "name": "value",
                            "nodeType": "YulIdentifier",
                            "src": "921:5:1"
                          },
                          {
                            "arguments": [
                              {
                                "name": "value",
                                "nodeType": "YulIdentifier",
                                "src": "946:5:1"
                              }
                            ],
                            "functionName": {
                              "name": "cleanup_t_uint256",
                              "nodeType": "YulIdentifier",
                              "src": "928:17:1"
                            },
                            "nodeType": "YulFunctionCall",
                            "src": "928:24:1"
                          }
                        ],
                        "functionName": {
                          "name": "eq",
                          "nodeType": "YulIdentifier",
                          "src": "918:2:1"
                        },
                        "nodeType": "YulFunctionCall",
                        "src": "918:35:1"
                      }
                    ],
                    "functionName": {
                      "name": "iszero",
                      "nodeType": "YulIdentifier",
                      "src": "911:6:1"
                    },
                    "nodeType": "YulFunctionCall",
                    "src": "911:43:1"
                  },
                  "nodeType": "YulIf",
                  "src": "908:2:1"
                }
              ]
            },
            "name": "validator_revert_t_uint256",
            "nodeType": "YulFunctionDefinition",
            "parameters": [
              {
                "name": "value",
                "nodeType": "YulTypedName",
                "src": "891:5:1",
                "type": ""
              }
            ],
            "src": "855:122:1"
          }
        ]
      },
      "contents": "{\n\n    function abi_decode_t_uint256(offset, end) -> value {\n        value := calldataload(offset)\n        validator_revert_t_uint256(value)\n    }\n\n    function abi_decode_tuple_t_uint256(headStart, dataEnd) -> value0 {\n        if slt(sub(dataEnd, headStart), 32) { revert(0, 0) }\n\n        {\n\n            let offset := 0\n\n            value0 := abi_decode_t_uint256(add(headStart, offset), dataEnd)\n        }\n\n    }\n\n    function abi_encode_t_uint256_to_t_uint256_fromStack(value, pos) {\n        mstore(pos, cleanup_t_uint256(value))\n    }\n\n    function abi_encode_tuple_t_uint256__to_t_uint256__fromStack_reversed(headStart , value0) -> tail {\n        tail := add(headStart, 32)\n\n        abi_encode_t_uint256_to_t_uint256_fromStack(value0,  add(headStart, 0))\n\n    }\n\n    function cleanup_t_uint256(value) -> cleaned {\n        cleaned := value\n    }\n\n    function validator_revert_t_uint256(value) {\n        if iszero(eq(value, cleanup_t_uint256(value))) { revert(0, 0) }\n    }\n\n}\n",
      "id": 1,
      "language": "Yul",
      "name": "#utility.yul"
    }
  ],
  "sourceMap": "28:251:0:-:0;;;120:3;107:10;:16;;;;28:251;;;;;;",
  "deployedSourceMap": "28:251:0:-:0;;;;;;;;;;;;;;;;;;;;;;;;;;135:63;;;;;;;;;;;;;:::i;:::-;;:::i;:::-;;204:72;;;;;;;;;;;;;:::i;:::-;;;;;;;:::i;:::-;;;;;;;;135:63;191:1;178:10;:14;;;;135:63;:::o;204:72::-;240:4;260:10;;253:17;;204:72;:::o;7:139:1:-;;91:6;78:20;69:29;;107:33;134:5;107:33;:::i;:::-;59:87;;;;:::o;152:262::-;;260:2;248:9;239:7;235:23;231:32;228:2;;;276:1;273;266:12;228:2;319:1;344:53;389:7;380:6;369:9;365:22;344:53;:::i;:::-;334:63;;290:117;218:196;;;;:::o;420:118::-;507:24;525:5;507:24;:::i;:::-;502:3;495:37;485:53;;:::o;544:222::-;;675:2;664:9;660:18;652:26;;688:71;756:1;745:9;741:17;732:6;688:71;:::i;:::-;642:124;;;;:::o;772:77::-;;838:5;827:16;;817:32;;;:::o;855:122::-;928:24;946:5;928:24;:::i;:::-;921:5;918:35;908:2;;967:1;964;957:12;908:2;898:79;:::o",
  "source": "pragma solidity >=0.8.0;\r\n\r\ncontract SimpleStorage {\r\n  uint storedData;\r\n\r\n  constructor() payable {\r\n    storedData = 123;\r\n  }\r\n\r\n  function set(uint x) public payable {\r\n    storedData = x;\r\n  }\r\n\r\n  function get() public view returns (uint) {\r\n    return storedData;\r\n  }\r\n}",
  "sourcePath": "C:/Users/nervous/Desktop/test/blockchain-workshop-ethereum-simple/contracts/SimpleStorage.sol",
  "ast": {
    "absolutePath": "/C/Users/nervous/Desktop/test/blockchain-workshop-ethereum-simple/contracts/SimpleStorage.sol",
    "exportedSymbols": {
      "SimpleStorage": [
        30
      ]
    },
    "id": 31,
    "nodeType": "SourceUnit",
    "nodes": [
      {
        "id": 1,
        "literals": [
          "solidity",
          ">=",
          "0.8",
          ".0"
        ],
        "nodeType": "PragmaDirective",
        "src": "0:24:0"
      },
      {
        "abstract": false,
        "baseContracts": [],
        "contractDependencies": [],
        "contractKind": "contract",
        "fullyImplemented": true,
        "id": 30,
        "linearizedBaseContracts": [
          30
        ],
        "name": "SimpleStorage",
        "nameLocation": "37:13:0",
        "nodeType": "ContractDefinition",
        "nodes": [
          {
            "constant": false,
            "id": 3,
            "mutability": "mutable",
            "name": "storedData",
            "nameLocation": "61:10:0",
            "nodeType": "VariableDeclaration",
            "scope": 30,
            "src": "56:15:0",
            "stateVariable": true,
            "storageLocation": "default",
            "typeDescriptions": {
              "typeIdentifier": "t_uint256",
              "typeString": "uint256"
            },
            "typeName": {
              "id": 2,
              "name": "uint",
              "nodeType": "ElementaryTypeName",
              "src": "56:4:0",
              "typeDescriptions": {
                "typeIdentifier": "t_uint256",
                "typeString": "uint256"
              }
            },
            "visibility": "internal"
          },
          {
            "body": {
              "id": 10,
              "nodeType": "Block",
              "src": "100:29:0",
              "statements": [
                {
                  "expression": {
                    "id": 8,
                    "isConstant": false,
                    "isLValue": false,
                    "isPure": false,
                    "lValueRequested": false,
                    "leftHandSide": {
                      "id": 6,
                      "name": "storedData",
                      "nodeType": "Identifier",
                      "overloadedDeclarations": [],
                      "referencedDeclaration": 3,
                      "src": "107:10:0",
                      "typeDescriptions": {
                        "typeIdentifier": "t_uint256",
                        "typeString": "uint256"
                      }
                    },
                    "nodeType": "Assignment",
                    "operator": "=",
                    "rightHandSide": {
                      "hexValue": "313233",
                      "id": 7,
                      "isConstant": false,
                      "isLValue": false,
                      "isPure": true,
                      "kind": "number",
                      "lValueRequested": false,
                      "nodeType": "Literal",
                      "src": "120:3:0",
                      "typeDescriptions": {
                        "typeIdentifier": "t_rational_123_by_1",
                        "typeString": "int_const 123"
                      },
                      "value": "123"
                    },
                    "src": "107:16:0",
                    "typeDescriptions": {
                      "typeIdentifier": "t_uint256",
                      "typeString": "uint256"
                    }
                  },
                  "id": 9,
                  "nodeType": "ExpressionStatement",
                  "src": "107:16:0"
                }
              ]
            },
            "id": 11,
            "implemented": true,
            "kind": "constructor",
            "modifiers": [],
            "name": "",
            "nameLocation": "-1:-1:-1",
            "nodeType": "FunctionDefinition",
            "parameters": {
              "id": 4,
              "nodeType": "ParameterList",
              "parameters": [],
              "src": "89:2:0"
            },
            "returnParameters": {
              "id": 5,
              "nodeType": "ParameterList",
              "parameters": [],
              "src": "100:0:0"
            },
            "scope": 30,
            "src": "78:51:0",
            "stateMutability": "payable",
            "virtual": false,
            "visibility": "public"
          },
          {
            "body": {
              "id": 20,
              "nodeType": "Block",
              "src": "171:27:0",
              "statements": [
                {
                  "expression": {
                    "id": 18,
                    "isConstant": false,
                    "isLValue": false,
                    "isPure": false,
                    "lValueRequested": false,
                    "leftHandSide": {
                      "id": 16,
                      "name": "storedData",
                      "nodeType": "Identifier",
                      "overloadedDeclarations": [],
                      "referencedDeclaration": 3,
                      "src": "178:10:0",
                      "typeDescriptions": {
                        "typeIdentifier": "t_uint256",
                        "typeString": "uint256"
                      }
                    },
                    "nodeType": "Assignment",
                    "operator": "=",
                    "rightHandSide": {
                      "id": 17,
                      "name": "x",
                      "nodeType": "Identifier",
                      "overloadedDeclarations": [],
                      "referencedDeclaration": 13,
                      "src": "191:1:0",
                      "typeDescriptions": {
                        "typeIdentifier": "t_uint256",
                        "typeString": "uint256"
                      }
                    },
                    "src": "178:14:0",
                    "typeDescriptions": {
                      "typeIdentifier": "t_uint256",
                      "typeString": "uint256"
                    }
                  },
                  "id": 19,
                  "nodeType": "ExpressionStatement",
                  "src": "178:14:0"
                }
              ]
            },
            "functionSelector": "60fe47b1",
            "id": 21,
            "implemented": true,
            "kind": "function",
            "modifiers": [],
            "name": "set",
            "nameLocation": "144:3:0",
            "nodeType": "FunctionDefinition",
            "parameters": {
              "id": 14,
              "nodeType": "ParameterList",
              "parameters": [
                {
                  "constant": false,
                  "id": 13,
                  "mutability": "mutable",
                  "name": "x",
                  "nameLocation": "153:1:0",
                  "nodeType": "VariableDeclaration",
                  "scope": 21,
                  "src": "148:6:0",
                  "stateVariable": false,
                  "storageLocation": "default",
                  "typeDescriptions": {
                    "typeIdentifier": "t_uint256",
                    "typeString": "uint256"
                  },
                  "typeName": {
                    "id": 12,
                    "name": "uint",
                    "nodeType": "ElementaryTypeName",
                    "src": "148:4:0",
                    "typeDescriptions": {
                      "typeIdentifier": "t_uint256",
                      "typeString": "uint256"
                    }
                  },
                  "visibility": "internal"
                }
              ],
              "src": "147:8:0"
            },
            "returnParameters": {
              "id": 15,
              "nodeType": "ParameterList",
              "parameters": [],
              "src": "171:0:0"
            },
            "scope": 30,
            "src": "135:63:0",
            "stateMutability": "payable",
            "virtual": false,
            "visibility": "public"
          },
          {
            "body": {
              "id": 28,
              "nodeType": "Block",
              "src": "246:30:0",
              "statements": [
                {
                  "expression": {
                    "id": 26,
                    "name": "storedData",
                    "nodeType": "Identifier",
                    "overloadedDeclarations": [],
                    "referencedDeclaration": 3,
                    "src": "260:10:0",
                    "typeDescriptions": {
                      "typeIdentifier": "t_uint256",
                      "typeString": "uint256"
                    }
                  },
                  "functionReturnParameters": 25,
                  "id": 27,
                  "nodeType": "Return",
                  "src": "253:17:0"
                }
              ]
            },
            "functionSelector": "6d4ce63c",
            "id": 29,
            "implemented": true,
            "kind": "function",
            "modifiers": [],
            "name": "get",
            "nameLocation": "213:3:0",
            "nodeType": "FunctionDefinition",
            "parameters": {
              "id": 22,
              "nodeType": "ParameterList",
              "parameters": [],
              "src": "216:2:0"
            },
            "returnParameters": {
              "id": 25,
              "nodeType": "ParameterList",
              "parameters": [
                {
                  "constant": false,
                  "id": 24,
                  "mutability": "mutable",
                  "name": "",
                  "nameLocation": "-1:-1:-1",
                  "nodeType": "VariableDeclaration",
                  "scope": 29,
                  "src": "240:4:0",
                  "stateVariable": false,
                  "storageLocation": "default",
                  "typeDescriptions": {
                    "typeIdentifier": "t_uint256",
                    "typeString": "uint256"
                  },
                  "typeName": {
                    "id": 23,
                    "name": "uint",
                    "nodeType": "ElementaryTypeName",
                    "src": "240:4:0",
                    "typeDescriptions": {
                      "typeIdentifier": "t_uint256",
                      "typeString": "uint256"
                    }
                  },
                  "visibility": "internal"
                }
              ],
              "src": "239:6:0"
            },
            "scope": 30,
            "src": "204:72:0",
            "stateMutability": "view",
            "virtual": false,
            "visibility": "public"
          }
        ],
        "scope": 31,
        "src": "28:251:0"
      }
    ],
    "src": "0:279:0"
  },
  "legacyAST": {
    "absolutePath": "/C/Users/nervous/Desktop/test/blockchain-workshop-ethereum-simple/contracts/SimpleStorage.sol",
    "exportedSymbols": {
      "SimpleStorage": [
        30
      ]
    },
    "id": 31,
    "nodeType": "SourceUnit",
    "nodes": [
      {
        "id": 1,
        "literals": [
          "solidity",
          ">=",
          "0.8",
          ".0"
        ],
        "nodeType": "PragmaDirective",
        "src": "0:24:0"
      },
      {
        "abstract": false,
        "baseContracts": [],
        "contractDependencies": [],
        "contractKind": "contract",
        "fullyImplemented": true,
        "id": 30,
        "linearizedBaseContracts": [
          30
        ],
        "name": "SimpleStorage",
        "nameLocation": "37:13:0",
        "nodeType": "ContractDefinition",
        "nodes": [
          {
            "constant": false,
            "id": 3,
            "mutability": "mutable",
            "name": "storedData",
            "nameLocation": "61:10:0",
            "nodeType": "VariableDeclaration",
            "scope": 30,
            "src": "56:15:0",
            "stateVariable": true,
            "storageLocation": "default",
            "typeDescriptions": {
              "typeIdentifier": "t_uint256",
              "typeString": "uint256"
            },
            "typeName": {
              "id": 2,
              "name": "uint",
              "nodeType": "ElementaryTypeName",
              "src": "56:4:0",
              "typeDescriptions": {
                "typeIdentifier": "t_uint256",
                "typeString": "uint256"
              }
            },
            "visibility": "internal"
          },
          {
            "body": {
              "id": 10,
              "nodeType": "Block",
              "src": "100:29:0",
              "statements": [
                {
                  "expression": {
                    "id": 8,
                    "isConstant": false,
                    "isLValue": false,
                    "isPure": false,
                    "lValueRequested": false,
                    "leftHandSide": {
                      "id": 6,
                      "name": "storedData",
                      "nodeType": "Identifier",
                      "overloadedDeclarations": [],
                      "referencedDeclaration": 3,
                      "src": "107:10:0",
                      "typeDescriptions": {
                        "typeIdentifier": "t_uint256",
                        "typeString": "uint256"
                      }
                    },
                    "nodeType": "Assignment",
                    "operator": "=",
                    "rightHandSide": {
                      "hexValue": "313233",
                      "id": 7,
                      "isConstant": false,
                      "isLValue": false,
                      "isPure": true,
                      "kind": "number",
                      "lValueRequested": false,
                      "nodeType": "Literal",
                      "src": "120:3:0",
                      "typeDescriptions": {
                        "typeIdentifier": "t_rational_123_by_1",
                        "typeString": "int_const 123"
                      },
                      "value": "123"
                    },
                    "src": "107:16:0",
                    "typeDescriptions": {
                      "typeIdentifier": "t_uint256",
                      "typeString": "uint256"
                    }
                  },
                  "id": 9,
                  "nodeType": "ExpressionStatement",
                  "src": "107:16:0"
                }
              ]
            },
            "id": 11,
            "implemented": true,
            "kind": "constructor",
            "modifiers": [],
            "name": "",
            "nameLocation": "-1:-1:-1",
            "nodeType": "FunctionDefinition",
            "parameters": {
              "id": 4,
              "nodeType": "ParameterList",
              "parameters": [],
              "src": "89:2:0"
            },
            "returnParameters": {
              "id": 5,
              "nodeType": "ParameterList",
              "parameters": [],
              "src": "100:0:0"
            },
            "scope": 30,
            "src": "78:51:0",
            "stateMutability": "payable",
            "virtual": false,
            "visibility": "public"
          },
          {
            "body": {
              "id": 20,
              "nodeType": "Block",
              "src": "171:27:0",
              "statements": [
                {
                  "expression": {
                    "id": 18,
                    "isConstant": false,
                    "isLValue": false,
                    "isPure": false,
                    "lValueRequested": false,
                    "leftHandSide": {
                      "id": 16,
                      "name": "storedData",
                      "nodeType": "Identifier",
                      "overloadedDeclarations": [],
                      "referencedDeclaration": 3,
                      "src": "178:10:0",
                      "typeDescriptions": {
                        "typeIdentifier": "t_uint256",
                        "typeString": "uint256"
                      }
                    },
                    "nodeType": "Assignment",
                    "operator": "=",
                    "rightHandSide": {
                      "id": 17,
                      "name": "x",
                      "nodeType": "Identifier",
                      "overloadedDeclarations": [],
                      "referencedDeclaration": 13,
                      "src": "191:1:0",
                      "typeDescriptions": {
                        "typeIdentifier": "t_uint256",
                        "typeString": "uint256"
                      }
                    },
                    "src": "178:14:0",
                    "typeDescriptions": {
                      "typeIdentifier": "t_uint256",
                      "typeString": "uint256"
                    }
                  },
                  "id": 19,
                  "nodeType": "ExpressionStatement",
                  "src": "178:14:0"
                }
              ]
            },
            "functionSelector": "60fe47b1",
            "id": 21,
            "implemented": true,
            "kind": "function",
            "modifiers": [],
            "name": "set",
            "nameLocation": "144:3:0",
            "nodeType": "FunctionDefinition",
            "parameters": {
              "id": 14,
              "nodeType": "ParameterList",
              "parameters": [
                {
                  "constant": false,
                  "id": 13,
                  "mutability": "mutable",
                  "name": "x",
                  "nameLocation": "153:1:0",
                  "nodeType": "VariableDeclaration",
                  "scope": 21,
                  "src": "148:6:0",
                  "stateVariable": false,
                  "storageLocation": "default",
                  "typeDescriptions": {
                    "typeIdentifier": "t_uint256",
                    "typeString": "uint256"
                  },
                  "typeName": {
                    "id": 12,
                    "name": "uint",
                    "nodeType": "ElementaryTypeName",
                    "src": "148:4:0",
                    "typeDescriptions": {
                      "typeIdentifier": "t_uint256",
                      "typeString": "uint256"
                    }
                  },
                  "visibility": "internal"
                }
              ],
              "src": "147:8:0"
            },
            "returnParameters": {
              "id": 15,
              "nodeType": "ParameterList",
              "parameters": [],
              "src": "171:0:0"
            },
            "scope": 30,
            "src": "135:63:0",
            "stateMutability": "payable",
            "virtual": false,
            "visibility": "public"
          },
          {
            "body": {
              "id": 28,
              "nodeType": "Block",
              "src": "246:30:0",
              "statements": [
                {
                  "expression": {
                    "id": 26,
                    "name": "storedData",
                    "nodeType": "Identifier",
                    "overloadedDeclarations": [],
                    "referencedDeclaration": 3,
                    "src": "260:10:0",
                    "typeDescriptions": {
                      "typeIdentifier": "t_uint256",
                      "typeString": "uint256"
                    }
                  },
                  "functionReturnParameters": 25,
                  "id": 27,
                  "nodeType": "Return",
                  "src": "253:17:0"
                }
              ]
            },
            "functionSelector": "6d4ce63c",
            "id": 29,
            "implemented": true,
            "kind": "function",
            "modifiers": [],
            "name": "get",
            "nameLocation": "213:3:0",
            "nodeType": "FunctionDefinition",
            "parameters": {
              "id": 22,
              "nodeType": "ParameterList",
              "parameters": [],
              "src": "216:2:0"
            },
            "returnParameters": {
              "id": 25,
              "nodeType": "ParameterList",
              "parameters": [
                {
                  "constant": false,
                  "id": 24,
                  "mutability": "mutable",
                  "name": "",
                  "nameLocation": "-1:-1:-1",
                  "nodeType": "VariableDeclaration",
                  "scope": 29,
                  "src": "240:4:0",
                  "stateVariable": false,
                  "storageLocation": "default",
                  "typeDescriptions": {
                    "typeIdentifier": "t_uint256",
                    "typeString": "uint256"
                  },
                  "typeName": {
                    "id": 23,
                    "name": "uint",
                    "nodeType": "ElementaryTypeName",
                    "src": "240:4:0",
                    "typeDescriptions": {
                      "typeIdentifier": "t_uint256",
                      "typeString": "uint256"
                    }
                  },
                  "visibility": "internal"
                }
              ],
              "src": "239:6:0"
            },
            "scope": 30,
            "src": "204:72:0",
            "stateMutability": "view",
            "virtual": false,
            "visibility": "public"
          }
        ],
        "scope": 31,
        "src": "28:251:0"
      }
    ],
    "src": "0:279:0"
  },
  "compiler": {
    "name": "solc",
    "version": "0.8.3+commit.8d00100c.Linux.g++"
  },
  "networks": {},
  "schemaVersion": "3.3.4",
  "updatedAt": "2021-08-06T14:50:38.404Z",
  "devdoc": {
    "kind": "dev",
    "methods": {},
    "version": 1
  },
  "userdoc": {
    "kind": "user",
    "methods": {},
    "version": 1
  }
}
```
