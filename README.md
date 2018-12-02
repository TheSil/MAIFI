# Minesweeper AI Friendly Interface (MAIFI)
MAIFI is an interface specification of AI friendly interface for classic Minesweeper game. This is not an implementation, only specification to which specific Minesweeper implementations can become compliant to. It's use is meant for anyone who wants to test AI algorithms for Minesweeper and be able to easily interface a Minesweeper game without the need of writing UI interfacing layer (such as reading images, parsing pixels, etc...). This specification allows for standard API being included either in Minesweeper implementations themselves, or in a form of adapters (which can be nice exercise for those who indeed want to write their own UI interfacing layer). 

# API Format and protocol
All the requests and responses are done in [JSON](https://en.wikipedia.org/wiki/JSON) format. While main specification does not prescribe any specific means on how this JSON format is exchanged (a transport protocol), it includes an extension that describes two most common approaches which are expected to be used - the HTTP and UDP (see [Protocol Extensions](v1.md/#Protocol-Extensions)).  For example for desktop applications this can be by Network TCP/IP sockets, or through file, while for Web based application it can be through HTTP requests. This specification assumes that this layer has taken care of corresponding request/response matching and so it deals only with minimal content.

# Current version

Current version in progress is [1.0.0](v1.md).  

# Older versions

There is no older version yet.

# MAIFI compliant Minesweeper implementations
Currently there are no compliant implementations.