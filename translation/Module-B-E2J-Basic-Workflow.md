(slide 1)
# FOSSology: Introduction and Basic Workflow

(slide 2)
## The Problem Actually

#### You know these examples  

Distributing open source software requires to  
- Provide licenses of involved software  
- Provide copyright statements of involved authors  
- Provide disclaimers  
- … and much more  

(slide 3)
## It is about finding licenses

#### Finding Licenses

- License texts  
- References to licenses  
- Written texts explaining licensing  
- License relevant statements  

(slide 4)
## An Example – What do we find?

#### The Example

- (Apache projects are known for homogenous licensing)  
- Such a project declares its licensing on its Website  
- However, Open Source implies using other open source  
- As such, a projects can contain also parts from other open source projects  

(slide 5)
## Using FOSSology with this Example

#### Open Source and Reuse

- It is natural that an OSS project reuses available https://github.com/fossology/fossology  
- Likely OSS from other projects is found  
- For example, FOSSology will find 25 other licensing relevant text occurrences in Apache thrift  

(slide 6)
## Using FOSSology with this Example

#### Another Example: Linux Kernel Project

- Looking at the Linux kernel will result in thousands of files containing license relevant information  
- Analyzing them yields about 30 distinctive licensing statements  

(slide 7)
## What is FOSSology?

A Web server application for license and copyright compliance of software components.  

FOSSology Project  
https://www.fossology.org/  

- Published first in 2008, GPL-2.0  
- 2015: Linux Foundation collaboration project  
- Web server based and command line interfaces  
- Scanning agents searching for license and copyright relevant hits (and more …)  
- A multi-user / multi-tenant Web UI for review organizing clearing job  

FOSSology Development  
https://www.github.com/fossology/fossology  

- Standard Web application stack:  
    - Linux, Apache 2, PostgreSQL, PHP,  
- Web-based UI in PHP, but scanners  
    - written in C / C++  
- Two ways to interact:  
    - Web user interface  
    - Command line utilities  

(slide 8)
## How does FOSSology work? – Overview 1 of 2

See more details the Basic Workflow Description: https://www.fossology.org/get-started/basic-workflow  

| Upload OSS Package  |  

- Upload an open source package to the server  
- Select scan agents that analyze the software  

| Review and Adjust (“Clearing”)  |  

- Review what scanners have found  
- Review license occurrences and correct findings if necessary  

| Generate  |  

- Generate report output  
- For example list of licenses or SPDX  

(slide 9)
## Hands-On: Basic End-to-End Workflow

Functionality  

1. Using FOSSology End-to-End  
    - From uploading …  
    - … to generating report: SPDX  
1. Uploading - offers a variety of selections  
1. Review the uploaded file in the license browser  
1. Review the found licenses in the aggregated view  
1. Do the clearing work  
1. Review the copyrights  
1. Review the Export Control and Customs (ECC)  
1. Generate desired report output  

Example  

Upload ionicons-3.0.0  
- Go to license browser by clicking upload name or selecting clearing from the action menu  
- Select “go to all …. with licenses”  
- Review licenses and apply decisions  
Select the copyright, e-mail, url section from the yellow menu bar area  
- Review copyright statements and correct in case  
Select ECC from the yellow area and review  
Go to Browse main view  
- Select the pop-up menu of the ionicons upload  

(slide 10)
## How does FOSSology work? – Overview 2 of 2

Upload Component  

- Uploading source code archive (*.zip, *.tar.gz, etc)  

Agents Scanning  

- Agents scan for license relevant text  
- Copyrights, Export Control (ECC), your keywords to look for etc.  

Review Results  

- Review scanner results for wrong license classification  
- Review other scanner findings (copyrights, ECC)  

Generate Reporting  

- Result of the “clearing”  
    - SPDX reporting  
    - Generated notice or readme file  
    - debian-copyright  

Pass Report to Client  

(slide 11)
## FOSSology Feature Overview

A Web server application for license and copyright compliance of software components.  

License Scan features  

- Regular expression scanner  
- Text similarity scanner  
- License (text) management  
- Aggregation of licenses in hierarchical view  
- License histogram  
- Supporting concluded vs. found license  
- Bulk processing of files with same licensing  
- Reusing of license conclusions  

Other features  

- Copyright, authorship statements scanner  
- Export control and customs scanner  
- Command line interfaces  
- Reporting  
    - SPDX RDF and tag-value  
    - Debian-copyright  
    - Plain text output  
- Files sorting in buckets  
- User, group and upload management  

(slide 12)
## Features: Two License Scanners: Nomos and Monk

Nomos Keywords  

- Finds all kind of license relevant texts  
- Finds unknown Licenses  

Nomos Reg. Expressions  

- Finds most license relevant texts  
- Identifies also derivatives of licenses

Bulk Phrase Matches  

- Good for finding actual licenses  
- Identifies also derivatives of licenses  

Monk Full text Matches  

- Certainty that known license text is actually found and wording is exactly reproduced  

Flexibility  

- Very imprecise  
- Does not identify license  
- High number of false positives  

- Only limited precision for identifying actual licenses  
- False positives

- Limited to known phrases only  
- Does not provide certainty about original or derivative  

- Works only on known license texts  
- Actual occurrences are minority  

Precision  

(slide 13)
## More Features in FOSSology

- Workflow integration with command line interfaces  
    - Do uploads and scans from the command line, right from your scripts  
    - Or just run individual agents (e.g. for licenses) from command line  
    - Schedule activities / integrate them into automated workflows  
- ECC (Export Control and Customs)  
    - Regular expressions searching for export control and customs  
- License data sets import and export  
    - Regular expressions searching for export control and customs  
- Buckets  
    - Define rules for files with license results for collecting them in dedicated lists / buckets  

(slide 14)
## FOSSology is Open Source

#### What happens actually?

- As an organization distributing software there is responsibility for license compliance  
- This work must be actually provided by 3rd parties as well!  
- With FOSSology, a tool is freely available supporting all kind of organizations with their license compliance efforts  
- GPL-2.0 licensed  

(slide 15)
## Overview: FOSSology Hands On

1. Basic End-to-End Workflow  
    Overview: What do I need to do actually to get the SPDX / Readme / DEP5  
1. Accelerate the File Handling  
    Using bulk scanning to correct scan results  
1. Reuse of Clearing Decisions  
    Process only differences for newer versions of a scanned component  
1. Management of Licenses  
    See the licenses and where to edit  
    Export and import more licenses  
1. Organizing the Uploads  
    Getting started with folders, uploads and access rights  
    Creating users and groups  

(slide 16)
## Thank you for your attention!
ご清聴ありがとうございました！

(C) 2016-2018  Siemens AG, The Linux Foundation


CC-BY-SA 4.0  
https://creativecommons.org/licenses/by-sa/4.0/

Internet  
https://www.fossology.org

Github  
https://github.com/fossology/fossology

もっと知りたい人は、  
https://www.spdx.org  
https://www.openchainproject.org  
https://github.com/sw360/sw360portal  


(C) 2016-2018  Siemens AG, The Linux Foundation - CC-BY-SA 4.0

