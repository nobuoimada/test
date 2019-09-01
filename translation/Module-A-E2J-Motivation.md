(slide 1)
# FOSSology: License Analysis

Part I: Why do we need to look at licenses?

(slide 2)
## What is Open Source Software Licensing?

Basics about Licensing
- Obligations
- Restrictions
- Rights

Example for GPL version 2.0 (selection)
- Obligations
    - Include original source, copyrights
    - Include license
- Restrictions
    - Cannot be held liable
- Rights
    - Modify
    - Distribute

Further reading:
- The Linux Foundation provides a public training including basics about licensing https://training.linuxfoundation.org/linux-courses/open-source-compliance-courses/compliance-basics-for-developers
- The TLDR Legal pages at https://tldrlegal.com/ provide OUTLINES about license obligations, restrictions, rights

(slide 3)
## Open Source Software Licenses

Open Source Licenses
- There are many of them
- “License proliferation”
- They can be categorized, but requires effort and assessment
    - Copyleft vs. permissive licenses
    - GPL version 2 compatibility
    - Patent left effect
    - … a lot more possible.

Further reading:
- See the SPDX License List pages at http://spdx.org/licenses/ to see a selection of popular open source licenses

(slide 4)

## Analysis – Not Only Scanning but also Concluding

### What are the goals?
It is about telling the software developers what to care for:

1. Identify obligations to fulfill, including providing for example
	a) Credits (copyrights, prominent notice)
	b) Information about licensing
	c) Source code
1. Check for license compatibility
	a) Simple example: GPL version 2 and CC-BY-SA (copyleft effect examples)
1. Be able to check desired usage
	a) Does you business case match the licensing?
	b) Is the context of usage envisaged from the OSS publishers

Further reading:
- On obligations there is the OSADL association
- They have published a set of obligation data for various licenses: https://www.osadl.org/Access-to-raw-data.oss-compliance-raw-data-access.0.html


(slide 5)
# FOSSology: Component Analysis

Part II: Motivating Examples

(slide 6)
## Examples for Licensing – Clarification Needed

(all examples from the same package zlib-1.2.8.tar.gz)

- These real world examples show references to a licensing statement, which is elsewhere
- A scanner for text cannot generally determine the licensing from these files without capturing the particular occurrence and context
- A person is required to clarify the licensing 


(slide 7)
## Examples for Licensing – Clarification Needed 2

(from zlib-1.2.8.tar/ zlib-1.2.8/ contrib/ amd64/ amd64-match.S)

Another real world example:
- What was meant to be fun (or a political statement), is difficult for license analysis
- Question: Can this be ignored or shall the origination check for ownership of referred parafernalia?

(slide 8)
## Examples for Licensing – Clarification Needed 3
(TrueCrypt 7.1a Source.zip/ Common/ Cache.c)

Another real world example:
The text is actually occurs with this formatting in file
Very special occurrence in fact that requires review

(slide 9)
## Examples for Licensing – Clarification Needed 4

(TrueCrypt 7.1a Source.zip/ Crypto/ AesSmall.h)

Another real world example:
- How does the organization decide which license to choose
- There may be an external reason for choosing either one or the another

(slide 10)
## Examples for Licensing – Attention Needed 5

Another real world example:
- It is actually based on an MIT license text
- MIT license: very popular and permissive
- Added two conditions inside the original license text
(not so permissive)
- Very hard to identify with regular expression matching

(slide 11)
## Some Example from out in the wild (1)

(slide 12)
## Some Example from out in the wild (2)

(slide 13)
## Examples for Copyrights – Clarification Needed

1. Examples of incomplete statements
    a) Year missing
    b) Individual or organization missing
1. Copyright notice missing
    a) Again: What about orphaned files? Who wrote them? 
1. Ambiguous copyright information for every file
    a) Copyright or copyright sign, year or years, individual or organization
    b) Common understanding is covered by the Berne convention
1. How about authored, thanks to, contributed?
    a) They do not express copyright, consult your legal counsel for guidance in these cases


- The Wikipedia article on the Berne convention presents the basics and origin about copyright law https://en.wikipedia.org/wiki/Berne_Convention

(slide 14)
# FOSSology: Component Analysis
Part III: Scope and Terminology

(slide 15)
## Analyzing the License Situation of a Component

Analysis & Clarification of Compliance Issues

1. Analyzing Component vs. Usage Analysis
    a) On a per component basis
    b) Shall not consider a particular usage case – enabling reuse of license analysis
    c) Opposed the usage clearing: considers all involved components

(slide 16)
## Misconceptions: Other Terms and Analysis

Component Analysis & Clarification of Component License Condition

1. License Analysis

    a) How to call what: license analysis vs. component analysis?
    b) There is also clarifying license terms required, for example: new licenses, rare licenses, licenses written for the US law, used in Europe, etc.

1. Looking at OSS components or your own product?
    a) For re-using license analysis: going OSS component by OSS component
    b) An analysis on product level considers incompatible
licensing or business case compatibility

(slide 17)
## License Analysis of a Component - Summary

1. Overall goals
    a) Comply with OSS community and mitigate risk
    b) Help the engineering with definitive instructions
    c) Building a list of reusable assets, requires usage independent clearing of component
1. How to perform a component analysis for licensing
    a) Reviewing file notices
    b) Reviewing license texts
    c) Determining the exact text for obligations (rights, restrictions)
    d) Identify new licenses
    e) License clarification required?
     - OSS Expert group available in organisation
     - Legal advice required 

- The FOSSology project enables the tool-based identification of licenses:
    - Finding license relevant texts
    - Aggregation in a hierarchy
    - Highlighting text occurrences
    - Identifying wording differences compared with reference texts
    - Searching for licensing phrases
    - Reporting of found licenses

(slide 18)
## Thank you for your attention!

(C) 2016-2018  Siemens AG, The Linux Foundation


CC-BY-SA 4.0
https://creativecommons.org/licenses/by-sa/4.0/

Internet
https://www.fossology.org

Github
https://github.com/fossology/fossology

Further Links
https://www.spdx.org
https://www.openchainproject.org
https://github.com/sw360/sw360portal


(C) 2016-2018  Siemens AG, The Linux Foundation - CC-BY-SA 4.0
