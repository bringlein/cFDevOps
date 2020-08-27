# Workshop on DevOps support for Cloud FPGA platforms


## Why is cFDevOps important?

With the slowdown of Moore's law as we know it, the Cloud is resorting to heterogeneous, accelerated computing to satisfy the ever-increasing demand for performance and power efficiency. In just a few years, FPGAs have emerged as compute accelerators next to GPUs and are part of the standard offerings from many Cloud vendors. However, the development environment, deployment procedures, security measures, and monitoring tools are different for each platform and the portability of the FPGA kernel designs remains limited. 
In this workshop, leading platform providers and developers are going to present the state-of-the-art for Cloud FPGA platforms and explore opportunities and directions for future improvements from the developer's point of view. Instead of focusing on the performance and optimization of a specific application, the goal of this workshop is to highlight the challenges, which a Cloud application developer faces when designing, implementing, deploying and debugging Cloud services on Cloud FPGA platforms. One important aspect is portability and scalability of designs across different Cloud providers and target platforms. 



## Program

The workshop will take place on  **Friday, September 4th 2020, 14h-17h CEST**. The workshop will be held online (Zoom Webinar).

| **Time (CEST)**  | **Title**                    | **Presenters**                |
|:----------------:|:-----------------------------|:------------------------------|
| 14:00 | Opening  | *The Organizers* |
| 14:05 | **Session 1**  | **Applications and Operations of Cloud FPGA environments** |
|       | Intro | *The Organizers* |
| 14:10 | Scalable FPGA Acceleration of Genomics Algorithms on the BlueBee Platform | Zaid Al-Ars |
| 14:20 | FPGA Operations for an Academic HPC System | Tobias Kenter |
| 14:40 | Making FPGAs First Class Citizens in the Cloud | Derek Chiou |
| 15:00 | Q & A | *Everyone* |
| 15:10 | **Break** | |
| 15:20 | **Session 2**  | **Programmability & Portability in Cloud FPGA environments** |
|       | Intro | *The Organizers* |
| 15:25 | Auto-scalable Heterogenous FPGA deployment on cloud and on-prem | Chris Kachris |
| 15:45 | openRole: How to bring 'Design once, run everywhere' to FPGAs | Burkhard Ringlein |
| 16:05 | Making Software Programmability for FPGAs a Success | Vinod Kathail |
| 16:25 | DevCloud: Intel’s FPGA enabled cloud computing | Lawrence Landis |
| 16:45 | Q & A | *Everyone* |
| 16:55 | Closing | *The Organizers* |


(More details about the talks see below.)


## Registration

Registration is mandatory via the FPL registration [here (Whova)](https://whova.com/portal/registration/fpl_202008/).
The registration is free of charge.

More details about the FPL registration can be found [here](https://www.fpl2020.org/attending/registration).


## Talks

### Session 1: Applications and Operations of Cloud FPGA environments

#### Scalable FPGA Acceleration of Genomics Algorithms on the BlueBee Platform
by *Zaid Al-Ars, Assistant Professor at TU Delft, Netherlands and Co-founder, BlueBee*


**Abstract:** The field of genomics has become a major contributor to exceptionally large datasets that require computationally expensive algorithms to analyze and extract insights. In order to shorten the analysis time, reduce cost, and increase computational efficiency, various hardware acceleration solutions have been proposed to accelerate computationally intensive algorithms in a number of genomics analysis pipelines. This makes FPGAs an attractive alternative to enable high-performance computation of such algorithms. In this talk, we show a couple of FPGA accelerated solutions of well-known computationally expensive genomics algorithms and the value they add to complex analysis pipelines. We will also discuss the Bluebee platform that enables a scalable, accelerated and secure private-cloud solution targeted at the clinic. Scalability of the platform allows for seamless increase of the throughput to analyze multiple genomics datasets in parallel, combined with acceleration to allow for reducing the latency of the analysis of any give dataset. The presentation also shows the results of a case study carried out with the German Cancer Research Center to execute their cancer diagnostic pipeline, achieving 8x acceleration of a whole genome sequencing dataset on a single compute node.

#### FPGA Operations for an Academic HPC System
by *Tobias Kenter, PC2, University of Paderborn*

**Abstract:** Power efficiency and performance have made FPGAs an increasingly attractive accelerator technology for data centers and HPC. The ability to map algorithms or library components directly into hardware structures is central for the efficiency, but also creates challenges since application components need to coexist with infrastructure like host interfaces and memory controllers on the same chip. The current HPC system at the Paderborn Center for Parallel Computing, that is mainly used for scientific applications like atomistic simulations, optoelectronics and quantum photonics, is equipped with 32 state-of-the-art FPGA accelerator cards. The operation concept of the system and particularly its FPGA section aims to hide some of the infrastructure complexity from users and developers on the system, while at the same time exposing the necessary flexibility to make best use of the device resources. In this presentation, I will talk about the operations and usage of this system under the aspects of provided infrastructure and flexible usage options. This includes the integration with the workload manager Slurm that maps compute jobs to resources and allows for on-demand provisioning of different versions of the board support package (BSP), also often denoted as shell. The BSP provides the memory, host, and network interfaces that developers of accelerator code need to use to integrate application kernels with the rest of the system. Looking beyond current usage modes, the talk will conclude with an outlook on challenges and opportunities for future FPGA usage in HPC systems.


#### Making FPGAs First Class Citizens in the Cloud
by *Derek Chiou, Partner Architect, Microsoft*

**Abstract:** FPGAs have been traditionally relegated to prototyping and glue logic. Microsoft has demonstrated that FPGAs can be used to implement significant infrastructure and computation components at full data center scale.  This talk will discuss some of the barriers that were overcome to get to that level of deployment and what I think would help FPGAs to further spread through the cloud.



### Session 2: Programmability & Portability in Cloud FPGA environments


#### Auto-scalable Heterogeneous FPGA deployment on cloud and on-prem 
by *Chris Kachris, Ph.D, CEO of InAccel*

**Abstract:** FPGAs have been emerged as a powerful accelerator platform for many applications like deep neural networks, machine learning and video transcoding. Cloud vendors have recognized the power of FPGAs and have recently adopted FPGAs as a computing resource that users can utilize. However, there are currently several limitations that prevent the automatic deployment and utilization of FPGA on the cloud or on-prem. Enterprise customers now have the option to adopt a hybrid deployment for their FPGA-accelerated applications. That means, that companies can purchase a small number of FPGAs deployed on-prem and if these FPGAs are overloaded, they can automatically scale it using the cloud resources. InAccel, using the unique platform-agnostic FPGA orchestration allows auto-scaling hybrid FPGA deployment in the most efficient way. In this presentation, InAccel will demonstrate how users can experience the power of the FPGAs on a hybrid deployment on-prem and on cloud. InAccel will show a unique platform that allows vendor-agnostic and platform agnostic auto-scalable FPGA deployment on the a heterogeneous environment.


#### openRole: How to bring 'Design once, run everywhere' to FPGAs
by *Burkhard Ringlein, IBM Research Europe, Switzerland*

**Abstract:** The emergence of FPGAs as compute accelerators in the Cloud and other multi-user environments inevitably lead to a split of the FPGA design into an user application programmed by the developers and a platform specific part controlled by the infrastructure provider. This split of FPGA logic into a vendor controlled SHELL and a user-controlled ROLE allows the necessary introduction of different privilege levels within an FPGA design and potentially improves re-usability of user applications. The SHELL – ROLE  architectural pattern can be observed widely across different FPGA platforms, but despite the strong similarity of approaches, all implementations differ in details. The differences in the SHELL – ROLE  interface between platform and application limits the portability of applications for no good reason and decelerates the adoption of all FPGA-based platforms. This situation resembles the early days of operating systems running on CPUs, before standards like POSIX introduced unified interfaces between the OS and the application code. We propose to address this with openROLE, which is an attempt to formulate similar standards for FPGA platforms.


#### Making Software Programmability for FPGAs a Success
by *Vinod Kathail, Xilinx Fellow and Chief Architect for Vitis, Xilinx*

**Abstract:** FPGAs provide significant advantages in throughput, latency, and energy efficiency for implementing low-latency, compute-intensive applications when compared to general-purpose CPUs and GPUs.  Over the last decade, FPGAs have evolved into highly configurable SoCs with on-chip CPUs, domain-specific programmable accelerators, and flexible connectivity options.This advancement on the device side is accompanied by the availability of higher-level programming approaches which has made FPGAs significantly easy to use for a wide range of compute intensive applications. Most of this advancement has focused on the two main areas: 1) Platform or shell abstraction to provide standard services for device management, memory management and data transfers to applications, something that is commonly available for CPUs and GPUs. 2)Programming abstraction for higher level programming of FPGA either using HLS with languages like C, C++ and OpenCL as entry points, or using domain specific architectures and integrating with higher-level frameworks like Spark and Tensorflow enabling data scientists to work in their familiar environment.  There has been, however, less focus on some of the other areas that application programmers expect, but that is beginning to change as the FPGA usage in compute intensive applications grows. These include: 1) Easy composability enabling easier construction of large, complex applications using libraries and other building blocks, some of which may be running on other devices or accelerators. 2) Portability from one device to another, from one platform to another, and from one release of tools and platforms to the next release. In this talk, we will briefly discuss the challenges associated with these requirements and possible solutions to address them, hoping to spark a thought-provoking debate.


#### DevCloud: Intel’s FPGA enabled cloud computing
by *awrence Landis, Senior Manager, Intel Programmable Solutions Group*

**Abstract:** This presentation will describe the Intel FPGA enabled cloud computing clusters accessible to the academic community, which one will serve your needs, and how to gain access. Intel offers a number of cloud computing clusters using attached FPGA Acceleration Cards that are available to academia and researchers. A number of heterogenous acceleration workflows are supported including: HLS and OpenCL emulation and compilation, OneAPI (dpc++) emulation and compilation, FPGA download and heterogeneous workload execution on XEON servers with attached FPGA cards, OpenVIno Computer Vision and AI inference acceleration across CPU and FPGA, hands-free control of remote FPGA boards. 



## Organizers


#### Gustavo Alonso, Department of Computer Science, ETH Zurich, Switzerland
Gustavo Alonso is a Professor of Computer Science at ETH Zürich where he is a member of the Systems Group (www.systems.ethz.ch) and the Head of the Institute for Computing Platforms. He has a degree in electrical engineering from the Madrid Technical University as well as a M.S. and Ph.D. degrees in Computer Science from UC Santa Barbara. Gustavo's research interests encompass almost all aspects of systems, from design to run time. He works on distributed systems, data processing, and system aspects of programming languages. Most of his research these days is related to data processing on data centers and the cloud as well as hardware acceleration using FPGAs. Gustavo has received numerous awards for his work, including four Test-of-Time awards for contributions to databases, programming languages, mobile computing, and systems. He is a Fellow of the ACM and of the IEEE as well as a Distinguished Alumnus of the Department of Computer Science of UC Santa Barbara.


#### Chris Kachris, inaccel, Greece
Chris Kachris the founder and CEO of InAccel that helps companies speedup their applications using hardware accelerators (FPGAs) in the cloud or on-prem. Inaccel, using a unique FPGA orchestrator, allows scalable deployment of FPGA clusters. Chris holds a Ph.D. from Delft University of Technology. He has published more than 70 papers in international journals and conferences with more than 1800 citations. He has over 15 years of experience on FPGAs and he is the editor of the book Hardware Accelerators in Data Centers.


#### Christoph Hagleitner, IBM Research Europe, Switzerland
Christoph Hagleitner leads the cloudFPGA project at the IBM Research Europe Lab (ZRL) in Ruschlikon, Switzerland. He obtained a Ph.D. degree for a thesis on CMOS-integrated Microsensors from ETH, Zurich, Switzerland in 2002. In 2003 he joined IBM Research to work on the system architecture of a novel probe-storage device (“millipede”-project). In 2008, he started to build up a new research group in the area of accelerator technologies. The team initially focused on integrated accelerator cores and gradually expanded its research to heterogeneous computing systems and their applications.


#### Dionysios Diamantopoulos, IBM Research Europe, Switzerland
Dionysios Diamantopoulos is a Post-Doc Researcher in the  Cloud & AI Systems Research department of IBM Research  Europe. Dionysios holds a PhD  from ECE/Technical University of Athens (2015), and a D.Eng. from CEID/University of Patras (2009). Being affiliated with the ICCS, he was enrolled in several research projects from EU (FP7, H2020) and European Space Agency.  Dionysios joined IBM ZRL (2017) as a researcher in Transprecision Computing. His research is disseminated in one book chapter and more than 30 publications in international conferences and journals. He is the co-inventor of  three filed patents and one pending (USPTO). His research interests lie in the system-level specialization that lay the foundation of heterogeneous-accelerated systems for the hybrid cloud era.  He is a member of HiPEAC, IEEE, IEEE CAS and Technical Chamber of Greece. 


#### Burkhard Ringlein, IBM Research Europe, Switzerland
Burkhard Ringlein is a Predoctoral Researcher in the Cloud & AI Systems Research department of the IBM Research Zurich Laboratory and pursues his PhD in cooperation with the Department of Computer Science, Computer Architecture of the Friedrich-Alexander University Erlangen-Nürnberg, Germany. As part of the cloudFPGA project, he is focusing on Distributed Reconfigurable Architectures in the context of High-Performance-Computing and AI Acceleration. 


## Contact

[Christoph Hagleitner](http://researcher.watson.ibm.com/researcher/view.php?person=zurich-HLEhttp://researcher.watson.ibm.com/researcher/view.php?person=zurich-HLE)

[Burkhard Ringlein](https://researcher.watson.ibm.com/researcher/view.php?person=zurich-NGL)


