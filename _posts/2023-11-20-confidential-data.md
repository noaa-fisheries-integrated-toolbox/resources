---
title: "Resources for working with sensitive information"
excerpt: "Helpful links for working with secrets and confidential data"
date: 2023-11-20
toc: true
categories:
  - NOAA Resources
tags:
  - git
  - GitHub
  - software user resources
  - developer resources
---

## What is sensitive information and confidential data?

There are many types of sensitive information within our work systems. This includes usernames, passwords, login information, port numbers, IP addresses, server names, Application Programming Interface (API) keys, Personal Identifiable Information (PII), Business Identifiable Information (BII), and confidential data. Confidential data could include information that must be protected under a data sharing agreement, grant, or contract; NOAA Fisheries also has very specific kinds of confidential information as defined by the [Magnuson-Stevens Fishery Conservation and Management Act (MSA)](https://www.fisheries.noaa.gov/topic/laws-policies/magnuson-stevens-act), which we refer to as MSA confidential data. There are many laws, regulations, and policies that determine how each of these types of protected information should be handled. Further, each region and Science Center has various policies and procedures about how to handle this information.

Working with sensitive information can cause challenges when working on GitHub, where sensitive information should **never** be stored, even if your repository is private. Likewise, care must be taken when creating public products from summarized confidential data.

Luckily, there are resources to help keep many types of sensitive information protected.

## For R users: Confidentiality Confidence Builder

Ady Rios (SEFSC) put together this [Confidentiality Confidence Builder](https://github.com/nmfs-opensci/Confidentiality-Confidence-Builder) to learn tools and install safeguards to avoid pushing passwords or other sensitive information onto GitHub.

## Preventing accidental commits of confidential data in the GitHub Guide

The NOAA Fisheries Open Science GitHub Best Practices Guide provides some [tips for avoiding accidental commits containing confidential data](https://nmfs-opensci.github.io/GitHub-Guide/#preventing-inadvertent-committing-of-secrets-or-credentials-to-github).

## GitHub: secret scanning and push protection

For public repositories on GitHub, [secret scanning](https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning#about-secret-scanning-alerts-for-users) can be turned on to identify common sensitive information patterns quickly. There is also an option to block commits that contain secrets. Learn more on how to [set this up](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository/managing-security-and-analysis-settings-for-your-repository#enabling-or-disabling-security-and-analysis-features-for-public-repositories).

## Community support for working with sensitive information

Reaching out to the [NMFS R User Group](https://nmfs-ost.github.io/noaa-fit-resources/noaa%20resources/nmfs-r-ug-calendar/) with questions can help you connect with others in NOAA Fisheries who are processing confidential data.

## MSA Confidential Data

There are two clauses in MSA that describe MSA confidential data: _1.) "Any information submitted to the Secretary, a State fishery management agency, or a marine fisheries commission by any person in compliance with the requirements of this Act shall be confidential and shall not be disclosed"_ and _2.) "Any observer information shall be confidential and shall not be disclosed"_.

In addition to those definitions, MSA also provides exceptions for the release of _information submitted to the Secretary, management plan development, monitoring, or enforcement_:
(A) to Federal employees and Council employees who are responsible for fishery management plan development, monitoring, or enforcement;
(B) to State or Marine Fisheries Commission employees as necessary to further the Department’s mission, subject to a confidentiality agreement that prohibits public disclosure of the identity of business of any person;
(C) to State employees who are responsible for fishery management plan enforcement, if the States employing those employees have entered into a fishery enforcement agreement with the Secretary and the agreement is in effect;
(D) when required by court order;
(E) when such information is used by State, Council, or Marine Fisheries Commission employees to verify catch under a limited access program, but only to the extent that such use is consistent with subparagraph (B);
(F) when the Secretary has obtained written authorization from the person submitting such information to release such information to persons for reasons not otherwise provided for in this subsection, and such release does not violate other requirements of this Act;
(G) when such information is required to be submitted to the Secretary for any determination under a limited access program; or 
(H) in support of homeland and national security activities, including the Coast Guard’s homeland security missions as defined in section 888(a)(2) of the Homeland Security Act of 2002 (6 U.S.C. 468(a)(2)). 

And the exceptions for _information collected by observers are_:
(A) as authorized by a fishery management plan or regulations under the authority of the North Pacific Council to allow disclosure to the public of weekly summary bycatch information identified by vessel or for haul-specific bycatch information without vessel identification;
(B) when such information is necessary in proceedings to adjudicate observer certifications; or
(C) as authorized by any regulations issued under paragraph (3) allowing the collection of observer information, pursuant to a confidentiality agreement between the observers, observer employers, and the Secretary prohibiting disclosure of the information by the observers or observer employers, in order—
(i) to allow the sharing of observer information among observers and between observers and observer employers as necessary to train and prepare observers for deployments on specific vessels; or
(ii) to validate the accuracy of the observer information collected.

As of this date, the only guidance we have about how to protect MSA confidential data is: 
"The Secretary shall, by regulation, prescribe such procedures as may be necessary to preserve the confidentiality of information submitted in compliance with any requirement or regulation under this Act, except that the Secretary may release or make public any such information in any aggregate or summary form which does not directly or indirectly disclose the identity or business of any person who submits such information. Nothing in this subsection shall be interpreted or construed to prevent the use for conservation and management purposes by the Secretary, or with the approval of the Secretary, the Council, of any information submitted in compliance with any requirement or regulation under this Act or the use, release, or publication of bycatch information pursuant to paragraph (2)(A)."

The **Confidentiality Confidence Builder** describes a few tricks to avoid pushing MSA confidential data to GitHub, but it requires more manual diligence than protecting other types of sensitive information like passwords or private links. There are many scientists at NOAA Fisheries that have designed workflows based on processing confidential fisheries data.

## Guidance for handling sensitive information and confidential data

A new proposed rule is expected that will direct the agency to create more thorough and transparent guidance for handling confidential data. Until that rule publishes, it is the user's responsibility to protect sensitive information and at the discretion of each FMC to establish their own procedures. There are some [guidelines](https://drive.google.com/drive/folders/1cmiHnKCk-2N6WbsPX2kb8DV3DZympbzQ) (NOAA Internal Only).

*Thanks to Erin Steiner (NWFSC) and Molly Stevens (SEFSC) for authoring this post!*