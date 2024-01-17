---
title: What is federated analytics?
---

# What is federated analytics and what it might mean for me and my health data?

1. [What is a Trusted Research Environment (TRE)?](#tre)
2. [What are the Five Safes?](#fivesafes)
3. [What is federated analytics and why is it needed?](#federated)
4. [Advantages and disadvantages of federated analytics](#pros-and-cons)
5. [What is TRE-FX and what is the project trying to do?](#trefx)

## What is a Trusted Research Environment (TRE)? {#tre}

A Trusted Research Environment (TRE) is a highly secure computer system where health data is stored. Approved researchers can access this data remotely by using secure logins and passwords. TREs are designed to be safe, allowing only authorised individuals to access the data. 

Data cannot be added or removed without proper permissions, ensuring transparency and accountability. Multiple sources of data can be combined in a TRE to create a comprehensive dataset for research. 

Researchers can apply to access and analyse the data using computer programs they develop. While TREs are secure, organisations must still follow legal requirements when sending data to a TRE. 


## The Five Safes – what are they and why are they important? {#fivesafes}

Health data contains personal and sensitive information about people. When this data is used for research, it's crucial to handle it safely, even if it has been made anonymous. This way, we can all benefit from important research findings while respecting individuals' privacy. To ensure safe data usage, a framework called the Five Safes has been introduced.

When it is used for research, even when de-identified, it is important that the health data is used in a safe way, so that we can all benefit from the results of important research, but that the privacy of individuals is respected.   

Whenever a healthcare provider decides to share de-identified health data with a researcher, the Five Safes serve as a checklist to ensure the safety of data sharing in the best interest of the public.

The projects requesting access to the data are thoroughly evaluated to make sure that using the data will benefit and not harm the public. The individuals accessing the data undergo careful checks to ensure they have the required training and can be trusted with sensitive health information. The data itself is carefully examined to ensure that it cannot be used to identify any individual. Typically, there is a legal contract that specifies how the research results will be shared while maintaining privacy. Finally, agreements are reached on where and how the data will be accessed securely.

By following the Five Safes principles, health data can be used responsibly, leading to valuable research outcomes while safeguarding the privacy of individuals.

{% include image.html file="/assets/five-safes.png" caption="Figure 1. Five Safes: Safe Projects, Safe People, Safe Setting, Safe Output, Safe Data." alt="Safe Projects (is the requested use of the data appropriate?), Safe People (Can the researchers be trusted to ue the data appropriately?), Safe Settings (Is the data stored in a safe manner which limits the possibility for unauthorised use?), Safe Output (Could the results cause any individual to be identified, can this be minimised?), Safe Data (Is there a risk that a person could be identified from the data, can this be minimised?) " max-width="10" %}

## What is federated analytics? {#federated}

Federated analytics is a system where the data does not move, and instead the computer code the researchers write is sent to the data.

Sometimes the dataset is made from lots of pots of data in different settings.  For example, a dataset studying asthma might include data from several hospitals around the country. Instead of the hospitals sending all that data to one TRE (as described above), in federated analytics each hospital would build their own TRE and keep their data within that TRE. 

In this situation, the researcher writes their computer code and this is then sent to each TRE, analysing only the data kept in that one TRE.  The results from all the different TREs are then returned to the researchers and combined.

### Why is Federated analytics needed? {#why-federated}

Federated analytics is an innovative approach that enables data analysis and machine learning while respecting privacy and security. They allow organisations and individuals to collectively gain insights and train models without directly sharing their raw data.

The key reasons it is needed are as follows:

* This devolved approach reduces the need for large-scale data transfers, leading to faster and more efficient processing.
* Allows extraction of useful information like trends in a population’s health without revealing any individual’s specific details.
* Allows analysis on a larger and more diverse dataset, resulting in more accurate and comprehensive insights that represent a broader population or user base.
* Promotes privacy preservation, as data remains under the control of the data owners.
* Enables collaboration across organisations and individuals.
* Supports valuable insights and advancements in healthcare while safeguarding personal privacy.
* Data remains private while contributing to the collective knowledge embedded in the shared machine learning model.
* By enabling collaboration and knowledge sharing, federated analytics supports innovation and discovery. 
* Machine learning models can be trained on local devices to capture unique insights.

## What are the advantages and  disadvantages of federated analytics? {#pros-and-cons}

Advantages:

* The local organization keeps full control of the data and only has to allow access to its own data
* The data stays put and is not sent anywhere. Computer code to perform the research is sent to the data.
* The local organisation has control over who accesses the data
* The local organisation can audit and check which data is usde for which project

Disadvantages:
* As each organization only "sees" its own data, it is harder to check that the data has been collected in the same way
* It is harder to know what the whole dataset looks like, as data is spread across organizations
* The researcher does not see the data, and cannot check if the dataset has everything they need for the research projet
* It is unknown whether analysis data in "pots" and combing the results loses any meaning or accuacy
* The local organisation has to know how to build and run a TRE

## What is TRE-FX and what is the project trying to do? {#trefx}

_It is hard for a researcher to perform analysis across multiple TREs_, for example when data is to be analysed across geographical or governance boundaries, such as the devolved nature of healthcare in the United Kingdom. _Yet this ability is urgently needed_.

Analysis across a federation of TREs would enable timely analysis of UK wide scattered data to answer urgent questions, as we needed in the COVID-19 pandemic. The technologies and standards we need to be able to do this are available now. They do not need to be invented.

**TRE-FX** is assembling leading technology providers from [ELIXIR-UK](https://elixiruknode.org/) and [HDR UK](https://www.hdruk.ac.uk/), with three TRE providers and two leading analysis platforms to show through a real reference implementation how we can use secure Research Objects to move between TREs while still supporting the **Five Safes principles** that govern and protect patient data; all overseen by patient representatives.

The impact will be a step change for how researchers can safely combine data from many sources, and for how data providers from any sector can safely implement this using technology and standards we already have today.


