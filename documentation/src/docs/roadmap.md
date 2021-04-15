<!--
Copyright Pravega Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->
# Pravega Roadmap

The following will be the primary feature focus areas for our upcoming releases.

## Version 0.10
* Video analytics ([#4087](https://github.com/pravega/pravega/issues/4087))
    * Rust client
    * Support large events <=1GB ([PDP 43](https://github.com/pravega/pravega/wiki/PDP-43-Large-Events), [#5056](https://github.com/pravega/pravega/issues/5056))
* Security
    * TLS 1.3
* Serviceability
    * Disaster Recovery
    * Health Check ([PDP 45](https://github.com/pravega/pravega/wiki/PDP-45-Pravega-Healthcheck), [#5046](https://github.com/pravega/pravega/issues/5046), [#5098](https://github.com/pravega/pravega/issues/5098))
    * Improved metrics & logging
* Performance
    * Transactions
    * Read performance (tail, historical & random)
* Operators
    * Dynamic scaling
* Key-Value Store beta 2.0
* Consumption Based Rentention production ready ([#5108](https://github.com/pravega/pravega/issues/5108))

## Version 0.11
* Spillover from 0.10
* Refactor Tier-1
* Native client bindings (phase 2: Golang)
* Quality-of-Service-related features
* Segment Container load balancing ([#1644](https://github.com/pravega/pravega/issues/1644))
* Idempotent writer ([#1210](https://github.com/pravega/pravega/issues/1210), [#1437](https://github.com/pravega/pravega/issues/1437))
* Support config-based CDI and Spring client injection
* Cross-site replication (active-passive)
* Performance improvements continued
* Security enhancements continued

## Version 0.12
* Spillover from 0.11
* Native client bindings (phase 3: Node.js, Ruby, C#)
* Cross-site replication
* QoS improvements continued
* Performance improvements continued
* Security enhancements continued
* Edge functions
* Shared namespace across Pravega clusters (between edge and core)
* Pravega WebUI

# Future Items
The following items are new features that we wish to build in upcoming Pravega releases, however many active work is currently underway.  Please reach out on the Pravega channels if you're interested in picking one of these up.

-  Operational Features
    -  Non-disruptive and rolling upgrades for Pravega
    -  Provide default Failure Detector
    -  Exposing information for administration purposes
    -  Ability to define throughput quotas and other QoS guarantees
-  Pravega Connectors / Integration
    -  Kafka API Compatibility (Producer and Consumer APIs)
    -  Spark connectors (source/sink)
    -  REST Proxy for Reader/Writer (REST proxy for Admin operations is already there)
-  Stream Management
    -  Stream aliasing
    -  Ability to assign arbitrary Key-Value pairs to streams - Tagging
-  Tiering Support
    -  Policy driven tiering of Streams from Streaming Storage to Long-term storage
    -  Support for additional Tier 2 Storage backends
