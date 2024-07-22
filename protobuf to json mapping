
## Protobuff to Json Mapping
# Protobuf to JSON Conversion Examples

This document provides examples of converting Protocol Buffers (protobuf) messages to their corresponding JSON formats. Each example showcases different features of protobuf, such as simple messages, nested messages, repeated fields, enum fields, and map fields.

## Example 1: Simple Message

### Protobuf Definition
```proto
syntax = "proto3";

message User {
  string id = 1;
  string name = 2;
  string email = 3;
}
{
  "id": "123",
  "name": "John Doe",
  "email": "johndoe@example.com"
}
```
## Example 2
```
syntax = "proto3";

message Address {
  string street = 1;
  string city = 2;
  string state = 3;
  string zip = 4;
}

message User {
  string id = 1;
  string name = 2;
  Address address = 3;
}
{
  "id": "123",
  "name": "John Doe",
  "address": {
    "street": "123 Main St",
    "city": "Anytown",
    "state": "CA",
    "zip": "12345"
  }
}
```
## Example 3
```
syntax = "proto3";

message PhoneNumber {
  string number = 1;
  string type = 2;
}

message User {
  string id = 1;
  string name = 2;
  repeated PhoneNumber phone_numbers = 3;
}
{
  "id": "123",
  "name": "John Doe",
  "phone_numbers": [
    {
      "number": "555-1234",
      "type": "home"
    },
    {
      "number": "555-5678",
      "type": "work"
    }
  ]
}
```
### Example 4
```
syntax = "proto3";

enum Status {
  ACTIVE = 0;
  INACTIVE = 1;
  BANNED = 2;
}

message User {
  string id = 1;
  string name = 2;
  Status status = 3;
}
{
  "id": "123",
  "name": "John Doe",
  "status": "ACTIVE"
}
```
### Example 5
```
syntax = "proto3";

message PhoneNumber {
  string number = 1;
  string type = 2;
}

message User {
  string id = 1;
  string name = 2;
  repeated PhoneNumber phone_numbers = 3;
}
{
  "id": "123",
  "name": "John Doe",
  "phone_numbers": [
    {
      "number": "555-1234",
      "type": "home"
    },
    {
      "number": "555-5678",
      "type": "work"
    }
  ]
}
```
