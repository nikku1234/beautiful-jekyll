---
layout: post
title: Creational Patterns
#gh-repo:
#gh-badge: [star, fork, follow]
tags: [design-patterns,builder,single,prototype]
image:

---

Edge computing is transforming the way data is being handled, processed, and delivered from millions of devices around the world. The explosive growth of internet-connected devices – the [IoT](https://www.networkworld.com/article/3207535/what-is-iot-how-the-internet-of-things-works.html) – along with new applications that require real-time computing power, continues to drive edge-computing systems.

Faster networking technologies, such as [5G](https://www.networkworld.com/article/3330603/5g-versus-4g-how-speed-latency-and-application-support-differ.html) wireless, are allowing for edge computing systems to accelerate the creation or support of real-time applications, such as video processing and analytics, self-driving cars, artificial intelligence and robotics, to name a few.



## What is edge computing?

Gartner defines edge computing as “a part of a distributed computing topology in which information processing is located close to the edge – where things and people produce or consume that information.”

At its basic level, edge computing brings computation and data storage closer to the devices where it’s being gathered, rather than relying on a central location that can be thousands of miles away. This is done so that data, especially real-time data, does not suffer latency issues that can affect an application’s performance. In addition, companies can save money by having the processing done locally, reducing the amount of data that needs to be processed in a centralized or cloud-based location.

Edge computing was developed due to the exponential growth of IoT devices, which connect to the internet for either receiving information from the cloud or delivering data back to the cloud. And many IoT devices generate enormous amounts of data during the course of their operations.



![Network World - How Edge Computing Works [diagram]](https://images.idgesg.net/images/article/2017/09/nw_how_edge_computing_works_diagram_1400x1717-100736111-large.jpg)

Think about devices that monitor manufacturing equipment on a factory floor, or an internet-connected video camera that sends live footage from a remote office. While a single device producing data can transmit it across a network quite easily, problems arise when the number of devices transmitting data at the same time grows. Instead of one video camera transmitting live footage, multiply that by hundreds or thousands of devices. Not only will quality suffer due to latency, but the costs in bandwidth can be tremendous.

Edge-computing hardware and services help solve this problem by being a local source of processing and storage for many of these systems. An edge gateway, for example, can process data from an edge device, and then send only the relevant data back through the cloud, reducing bandwidth needs. Or it can send data back to the edge device in the case of real-time application needs.



These edge devices can include many different things, such as an IoT sensor, an employee’s notebook computer, their latest smartphone, the security camera or even the internet-connected microwave oven in the office break room. Edge gateways themselves are considered edge devices within an edge-computing infrastructure.



In the beginning, there was One Big Computer. Then, in the Unix era, we learned how to connect to that computer using dumb (not a pejorative) terminals. Next we had personal computers, which was the first time regular people really owned the hardware that did the work.

Right now, in 2018, we’re firmly in the cloud computing era. Many of us still own personal computers, but we mostly use them to access centralized services like Dropbox, Gmail, Office 365, and Slack. Additionally, devices like Amazon Echo, Google Chromecast, and the Apple TV are powered by content and intelligence that’s in the cloud — as opposed to the DVD box set of *Little House on the Prairie* or CD-ROM copy of Encarta you might’ve enjoyed in the personal computing era.

MOST OF THE NEW OPPORTUNITIES FOR THE “CLOUD” LIE AT THE “EDGE”

As centralized as this all sounds, the truly amazing thing about cloud computing is that a seriously large percentage of all companies in the world now rely on the infrastructure, hosting, machine learning, and compute power of a very select few cloud providers: Amazon, Microsoft, Google, and IBM.

Amazon, the largest by far of these “public cloud” providers (as opposed to the “private clouds” that companies like Apple, Facebook, and Dropbox host themselves) had [47 percent of the market](https://www.skyhighnetworks.com/cloud-security-blog/microsoft-azure-closes-iaas-adoption-gap-with-amazon-aws/) in 2017.

The advent of edge computing as a buzzword you should perhaps pay attention to is the realization by these companies that there isn’t much growth left in the cloud space. Almost everything that can be centralized has been centralized. Most of the new opportunities for the “cloud” lie at the “edge.”

So, what is edge?

The word edge in this context means literal geographic distribution. Edge computing is computing that’s done at or near the source of the data, instead of relying on the cloud at one of a dozen data centers to do all the work. It doesn’t mean the cloud will disappear. It means the cloud is coming to you.

That said, let’s get out of the word definition game and try to examine what people mean practically when they extoll edge computing.

Edge computing is a networking philosophy focused on bringing computing as close to the source of data as possible in order to reduce latency and bandwidth use. In simpler terms, edge computing means running fewer processes in the cloud and moving those processes to local places, such as on a user’s computer, an [IoT device](https://www.cloudflare.com/learning/ddos/glossary/internet-of-things-iot/), or an [edge server](https://www.cloudflare.com/learning/cdn/glossary/edge-server/). Bringing computation to the network’s edge minimizes the amount of long-distance communication that has to happen between a client and server.



## Why does edge computing matter?

For many companies, the cost savings alone can be a driver towards deploying an edge-computing architecture. Companies that embraced the cloud for many of their applications may have discovered that the costs in bandwidth were higher than they expected.

Increasingly, though, the biggest benefit of edge computing is the ability to process and store data faster, enabling for more efficient real-time applications that are critical to companies. Before edge computing, a smartphone scanning a person’s face for facial recognition would need to run the facial recognition algorithm through a cloud-based service, which would take a lot of time to process. With an edge computing model, the algorithm could run locally on an edge server or gateway, or even on the smartphone itself, given the increasing power of smartphones. Applications such as virtual and augmented reality, self-driving cars, smart cities and even building-automation systems require fast processing and response.

“Edge computing has evolved significantly from the days of isolated IT at ROBO [Remote Office Branch Office] locations,” says Kuba Stolarski, a research director at IDC, in the “[Worldwide Edge Infrastructure (Compute and Storage) Forecast, 2019-2023](https://www.idc.com/getdoc.jsp?containerId=US45575419)” report. “With enhanced interconnectivity enabling improved edge access to more core applications, and with new IoT and industry-specific business use cases, edge infrastructure is poised to be one of the main growth engines in the server and storage market for the next decade and beyond.”



Companies such as NVIDIA have recognized the need for more processing at the edge, which is why we’re seeing new system modules that include artificial intelligence functionality built into them. The company’s [latest Jetson Xavier NX module](https://nvidianews.nvidia.com/news/nvidia-announces-jetson-xavier-nx-worlds-smallest-supercomputer-for-ai-at-the-edge), for example, is smaller than a credit-card, and can be built into smaller devices such as drones, robots and medical devices. AI algorithms require large amounts of processing power, which is why most of them run via cloud services. The growth of AI chipsets that can handle processing at the edge will allow for better real-time responses within applications that need instant computing.

## Privacy and security

However, as is the case with many new technologies, solving one problem can create others. From a security standpoint, data at the edge can be troublesome, especially when it’s being handled by different devices that might not be as secure as a centralized or cloud-based system. As the number of IoT devices grow, it’s imperative that IT understand the potential security issues around these devices, and to make sure those systems can be secured. This includes making sure that data is encrypted, and that the correct access-control methods and even [VPN](https://www.networkworld.com/article/3268744/understanding-virtual-private-networks-and-why-vpns-are-important-to-sd-wan.html)tunneling is utilized.

Furthermore, differing device requirements for processing power, electricity and network connectivity can have an impact on the reliability of an edge device. This makes redundancy and failover management crucial for devices that process data at the edge to ensure that the data is delivered and processed correctly when a single node goes down.

## What about 5G?

Around the world, carriers are deploying 5G wireless technologies, which promise the benefits of high bandwidth and low latency for applications, enabling companies to go from a garden hose to a firehose with their data bandwidth. Instead of just offering the faster speeds and telling companies to continue processing data in the cloud, many carriers are working edge-computing strategies into their 5G deployments in order to offer faster real-time processing, especially for mobile devices, connected cars and self-driving cars.

In its recent report “[5G, IoT and Edge Compute Trends](https://www.networkworld.com/resources/194551/5g--iot-and-edge-compute-trends),” Futuriom writes that 5G will be a catalyst for edge-compute technology. “Applications using 5G technology will change traffic demand patterns, providing the biggest driver for edge computing in mobile cellular networks,” the firm writes. It cites low-latency applications that include IoT analytics, machine learning, virtual reality, autonomous vehicles as those that “have new bandwidth and latency characteristics that will require support from edge-compute infrastructure.”

In its [predictions for 2020](https://go.forrester.com/predictions-2020/), Forrester also cited [the need for on-demand compute](https://www.networkworld.com/article/3451532/forrester-edge-computing-is-about-to-bloom.html)and **real-time** application engagements would play a role in driving the growth of edge computing in 2020.

It’s clear that while the initial goal for edge computing was to reduce bandwidth costs for IoT devices over long distances, the growth of real-time applications that require local processing and storage capabilities will drive the technology forward over the coming years.



## LATENCY

One great driver for edge computing is the speed of light. If a Computer A needs to ask Computer B, half a globe away, before it can do anything, the user of Computer A perceives this delay as latency. The brief moments after you click a link before your web browser starts to actually show anything is in large part due to the speed of light. Multiplayer video games implement numerous elaborate techniques to mitigate true and perceived delay between you shooting at someone and you knowing, for certain, that you missed.

EDGE COMPUTING HAS PRIVACY BENEFITS, BUT THEY AREN’T GUARANTEED

Voice assistants typically need to resolve your requests in the cloud, and the roundtrip time can be very noticeable. Your Echo has to process your speech, send a compressed representation of it to the cloud, the cloud has to uncompress that representation and process it — which might involve pinging another API somewhere, maybe to figure out the weather, and adding more speed of light-bound delay — and then the cloud sends your Echo the answer, and finally you can learn that today you should expect a high of 85 and a low of 42, so definitely give up on dressing appropriately for the weather.

So, a recent rumor that Amazon is [working on its own AI chips for Alexa](https://techcrunch.com/2018/02/12/amazon-may-be-developing-ai-chips-for-alexa/) should come as no surprise. The more processing Amazon can do on your local Echo device, the less your Echo has to rely on the cloud. It means you get quicker replies, Amazon’s server costs are less expensive, and conceivably, if enough of the work is done locally you could end up with more privacy — if Amazon is feeling magnanimous.

## PRIVACY AND SECURITY

It might be weird to think of it this way, but the security and privacy features of an iPhone are well accepted as an example of edge computing. Simply by doing encryption and storing biometric information on the device, Apple offloads a ton of security concerns from the centralized cloud to its diasporic users’ devices.

But the other reason this feels like edge computing to me, not personal computing, is because while the compute work is distributed, the definition of the compute work is managed centrally. You didn’t have to cobble together the hardware, software, and security best practices to keep your iPhone secure. You just paid $999 at the cellphone store and trained it to recognize your face.

The management aspect of edge computing is hugely important for security. Think of how much pain and suffering consumers have experienced with [poorly managed Internet of Things devices](https://www.theverge.com/2016/10/21/13362354/dyn-dns-ddos-attack-cause-outage-status-explained).

That’s why Microsoft is working on [Azure Sphere](https://click.linksynergy.com/deeplink?id=nOD/rLJHOac&mid=24542&u1=[]vg[e]17091625[r]google.com[t]w[d]D&murl=https://azure.microsoft.com/en-us/blog/introducing-microsoft-azure-sphere-secure-and-power-the-intelligent-edge/), which is a managed Linux OS, a certified microcontroller, and a cloud service. The idea is that your toaster should be as difficult to hack, and as centrally updated and managed, as your Xbox.

I have no idea if the industry will embrace Microsoft’s specific solution to the IoT security problem, but it seems an easy guess that most of the hardware you buy a few years from now will have its software updated automatically and security managed centrally. Because otherwise your toaster and dishwasher will join a botnet and ruin your life.

If you doubt me, just look at the success Google, Microsoft, and Mozilla have had in moving browsers to an “evergreen” model.

Think about it: you could probably tell me which version of Windows you’re running. But do you know which version of Chrome you have? Edge computing will be more like Chrome, less like Windows.

## BANDWIDTH

Security isn’t the only way that edge computing will help solve the problems IoT introduced. The other hot example I see mentioned a lot by edge proponents is the bandwidth savings enabled by edge computing.

For instance, if you buy one security camera, you can probably stream all of its footage to the cloud. If you buy a dozen security cameras, you have a bandwidth problem. But if the cameras are smart enough to only save the “important” footage and discard the rest, your internet pipes are saved.

Almost any technology that’s applicable to the latency problem is applicable to the bandwidth problem. Running AI on a user’s device instead of all in the cloud seems to be [a huge focus for Apple and Google right now](https://www.theverge.com/2017/10/19/16502538/mobile-ai-chips-apple-google-huawei-qualcomm).

COMPANIES WILL CONTROL EVEN MORE OF YOUR LIFE EXPERIENCES THAN THEY DO RIGHT NOW

But Google is also working hard at making even websites more edge-y. [Progressive Web Apps](https://www.theverge.com/circuitbreaker/2018/4/11/17207964/web-apps-quality-pwa-webassembly-houdini) typically have offline-first functionality. That means you can open a “website” on your phone without an internet connection, do some work, save your changes locally, and only sync up with the cloud when it’s convenient.

Google also is getting smarter at combining local AI features for the purpose of privacy *and*bandwidth savings. For instance, [Google Clips](https://www.theverge.com/2018/2/27/17055618/google-clips-smart-camera-review) keeps all your data local by default and does its magical AI inference locally. It doesn’t work very well at its stated purpose of capturing cool moments from your life. But, conceptually, it’s quintessential edge computing.



## WHAT ARE WE GIVING UP?

I have some fears about edge computing that are hard to articulate, and possibly unfounded, so I won’t dive into them completely.

But the big picture is that the companies who do it the best will control even more of your life experiences than they do right now.

When the devices in your home and garage are managed by Google Amazon Microsoft Apple, you don’t have to worry about security. You don’t have to worry about updates. You don’t have to worry about functionality. You don’t have to worry about capabilities. You’ll just take what you’re given and use it the best you can.

In this worst-case world, you wake up in the morning and ask Alexa Siri Cortana Assistant what features your corporate overlords have pushed to your toaster, dishwasher, car, and phone overnight. In the personal computer era you would “install” software. In the edge computing era, you’ll only use it.

It’s up to the big companies to decide how much control they want to gain over their users’ lives. But, it might also be up to us users to decide if there’s another way to build the future. Yes, it’s kind of a relief to take your hands off the steering wheel and let Larry Page guide you. But what if you don’t like where he’s going?

One drawback of edge computing is that it can increase attack vectors. With the addition of more ‘smart’ devices into the mix, such as edge servers and IoT devices that have robust built-in computers, there are new opportunities for malicious attackers to compromise these devices.

Another drawback with edge computing is that it requires more local hardware. For example, while an IoT camera needs a built-in computer to send its raw video data to a web server, it would require a much more sophisticated computer with more processing power in order for it to run its own motion-detection algorithms. But the dropping costs of hardware are making it cheaper to build smarter devices.

One way to completely mitigate the need for extra hardware is to take advantage of edge servers. For example, with Cloudflare’s network of 200 geographically distributed edge locations, Cloudflare customers can have edge code running worldwide using [Cloudflare Workers](https://www.cloudflare.com/products/cloudflare-workers/).





## What differentiates edge computing from other computing models?

The first computers were large, bulky machines that could only be accessed directly or via terminals that were basically an extension of the computer. With the invention of personal computers, computing could take place in a much more distributed fashion. For a time, personal computing was the dominant computing model. Applications ran and data was stored locally on a user's device, or sometimes within an on-premise data center.

[Cloud computing](https://www.cloudflare.com/learning/cloud/what-is-the-cloud/), a more recent development, offered a number of advantages over this locally based, on-premise computing. Cloud services are centralized in a vendor-managed "cloud" (or collection of data centers) and can be accessed from any device over the Internet.

However, cloud computing can introduce latency because of the distance between users and the data centers where cloud services are hosted. Edge computing moves computing closer to end users to minimize the distance that data has to travel, while still retaining the centralized nature of cloud computing.

To summarize:

- Early computing: Centralized applications only running on one isolated computer
- Personal computing: Decentralized applications running locally
- Cloud computing: Centralized applications running in data centers
- Edge computing: Centralized applications running close to users, either on the device itself or on the network edge

## What is an example of edge computing?

Consider a building secured with dozens of high-definition IoT video cameras. These are ‘dumb’ cameras that simply output a raw video signal and continuously stream that signal to a cloud server. On the cloud server, the video output from all the cameras is put through a motion-detection application to ensure that only clips featuring activity are saved to the server’s database. This means there is a constant and significant strain on the building’s Internet infrastructure, as significant bandwidth gets consumed by the high volume of video footage being transferred. Additionally, there is very heavy load on the cloud server that has to process the video footage from all the cameras simultaneously.

Now imagine that the motion sensor computation is moved to the network edge. What if each camera used its own internal computer to run the motion-detecting application and then sent footage to the cloud server as needed? This would result in a significant reduction in bandwidth use, because much of the camera footage will never have to travel to the cloud server.

Additionally, the cloud server would now only be responsible for storing the important footage, meaning that the server could communicate with a higher number of cameras without getting overloaded. This is what edge computing looks like.

## What are other possible use cases for edge computing?

Edge computing can be incorporated into a wide variety of applications, products, and services. A few possibilities include:

- Security system monitoring: As described above.
- IoT devices: Smart devices that connect to the Internet can benefit from running code on the device itself, rather than in the cloud, for more efficient user interactions.
- Self-driving cars: Autonomous vehicles need to react in real time, without waiting for instructions from a server.
- More efficient caching: By running code on a CDN edge network, an application can customize how content is cached to more efficiently serve content to users.
- Medical monitoring devices: It is crucial for medical devices to respond in real time without waiting to hear from a cloud server.
- Video conferencing: Interactive live video takes quite a bit of bandwidth, so moving backend processes closer to the source of the video can decrease lag and latency.

## What are the benefits of edge computing?

#### Cost savings

As seen in the example above, edge computing helps minimize bandwidth use and server resources. Bandwidth and cloud resources are finite and cost money. With every household and office becoming equipped with smart cameras, printers, thermostats, and even toasters, Statista [predicts](https://www.statista.com/statistics/471264/iot-number-of-connected-devices-worldwide/) that by 2025 there will be over 75 billion IoT devices installed worldwide. In order to support all those devices, significant amounts of computation will have to be moved to the edge.

#### Performance

Another significant benefit of moving processes to the edge is to reduce latency. Every time a device needs to communicate with a distant server somewhere, that creates a delay. For example, two coworkers in the same office chatting over an IM platform might experience a sizable delay because each message has to be routed out of the building, communicate with a server somewhere across the globe, and be brought back before it appears on the recipient’s screen. If that process is brought to the edge, and the company’s internal router is in charge of transferring intra-office chats, that noticeable delay would not exist.

Similarly, when users of all kinds of web applications run into processes that have to communicate with an external server, they will encounter delays. The duration of these delays will vary based upon their available bandwidth and the location of the server, but these delays can be avoided altogether by bringing more processes to the network edge.

#### New functionality

In addition, edge computing can provide new functionality that wasn’t previously available. For example, a company can use edge computing to process and analyze their data at the edge, which makes it possible to do so in real time.

To recap, the key benefits of edge computing are:

- Decreased latency
- Decrease in bandwidth use and associated cost
- Decrease in server resources and associated cost
- Added functionality

## 