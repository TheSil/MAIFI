# Minesweeper AI Friendly Interface (MAIFI)
MAIFI is an interface specification of AI friendly interface for classic Minesweeper game. This is not an implementation, only specification to which specific Minesweeper implementations can become compliant to. It's use is meant for anyone who wants to test AI algorithms for Minesweeper and be able to easily interface a Minesweeper game without the need of writing UI interfacing layer (such as reading images, parsing pixels, etc...). This specification allows for standard API being included either in Minesweeper implementations themselves, or in a form of adapters (which can be nice exercise for those who indeed want to write their own UI interfacing layer). 

The specification is currently work in progress (started on 12/02/2018), it is unstable and should not be followed (yet). 

# API Format and protocol
All the requests and responses are done in [JSON](https://en.wikipedia.org/wiki/JSON) format. This specification does not prescribe any specific means on how this JSON format is exchanged (transport protocol). For example for desktop applications this can be by Network TCP/IP sockets, or through file, while for Web based application it can be through HTTP requests. This specification assumes that this layer has taken care of corresponding request/response matching and so it deals only with minimal content.

# Version

Current version in progress is 1.0.0. There is no older version.

# Specification
The specification describes following messages:
- GetBoardInfo
- BoardInfo
- FlagField
- RevealField

## GetBoardInfo
Request for getting current board state information. 

TODO


## BoardInfo
It includes information about board layout, number of mines as well as individual fields state. Sent as a response to GetBoardInfo

TODO


## FlagField

Request to flag given field.

TODO

## RevealField
Request to revel given field.

TODO



# MAIFI compliant Minesweeper implementations
Currently there are no compliant implementations.