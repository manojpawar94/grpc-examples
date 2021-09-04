# Protocol Buffer

## Tag

In **Protocol Buffers**, field names are not important, whereas the field names are important in all programming language. In the **Protocol Buffers** the **Tag** tag name.

- Smallest tag : 1
- Largest tag : 2^29 - 1 or 536,870,911

The tags 19000 to 19999 are reserved by the Google. Hence you cannot use this tags in proto file. 

The tag numbered from 1 to 15 use 1 byte in space, so use them for more frequently populated fields to minimise the space. And the tag numbered from 16 to 2047 use 2 bytes.


## Default value

Each field if value is not set it has asscoiated default value.

Field Type|Default Value
---|---
bool | false
number | 0
string | empty string
list | empty list
enum | first value
repeated | empty list

There is no concept of required field or optional field in protocol buffer