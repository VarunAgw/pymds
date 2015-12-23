An authoritative-only DNS server with a pluggable architecture for determining how to resolve each request. New modules may be written in Python to control how names are resolved.

This has been the authoritative server for my blog for several months now without problem.

Included:

  * authoritative server able to serve multiple zones concurrently
  * zones currently loaded from simple zone files
  * able to refresh data from zone files without restart
  * simple modular API for processing DNS requests by writing python plugins

Planned:

  * more plugins: health check for load balancing across servers or datacenters and rr load balancing

Not planned:

  * resolver functionality
  * zone transfers