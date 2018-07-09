QOS:Quality Of Service is the description or measurement（度量） of the overall performance\(整体性能\) of a service,such as a telephony or computer network or a cloud computing service,particularly（特别） the performance seen by the users of the network.To quantitatively measure（定量评估） quality of service are often considered,such as packet loss（数据包丢失）,bit rate（比特率）,thorughput（吞吐率）,transmission delay（传输延时）,availability（有效性）， jitter（抖动）,etc.

In the field\(领域；运动场\) of computer networking and other packet-switched（分组交换的） telecommunication networks（电信网络）,quality of service refers to（适用于） traffic prioritization（传输优先级） and resource reservation（资源预留） control mechanisms（管理机制） rather than（而不是） the achieved（实现的） service quality.Quality of service is this ability to provide different priority to（for sth/sb 提供 sth ） different applications（应用程序）,users,or data flows（数据流）,or to guarantee a certain level of performance to a data flow（提供数据流有一定level的性能）.

Quality of service is particularly important for the transport of traffic\(通信量的传输\) with special requirements.In particular,developer（开发者） have introduced（引入，提出） Voice over IP technology to allow computer networks to become as userful as\(和···一样\) telephone nerworks for audio conversations（音频通话）,as well as（而且） supporting new applications with even（及时） stricter（严格的） nerwork performance requirements.

Quality of serveice technology:data flow accounting\(about h3c switch S10500\):

> * #### **acl number 3000**
> * #### **rule 0 permit ip source 1.1.1.1 destination 2.2.2.2 **
> * #### **traffic classifier classifier\_1**
> * #### **if-match acl 3000**
> * #### **traffic behavior behavior\_1**
> * #### **accuounting packet **
> * #### **qos policy QOS\_1**
> * #### ** classifier classifier**_**1 behavior behavior\_1**_
> * #### **inter g9/0/1 **
> * #### **qos apply policy  QOS\_1 inbound **
> * #### 
> * #### **display qos policy inter g9/0/1**



