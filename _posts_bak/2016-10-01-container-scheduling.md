---
layout: post
title: qCUDA
description: >
    GPGPU virtualization at a new API remoting method with para-virtualization
modified: 2016-10-28
category: [projects]
tags: [projects]
---

<section>
  <header>
    <h3>Contents</h3>
  </header>
<div id="drawer" markdown="1">
*  Auto generated table of contents
{:toc}
</div>
</section><!-- /#table-of-contents -->


## Overview

Future work to help decide on a scheduling solution

### Goal

Compare 3 of the current container scheduling solutions. Each approach will be tested using the same approach and metrics collected using via the same monitoring approach discussed in the previous post, namely - **Riemann** -> **InfluxDB** -> **Grafana**



The schedulers will be -

* [Docker Swarm](https://docs.docker.com/engine/swarm/)
* [Google Kubernetes](http://kubernetes.io/)
* [Hashicorp Nomad]()


### Pros & Cons

## Deployment

### Docker Swarm

We will use the same Ansible role that I used in the previous post


### Kubernetes

[Ansible](https://github.com/kubernetes/contrib/tree/master/ansible)


### Nomad

[Ansible](https://github.com/kbrebanov/ansible-nomad)