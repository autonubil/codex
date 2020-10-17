# end-to-end metrics

conns
conn_rate

reqs
req_rate

resps
resps_late
resp_rate

.latency
.latency_sum
.latency_avg
.latency_min
.latency_max
.latency_stddev
.latency_sumsqrs
.latency_var

.jitter
.jitter_sum
.jitter_avg
.jitter_min
.jitter_max
.jitter_stddev
.jitter_sumsqrs
.jitter_var

.samples

req. (network client to server)
req.latency
req.latency_sum
req.latency_avg
req.latency_min
req.latency_max
req.latency_stddev
req.latency_sumsqrs
req.latency_var
req.samples

resp. (network server to client)
resp.latency
resp.latency_sum
resp.latency_avg
resp.latency_min
resp.latency_max
resp.latency_stddev
resp.latency_sumsqrs
resp.latency_var
resp.samples

network. (network client to server + network server to client)
network.latency
network.latency_sum
network.latency_avg
network.latency_min
network.latency_max
network.latency_stddev
network.latency_sumsqrs
network.latency_var
network.samples

svc. (service/application server-side)
svc.latency
svc.latency_sum
svc.latency_avg
svc.latency_min
svc.latency_max
svc.latency_stddev
svc.latency_sumsqrs
svc.latency_var
svc.samples

oneway. (round-trip client to server+app to client)
oneway.latency
oneway.latency_sum
oneway.latency_avg
oneway.latency_min
oneway.latency_max
oneway.latency_stddev
oneway.latency_sumsqrs
oneway.latency_var
oneway.samples

rndtrip. (round-trip client to server+app to client)
rndtrip.latency
rndtrip.latency_sum
rndtrip.latency_avg
rndtrip.latency_min
rndtrip.latency_max
rndtrip.latency_stddev
rndtrip.latency_sumsqrs
rndtrip.latency_var
rndtrip.samples

transact. (initial client req to final resp)
transact.latency
transact.latency_sum
transact.latency_avg
transact.latency_min
transact.latency_max
transact.latency_stddev
transact.latency_sumsqrs
transact.latency_var
transact.samples
