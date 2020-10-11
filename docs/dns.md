# DNS Information Elements

dns.version.ver
dns.payload_size
dns.name_server.ip.addr
dns.upstream_server.ip.addr
dns.hosts_file
dns.svc.latency
dns.rndtrip.latency

dns.tid
dns.qr.id
dns.qr.name
dns.opcode.id
dns.opcode.name
dns.flags.bits
dns.flags.tags
dns.flags.aa
dns.flags.tc
dns.flags.rd
dns.flags.ra
dns.flags.z
dns.flags.ad
dns.flags.cd
dns.rcode.id
dns.rcode.name

dns.queries
dns.answers
dns.authorities
dns.additionals
dns.zones
dns.prereqs
dns.updates

dns.query.name
dns.query.type.id
dns.query.type.name
dns.query.class.id
dns.query.class.name

dns.answer.name
dns.answer.type.id
dns.answer.type.name
dns.answer.class.id
dns.answer.class.name
dns.answer.ttl
dns.answer.rdlength
dns.answer.rdata
dns.answer.[DNSType].[RDATA-related]

dns.authority.name
dns.authority.type.id
dns.authority.type.name
dns.authority.class.id
dns.authority.class.name
dns.authority.ttl
dns.authority.rdlength
dns.authority.rdata
dns.authority.[DNSType].[RDATA-related]

dns.additional.name
dns.additional.type.id
dns.additional.type.name
dns.additional.class.id
dns.additional.class.name
dns.additional.ttl
dns.additional.rdlength
dns.additional.rdata
dns.additional.[DNSType].[RDATA-related]

a.rdata
a.ip.addr

a6.rdata
a6.prefix_size
a6.ipv6_suffix
a6.prefix_name

aaaa.rdata
aaaa.ip.addr

afsdb.rdata
afsdb.subtype.id
afsdb.subtype.name
afsdb.host (host)

amtrelay.rdata
amtrelay.prec
amtrelay.d
amtrelay.type.id
amtrelay.type.name
amtrelay.relay

apl.rdata
apl.addr_family
apl.prefix
apl.n
apl.afd_size
apl.afd_part

atma.rdata
atma.addr

avc.rdata

caa.rdata
caa.flags
caa.tag
caa.value

cdnskey (dns.definitions.key)
cdnskey.rdata
cdnskey.flags
cdnskey.proto.id
cdnskey.proto.name
cdnskey.algo.id
cdnskey.algo.name
cdnskey.pub_key

cds (dns.definitions.digest)
cds.rdata
cds.key_tag
cds.algo.id
cds.algo.name
cds.digest_type.id
cds.digest_type.name
cds.digest

cert.rdata
cert.cert_type.id
cert.cert_type.name
cert.key_tag
cert.algo.id
cert.algo.name
cert.cert

cname.rdata
cname.domain (host)

csync.rdata
csync.soa_serial
csync.flags.bits
csync.flags.tags
csync.flags.immediate
csync.flags.soaminimum
csync.type_bitmap

dhcid.rdata
dhcid.id_type.id
dhcid.id_type.name
dhcid.digest_type.id
dhcid.digest_type.name
dhcid.digest

dlv (dns.definitions.digest)
dlv.rdata
dlv.key_tag
dlv.algo.id
dlv.algo.name
dlv.digest_type.id
dlv.digest_type.name
dlv.digest

dname.rdata
dname.target (host)

dnskey (dns.definitions.key)
dnskey.rdata
dnskey.flags
dnskey.proto.id
dnskey.proto.name
dnskey.algo.id
dnskey.algo.name
dnskey.pub_key

doa.rdata
doa.pen.id
doa.pen.name
doa.type.id
doa.type.name
doa.location.id
doa.location.name
doa.media_type
doa.data

ds.rdata
ds.key_tag
ds.algo.id
ds.algo.name
ds.digest_type.id
ds.digest_type.name
ds.digest

eid.rdata
eid.id

eui48.rdata
eui48.addr

eui64.rdata
eui64.addr

gid.rdata

gpos.rdata
gpos.longitude
gpos.latitude
gpos.altitude

hinfo.rdata
hinfo.cpu
hinfo.os

hip.rdata
hip.algo.id
hip.algo.name
hip.pub_key_size
hip.hit
hip.pub_key
hip.rendezvous_server

ipseckey.rdata
ipseckey.prec
ipseckey.gw_type.id
ipseckey.gw_type.name
ipseckey.algo.id
ipseckey.algo.name
ipseckey.gw
ipseckey.pub_key

isdn.rdata
isdn.addr
isdn.subaddr

key (dns.definitions.key)
key.rdata
key.flags
key.proto.id
key.proto.name
key.algo.id
key.algo.name
key.pub_key

kx.rdata
kx.pref
kx.exch (host)

l32.rdata
l32.pref
l32.locator

l64.rdata
l64.pref
l64.locator

loc.rdata
loc.ver
loc.horiz_precision
loc.vert_precision
loc.latitude
loc.longitude
loc.altitude

lp.rdata
lp.pref
lp.fqdn (host)

mb.rdata
mb.domain (host)

md.rdata
md.domain (host)

mf.rdata
mf.domain (host)

mg.rdata
mg.domain (host)

minfo.rdata
minfo.rmailbx (host)
minfo.emailbx (host)

mr.rdata
mr.domain (host)

mx.rdata
mx.pref
mx.exch (host)

naptr.rdata
naptr.order
naptr.pref
naptr.flags
naptr.services
naptr.regex
naptr.replacement (host)

nid.rdata
nid.pref
nid.node_id

nimloc.rdata
nimloc.locator

ninfo.rdata
ninfo.zs_data

ns.rdata
ns.domain (host)

nsap.rdata
nsap.addr

nsap_ptr.rdata
nsap_ptr.domain (host)

nsec.rdata
nsec.domain_next (host)
nsec.type_bitmap

nsec3.rdata
nsec3.algo.id
nsec3.algo.name
nsec3.flags
nsec3.iterations
nsec3.salt_size
nsec3.salt
nsec3.hash_size
nsec3.next_hashed_owner
nsec3.type_bitmap

nsec3param.rdata
nsec3param.algo.id
nsec3param.algo.name
nsec3param.flags
nsec3param.iterations
nsec3param.salt_size
nsec3param.salt

null.rdata

nxt.rdata
nxt.next (host)
nxt.type_bitmap

openpgpkey.rdata
openpgpkey.key

opt.rdata
opt.code
opt.size
opt.data
opt.rcode_ext.id
opt.rcode_ext.name
opt.ver
opt.flags.do
opt.z

ptr.rdata
ptr.domain (host)

px.rdata
px.pref
px.map822 (host)
px.mapx400 (host)

rkey (dns.definitions.key)
rkey.rdata
rkey.flags
rkey.proto.id
rkey.proto.name
rkey.algo.id
rkey.algo.name
rkey.pub_key

rp.rdata
rp.mbox (host)
rp.txt (host)

rrsig.rdata
rrsig.type_covered
rrsig.algo_num
rrsig.labels
rrsig.ttl_orig
rrsig.expire_timestamp
rrsig.create_timestamp
rrsig.key_tag
rrsig.signer (host)
rrsig.signature

rt.rdata
rt.pref
rt.inter_host (host)

sig (signature)
sig.rdata
sig.type_covered
sig.algo.id
sig.algo.name
sig.labels
sig.ttl_orig
sig.expire_timestamp
sig.create_timestamp
sig.key_tag
sig.signer (host)
sig.signature

sink.rdata
sink.coding
sink.subcoding
sink.data

smimea.rdata
smimea.cert_usage.id
smimea.cert_usage.name
smimea.selector
smimea.match_type.id
smimea.match_type.name
smimea.cert_assoc_data

soa.rdata
soa.mname (host)
soa.rname (host)
soa.serial
soa.refresh_interval
soa.retry_interval
soa.expire_interval
soa.ttl_min

spf.rdata

srv.rdata
srv.prio
srv.weight
srv.port.id
srv.port.name
srv.target (host)

sshfp.rdata
sshfp.algo.id
sshfp.algo.name
sshfp.fingerprint_type.id
sshfp.fingerprint_type.name
sshfp.fingerprint

ta (dns.definitions.digest)
ta.rdata
ta.key_tag
ta.algo.id
ta.algo.name
ta.digest_type.id
ta.digest_type.name
ta.digest

talink.rdata
talink.prev (host)
talink.next (host)

tkey.rdata
tkey.algo.id
tkey.algo.name
tkey.create_timestamp
tkey.expire_timestamp
tkey.mode.id
tkey.mode.name
tkey.rcode_ext
tkey.key_size
tkey.key_data
tkey.other_size
tkey.other_data

tlsa.rdata
tlsa.cert_usage.id
tlsa.cert_usage.name
tlsa.selector
tlsa.match_type.id
tlsa.match_type.name
tlsa.cert_assoc_data

tsig.rdata
tsig.algo.id
tsig.algo.name
tsig.fudge
tsig.mac.size
tsig.mac.addr
tsig.orig_id
tsig.error
tsig.other_size
tsig.other_data

txt.rdata

uid.rdata

uinfo.rdata

unspec.rdata

uri.rdata
uri.prio
uri.weight
uri.target (host)

wins.rdata
wins.lookup_timeout
wins.cache_timeout
wins.server.ip.addr

wins_r.rdata
wins_r.lookup_timeout
wins_r.cache_timeout
wins_r.server.domain (host)

wks.rdata
wks.ip.addr
wks.l4.proto.id
wks.l4.proto.name
wks.bitmap

x25.rdata
x25.psdn.addr

xpf.rdata
xpf.ip.version.ver
xpf.l4.proto.id
xpf.l4.proto.name
xpf.src.ip.addr
xpf.src.l4.port.id
xpf.src.l4.port.name
xpf.dst.ip.addr
xpf.dst.l4.port.id
xpf.dst.l4.port.name

zonemd.rdata
zonemd.soa_serial
zonemd.digest_type.id
zonemd.digest_type.name
zonemd.digest
