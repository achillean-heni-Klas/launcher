
#  **FLEETDEV Cloud**

![Go](https://img.shields.io/badge/go-1.22-blue)
![MQTT](https://img.shields.io/badge/protocol-MQTT-orange)
![Kubernetes](https://img.shields.io/badge/deploy-cloud--native-green)

**Manage and monitor autonomous device fleets from centralized dashboard.**

---

###  Intro

FLEETDEV connects edge devices to cloud infrastructure.
Real-time telemetry, firmware updates, and task orchestration.

Live demo: [cloud.fleetdev.app](https://cloud.fleetdev.app)

---

### 🪶 Quick Deploy

```bash
helm install FLEETDEV ./charts/FLEETDEV \
  --set cloud.mqttBroker=brokerdebug.FLEETDEV.dev
```

---

###  Architecture

```
[device] ⇄ [agent] ⇄ [broker] ⇄ [api] ⇄ [dashboard]
```

* Go agents, <5MB footprint
* gRPC telemetry streaming
* Built-in alerting

---

### API Example

```bash
curl https://api.FLEETDEV.app/v1/devices | jq .
```

---

### Plans

| Tier | Devices | Price |
| ---- | ------- | ----- |
| Hobby | 20 | Free |
| Startup | 500 | $25/mo |

Apache-2.0 © 
