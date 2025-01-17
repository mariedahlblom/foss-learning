---
layout: default
title: Secure supply chain
nav_order: 2
has_children: true
permalink: /SEC-supply-chain-Ind
---

# Secure supply chain
Prior to the launch of the free software movement, by Richard Stallman, the GNU Project and its manifest published in 1985, software was either not considered a commodity and shared freely in the world of academia, or simply considered part of the hardware on which it was supposed to dedicatedly run.

## Introduction
When consuming an open source component in an ecosystem where source code and/or binary versions of the component are automatically fetched from an external server to be part of your development/product/solution it’s very much desired to verifiably know that this component was built with integrity in a secure build system. It is also desired to have documented integrity between the built binary and the specified and verified source code developed by known community participants. The described setup is still immature, but there are initiatives pushing in this direction like OpenSSF focusing on secure supply of open source software.

Increasing regulatory requirements, like the need to declare your open source content, including versioning, in your developed software with a software bill of materials (SBOM), is focusing on transparency of open source usage for the consumer of the developed software. Given the amount of open source components being used by commercial companies in their product development, it’s a natural development given the risk exposure otherwise.

## Can you define trust
Trust is good and comes in various forms like formal and/or experience based, but a verifiable amount of certainty is preferred for a risk-based decision to consume an open source software. External sources can’t be blindly trusted why content verification is needed. Vicious and malicious community members can have the most well-polished facades. 

It’s possible to quantify the number of downloads over a defined time period, or the number of communities that are available on a server like Maven Central. Are such numbers providing trust? Or is it the number of developers contributing to a certain open source project creating trust? Basically, how can you quantify trust?

The alternative to blind trust, or trust by volume, is to always be able to quantify or verify the content and having trust in and from the verification mechanism. One such trust indicator is the OpenSSF ScoreCard initiative, which provide measured indicators regarding the open source software. This is the direction the industry is heading including methods like signed builds and commits.

##	Verification methods
There exist methods to verify the provided content. The developer can digitally sign-off the commit thus providing traceability and secure content. Digital signatures can also be used on the compiled result thus securing authenticity and the origin of the software. Furthermore, distributed hashes may be used to verify the received software artifact.

Sign-off methodology is today the most promising or talked about alternative for a secure supply chain, but it doesn’t deal at all with hi-jacked accounts or intended malicious behavior why other methods also are needed.

##	Accurate and trusted SBOM 
The "software bill of materials" (SBOM) has emerged as a key building block in software security and software supply chain risk management. A SBOM is a nested inventory, a list of ingredients that make up software components. In a nutshell, a SBOM is formal and machine-readable metadata that uniquely identifies a software package and its contents. It may include other information about its contents, including copyrights and license data. SBOMs are designed to be shared across organizations and are particularly helpful at providing transparency of components delivered by participants in a software supply chain. Many organizations concerned about software security are making SBOMs a cornerstone of their cyber-security strategy.

Still, the existence of an SBOM is not sufficient. The SBOM provides a declaration of included open source content and it serves as a foundation for a dialogue and an understanding of the included software components between provider and consumer. This understanding should include how possible weaknesses or risks have been mitigated.

The final result from a software composition analysis constitutes the external software content of your product, and shall be declared as a part of the SBOM. The SBOM shall be a part of the official delivery and shall be on a specified standardized format, like SPDX or CycloneDX.
Since the SBOM is an official delivery, it needs to be verifiable and signed which provides trust in the delivery.
