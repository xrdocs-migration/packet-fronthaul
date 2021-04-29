---
published: false
date: '2021-04-29 14:39 +0530'
title: Packetizing Mobile Fronthaul with Cisco NCS540-FH
---

Hope you guys managed to spend some time on my last [blog](https://xrdocs.io/packet-fronthaul/blogs/firstconvergedFH/) where I 
- Introduced Cisco’s Converged Packet Fronthaul Portfolio
- Summarized the benefits of a packetized fronthaul solution over other (sub-optimal) optical fronthaul solutions in the industry right now
- Walked through key highlights of our Packet Fronthaul products 
  
…and with that information, I am hoping, it will help you to justify migrating to a packet based fronthaul from the fronthaul solution currently deployed at your Radio Access Network.
In this Blog, I will spend some time on the technicalities of packetizing a traditional RAN (4G LTE), one which accounts for more than 70-80% of world’s RAN deployment.  

## CPRI

Back in 2003, Ericsson, Huawei, NEC, Nortel Networks and Siemens developed a proprietary internal interface of the radio base station. With the advent of Long-Term Evolution (LTE/4G), the CPRI consortium witnessed a change of guard– now, the development work on this front is being done by Ericsson, Huawei, NEC and Nokia. The latest [CPRI Specification](http://www.cpri.info/downloads/CPRI_v_7_0_2015-10-09.pdf) (v7.0) defines this interface as below:  

![FH_4.png]({{site.baseurl}}/images/FH_4.png)
  
  
_“CPRI is a digitized and serial internal base station interface between the Radio Equipment Controller (which you understand better as BaseBand Unit) and the Radio Equipment (better know to you as the Remote Radio Unit). The Interface carries User Plane Data (IQ Data), Control and Management mechanisms for transport, and means for synchronization between the RRU and BBU.”_
  
  
In a Cloud-RAN or Centralized-RAN deployment, the Remote Radio Unit (RRU) sits at a Cell Site (either atop the antenna or inside an Outdoor Cabinet) and far away from the Baseband Unit (BBU) which is placed at a Centralized Location (or a Far Edge Data Center as we call it now). The RRU and the BBU are connected via the CPRI Interface which carries digitized IQ (or User plane) samples back and forth to be able to deliver 4G/LTE service to the end-user. For all of you finding it difficult to connect LTE to CPRI, you should know that 1 LTE Data Frame is equal to 10 ms of a CPRI frame which are further sub-divided into Hyperframes and Basic Frames and can be interpreted in both time and frequency domain to be able to calculate relevant radio resources for a particular Cell Site or Base Station.

  
![FH_5.png]({{site.baseurl}}/images/FH_5.png)





