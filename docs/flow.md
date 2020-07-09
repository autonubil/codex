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

flow.meter.proc.pid
flow.meter.proc.start.timestamp
flow.meter.proc.end.timestamp

flow.meter.class.id
flow.meter.class.name
flow.meter.class.engine.id
flow.meter.class.engine.name

flow.meter.flow_timeout.active
flow.meter.flow_timeout.idle

flow.meter.observ.domain.id
flow.meter.observ.orig_domain.id
flow.meter.observ.domain.name
flow.meter.observ.point.id
flow.meter.observ.point.type.id
flow.meter.observ.point.type.name
flow.meter.observ.timestamp
flow.meter.observ.flows
flow.meter.observ.conns
flow.meter.observ.conn_duration_sum

flow.meter.select.id
flow.meter.select.id_flow_flags
flow.meter.select.name
flow.meter.select.seq_id

flow.meter.select.observed.packets_total
flow.meter.select.observed.flows_total
flow.meter.select.selected.packets_total
flow.meter.select.selected.flows_total

flow.meter.packet_select.algo.id
flow.meter.packet_select.algo.name
flow.meter.packet_select.interval.packets
flow.meter.packet_select.size.packets
flow.meter.packet_select.size.time
flow.meter.packet_select.gap.packets
flow.meter.packet_select.gap.time

flow.meter.flow_select.algo.id
flow.meter.flow_select.algo.name
flow.meter.flow_select.size.flows
flow.meter.flow_select.size.time
flow.meter.flow_select.gap.flows
flow.meter.flow_select.gap.time
flow.meter.flow_select.flows
flow.meter.flow_select.bytes
flow.meter.flow_select.packets

flow.meter.random_sample.size.packets
flow.meter.random_sample.population.packets

flow.meter.uniprob_sample.probability

flow.meter.hash_select.flow_domain
flow.meter.hash_select.digest.hash
flow.meter.hash_select.ip_payload.offset
flow.meter.hash_select.ip_payload.size
flow.meter.hash_select.observed.range.min
flow.meter.hash_select.observed.range.max
flow.meter.hash_select.selected.range.min
flow.meter.hash_select.selected.range.max
flow.meter.hash_select.digest.output
flow.meter.hash_select.func.initializer

flow.meter.first.timestamp
flow.meter.last.timestamp

flow.meter.records_ignore
flow.meter.bytes_ignore
flow.meter.packets_ignore
flow.meter.l2.frames_ignore
flow.meter.l2.bytes_ignore

flow.meter.records_drop
flow.meter.bytes_drop
flow.meter.packets_drop
flow.meter.l2.frames_drop
flow.meter.l2.bytes_drop


flow.export.engine.id
flow.export.engine.type.id
flow.export.engine.type.name
flow.export.start.timestamp

flow.export.proc.pid
flow.export.flow_version

flow.export.ip.addr {ip}
flow.export.orig_ip.addr {ip}
flow.export.host {host}
flow.export.netif.index
flow.export.netif.name
flow.export.ip.proto
flow.export.l4.port"
flow.export.sctp.stream_id
flow.export.sctp.data_record_reliability

flow.export.first.timestamp
flow.export.last.timestamp

flow.export.flows
flow.export.bytes
flow.export.msgs


flow.collect.ip.addr
flow.collect.l4.port
flow.collect.timestamp
