# rsSixtySeven

An open source AES67 implemention in [Rust](http://www.rust-lang.org)


## Introduction

The AES67 standard is designed to allow realtime transmission of uncompressed audio data over standard ethernet.
It has been defined by the Audio Engineering Society [http://www.aes.org/](http://www.aes.org/) to ensure interoperabilty
across multiple manufacturers.

In fact AES67 bundles previous standards and RFCs so many already implemented parts can be reused.

The following references (minimal subset) must be taken into account:

* IEEE 1588-2008 - IEEE Standard for a Precision Clock Synchronization Protocol for Networked Measurement and Control Systems, IEEE
* RFC 3190 – RTP Payload Format for 12-bit DAT Audio and 20- and 24-bit Linear Sampled Audio, IETF
* RFC 3261 - SIP: Session Initiation Protocol, IETF
* RFC 3264 - An Offer/Answer Model with the Session Description Protocol (SDP), IETF
* RFC 3550 – RTP: A Transport Protocol for Real-Time Applications, IETF
* RFC 4566 – Session Description Protocol, IETF
* RFC 7273 – RTP Clock Source Signalling, IETF

## Scope of this library

This library provides means of packetizing and timestamping audio data, as well as send and receive them over an ethernet network.
The retrieval of timestamps is done by an external library.

Examples are provided that show sending and receiving of wave files.

## License

Copyright 2016 Marc Schettke

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
