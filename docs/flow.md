# `flow`

flow.
flow.src.ip [ip]
flow.src.host [host]
flow.dst.ip [ip]
flow.dst.host [host]
flow.client.ip [ip]
flow.client.host [host]
flow.server.ip [ip]
flow.server.host [host]
flow.next_hop.ip [ip]
flow.next_hop.host [host]

flow.in.ip [ip]
flow.out.ip [ip]

flow.first.
flow.last.


flow.common_props
flow.direction.id
flow.direction.name
flow.flows
flow.forwarding_status
flow.id
flow.padding_size
flow.key_indicator
flow.biflow.direction.id
flow.biflow.direction.name
flow.opaque_octets
flow.l4.session_scope
flow.transact.id
flow.basic_list
flow.sub_template_list
flow.sub_template_multiList
flow.md5_checksum
flow.confidence.limit.upper
flow.confidence.limit.lower
flow.confidence.level
flow.error.absolute
flow.error.relative

flow.start.sysuptime
flow.start.timestamp
flow.start.time_offset

flow.end.sysuptime
flow.end.timestamp
flow.end.time_offset
flow.end.reason.id
flow.end.reason.name

flow.duration

flow.agg.flows
flow.agg.flows_started
flow.agg.flows_ended
flow.agg.src.unique_ip_addrs
flow.agg.dst.unique_ip_addrs
flow.agg.src.unique_ipv4_addrs
flow.agg.dst.unique_ipv4_addrs
flow.agg.src.unique_ipv6_addrs
flow.agg.dst.unique_ipv6_addrs
flow.agg.value_dist_method

flow.template.id
flow.template.ie.index
flow.template.ie.id
flow.template.ie.data_type
flow.template.ie.descr
flow.template.ie.name
flow.template.ie.range.start
flow.template.ie.range.end
flow.template.ie.semantic
flow.template.ie.unit
flow.template.ie.pen
flow.template.anonym.flags
flow.template.anonym.flag.sc.id
flow.template.anonym.flag.sc.name
flow.template.anonym.flag.pma
flow.template.anonym.flag.lor
flow.template.anonym.tech.id
flow.template.anonym.tech.name
flow.template.option_scope

meter.proc.pid
meter.proc.start.timestamp
meter.proc.end.timestamp

meter.class.id
meter.class.name
meter.class.engine.id
meter.class.engine.name

meter.flow_timeout.active
meter.flow_timeout.idle

meter.observ.domain.id
meter.observ.orig_domain.id
meter.observ.domain.name
meter.observ.point.id
meter.observ.point.type.id
meter.observ.point.type.name
meter.observ.timestamp
meter.observ.flows
meter.observ.conns
meter.observ.conn_duration_sum

meter.select.id
meter.select.id_flow_flags
meter.select.name
meter.select.seq_id

meter.select.observed.packets_total
meter.select.observed.flows_total
meter.select.selected.packets_total
meter.select.selected.flows_total

meter.packet_select.algo.id
meter.packet_select.algo.name
meter.packet_select.interval.packets
meter.packet_select.size.packets
meter.packet_select.size.time
meter.packet_select.gap.packets
meter.packet_select.gap.time

meter.flow_select.algo.id
meter.flow_select.algo.name
meter.flow_select.size.flows
meter.flow_select.size.time
meter.flow_select.gap.flows
meter.flow_select.gap.time
meter.flow_select.flows
meter.flow_select.bytes
meter.flow_select.packets

meter.random_sample.size.packets
meter.random_sample.population.packets

meter.uniprob_sample.probability

meter.hash_select.flow_domain
meter.hash_select.digest.hash
meter.hash_select.ip_payload.offset
meter.hash_select.ip_payload.size
meter.hash_select.observed.range.min
meter.hash_select.observed.range.max
meter.hash_select.selected.range.min
meter.hash_select.selected.range.max
meter.hash_select.digest.output
meter.hash_select.func.initializer

meter.first.timestamp
meter.last.timestamp

meter.records_ignore
meter.bytes_ignore
meter.packets_ignore
meter.l2.frames_ignore
meter.l2.bytes_ignore

meter.records_drop
meter.bytes_drop
meter.packets_drop
meter.l2.frames_drop
meter.l2.bytes_drop

export.proc.pid
export.flow_version

export.ip.addr {ip}
export.orig_ip.addr {ip}
export.host {host}
export.netif.index
export.netif.name
export.ip.proto
export.l4.port"
export.sctp.stream_id
export.sctp.data_record_reliability

export.first.timestamp
export.last.timestamp

export.flows
export.bytes
export.msgs


collect.ip.addr
collect.l4.port
collect.timestamp

system.engine.id
system.engine.type.id
system.engine.type.name
system.start.timestamp

