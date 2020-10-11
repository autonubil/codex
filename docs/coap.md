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
coap.class.id
coap.class.name
coap.req.method.id
coap.req.method.name
coap.resp.code.id
coap.resp.code.name
coap.msg_id
coap.token.value
coap.options
coap.option []
coap.option.delta
coap.option.delta_ext
coap.option.size
coap.option.size_ext
coap.option.value
coap.option.if_match
coap.option.uri.host.name
coap.option.etag
coap.option.if_none_match
coap.option.uri.port
coap.option.location_path
coap.option.uri.path
coap.option.content_format
coap.option.max_age
coap.option.uri.query
coap.option.accept
coap.option.location_query
coap.option.proxy.uri.ref
coap.option.proxy_scheme
coap.option.size1
coap.payload
