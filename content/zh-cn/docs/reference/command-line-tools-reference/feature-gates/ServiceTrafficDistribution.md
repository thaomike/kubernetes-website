---
title: ServiceTrafficDistribution
content_type: feature_gate

_build:
  list: never
  render: false

stages:
  - stage: alpha 
    defaultValue: false
    fromVersion: "1.30"
    toVersion: "1.30"
  - stage: beta
    defaultValue: true
    fromVersion: "1.31"
    toVersion: "1.32"
  - stage: stable
    defaultValue: true
    locked: true
    fromVersion: "1.33"
---

<!--
Allows usage of the optional `spec.trafficDistribution` field in Services. The
field offers a way to express preferences for how traffic is distributed to
Service endpoints.
-->
允许在 Service 中使用可选的 `spec.trafficDistribution` 字段。
此字段提供了一种对 Service 端点进行流量分发的偏好的表达方式。
