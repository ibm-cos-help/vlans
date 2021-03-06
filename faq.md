---
copyright:
  years: 1994, 2017
lastupdated: "2017-10-17"
---
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# FAQs


## Can I move an existing device to a new VLAN?

Existing devices can be moved to other VLANs, but only when the move is requested. Because VLANs are tied to a router and connections to each router are dependent upon the device's physical location, some VLAN moves may require a physical relocation, as well. This is always the case when the new VLAN is located in a different datacenter, but it also may apply when moving a device to a different VLAN within the same datacenter. Making this change interrupts network connectivity and requires changing the device's IP address when the connection is moved to the new VLAN. When moving a device to a new VLAN we ask that ample planning is allowed, because the machine will be offline for the duration of the move.


## Is there a way to specify which VLAN I want to use for my device when I order it?

Yes, a specific VLAN may be specified during the ordering process. When ordering a device, this option is available at the end of the order form. A private VLAN is selected, followed by a public VLAN. It is important to note that the VLAN must be located in the same datacenter as the device. We cannot assign a device to a VLAN that is in a different datacenter.

## How many devices may be assigned to a single VLAN?

There currently is no limit to the number of devices that are associated with a single VLAN at any time; however, when a hardware firewall is associated with a VLAN, the firewall rules may impose restrictions on the number of devices that reside on the VLAN.

## Do VLANs work on both the public and the private network?

Yes, there are both public and private VLANs. In most cases, a device has both--a public connection and a private connection-- which means it will have a connection in both a public and a private VLAN.

## What kinds of devices are assigned to a VLAN?

Any device that has a network connection will be associated with a VLAN. Dedicated servers have both a public and private network connection, so you will see those devices associated with both public and private VLANs (one VLAN per connection type, per device).

Hardware firewalls work a bit differently: they are positioned in front of a VLAN to intercept and filter traffic. These devices are tied to the VLAN for which they serve, but they do not actually reside on the VLAN itself.
