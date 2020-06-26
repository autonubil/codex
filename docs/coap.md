# `coap`

Constrained Application Protocol (CoAP)

https://tools.ietf.org/html/rfc7252

 0                   1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|Ver| T |  TKL  |      Code     |          Message ID           |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|   Token (if any, TKL bytes) ...
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|   Options (if any) ...
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|1 1 1 1 1 1 1 1|    Payload (if any) ...
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

coap.version.ver
coap.type.id
coap.type.name
coap.token.size
coap.code.id
coap.code.name
coap.class.id
coap.class.name
coap.detail.id
coap.detail.name
coap.msg_id
coap.token
coap.options
coap.option []
coap.option.delta
coap.option.delta_ext
coap.option.size
coap.option.size_ext
coap.option.value
coap.option.if_match
coap.option.uri_host
coap.option.etag
coap.option.if_none_match
coap.option.uri_port
coap.option.location_path
coap.option.uri_path
coap.option.content_format
coap.option.max_age
coap.option.uri_query
coap.option.accept
coap.option.location_query
coap.option.proxy_uri
coap.option.proxy_scheme
coap.option.size1
coap.payload
