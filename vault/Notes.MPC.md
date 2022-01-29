---
id: o3XAgybLAJzQd85ehWJH0
title: MPC
desc: ''
updated: 1643500418737
created: 1643396150975
---


## Multiparty Computation(MPC) or Secure MPC (SMPC)

**Secure multi-party computation (SMPC)** is a cryptographic technique that allows multiple people to compute a function, where the function itself and its outputs are public, but the inputs are kept private to each person.

Protocols: 

* **Threshold secret sharing**
* **Oblivious Transafer(OT)** allow two parties to transfer two encrypted messages from one party to the next in a way that ensures the messages were sent and received, but the sender doesn't know which one of the messages the receiver chose to open.
* **Private Set Intersection(PSI)**
* **Garbled Boolean circuits** are encrypted versions of digital logic circuits, consisting of hardware or programmed wires and logic gates that follow a prescribed logic when computing a function. To “garble” the circuit means encrypting the possible input combinations and possible outputs, described in the so-called truth tables at the logic gates. Then, each logic gate outputs cryptographic keys used to unlock the output of the next gate, a process set forth until arriving at the final result.
* **Shamir's secret sharing**, data (for example, personal data or a machine learning model) is split up into fragments, which in themselves do not contain any usable information. The secret shares are distributed amongst a set of parties to perform secure computation over the shares, releasing output to a designated party once done.

To elevate the privacy posture and cover more use cases, MPC is often combined with federated learning, homomorphic encryption and differential privacy.



Reference: 
* [Multiparty computation as supplementary measure and potential data anonymization tool](https://iapp.org/news/a/multiparty-computation-as-supplementary-measure-and-potential-data-anonymization-tool/)
* [A Pragmatic Introduction to Secure Multi-Party Computation](https://www.cs.virginia.edu/~evans/pragmaticmpc/pragmaticmpc.pdf)
* [Out of the Box, Blockchain Powered Verifiable PPC Framework](https://deltampc.com/en)
### Private Set Intersection(PSI)
> Maybe can be implemented in IoT devices.

PSI References: [Efficient Batched Oblivious PRF with Applications to Private Set Intersection](https://csrc.nist.gov/CSRC/media//Projects/pec/documents/stppa-02-PSI-rosulek.pdf)



### What is Oblivious Transafer(OT)

Oblivious Transfer (OT) has been a central primitive in the area of secure computation.

References:
[The Simplest Protocol for Oblivious Transfer](https://eprint.iacr.org/2015/267.pdf)
[SimpleOT Github](https://github.com/mkskeller/SimpleOT/tree/84d73522619f90ba2aabce8d660baef1442aa26d)


### Secret Sharing

