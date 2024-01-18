---
title: TRE-FX Project
---

# TRE-FX

_Delivering a federated network of TREs to enable safe analytics_

<a href="assets/img/tre-fx-logo.svg"><img src="assets/img/tre-fx-logo.svg" alt="TRE-FX, delivering a federated network of TREs to enable safe analytics" /></a>

TRE-FX was funded by UK Research & Innovation [Grant Number MC_PC_23007] as part of Phase 1 of the DARE UK (Data and Analytics Research Environments UK) programme, delivered in partnership with Health Data Research UK (HDR UK) and Administrative Data Research UK (ADR UK). 07)).

## Motivation

Trusted Research Environments (TREs) are secure locations in which data are placed for researchers to analyse. TREs host administrative data, hospital data or any other data that needs to remain securely isolated, but _it is hard for a researcher to perform an analysis across multiple TREs_, requesting and gathering the outputs from each one. This is a common problem in the UK's devolved healthcare system of geographical and governance boundaries. 

There are different ways of implementing TREs and the analysis tools that use them. A solution must be straightforward for existing, independent systems to adopt, must cope with the variety of system implementations, and must work within the "Five Safes" framework that enables data services to provide safe research access to data. 

TRE-FX assembled leading infrastructure researchers, analysis tool makers, TRE providers and public engagement specialists to streamline the exchange of data requests and results. The [Five Safes RO-Crate](/5s-crate/) standard packages up (Crates) the Objects needed for Research requests and results with the information needed for the tools and TRE providers to ensure that the crates are reviewed and processed according to Five Safes principles. TRE-FX [showed how this works](implementation) using software components and an end-to-end demonstrator implemented by a TRE in Wales. Two other TREs, in Scotland and England, are preparing to follow suit. Two analysis tool providers (Bitfount and DataSHIELD) modified their systems to use the RO-Crates. The next step is practical implementation as part of the HDR UK programme. Two large European projects will develop the approach further. 

**TRE-FX shows that it is possible to streamline how analysis tools access multiple TREs** while enabling the TREs to ensure that the access is safe. The approach scales as more TREs are added and can be adopted by established systems. Researchers will then be able to perform an analysis across multiple TREs much more easily, widening the scope of their research and making more effective use of the UK's data. If we had had this for COVID-19 data analysis, it would have super-charged researchers to be able to quickly answer pressing questions across the UK. 



## Project outputs

Carole Goble, Phil Quinlan (2024):  
[**TRE-FX: Core federation services for a federated network of TREs to enable Five Safes analytics**](https://doi.org/10.5281/zenodo.10527062).  
_DARE UK Webinar_, "[Linking Sensitive Data](https://dareuk.org.uk/linking-sensitive-data-insights-from-the-dare-uk-driver-projects-webinar-wednesday-17-january-2024-12-130pm/): Insights from the DARE UK Driver Projects", 2024-01-17  
<https://doi.org/10.5281/zenodo.10527062>

Thomas Giles, Stian Soiland-Reyes, Jonathan Couldridge, Stuart Wheater, Blaise Thomson, Jillian Beggs, Suzy Gallier, Sam Cox, Daniel Lea, Justin Biddle, Rima Doal, Naaman Tammuz, Becca Wilson, Christian Cole, Elizabeth Sapey, Simon Thompson, Professor Emily Jefferson, Phillip Quinlan, Carole Goble (2023):  
[**TRE-FX: Delivering a federated network of trusted research environments to enable safe data analytics**](https://doi.org/10.5281/zenodo.10055354).  
_Zenodo_ / DARE UK  
<https://doi.org/10.5281/zenodo.10055354>

Stian Soiland-Reyes, Stuart Wheater, Thomas Giles, Carole Goble, Philip Quinlan (2023):  
[**TRE-FX Technical Documentation - Five Safes RO-crate**](https://doi.org/10.5281/zenodo.10376350).  
_Zenodo_  
<https://doi.org/10.5281/zenodo.10376350>

Tom Giles, Jonathan Couldridge, Sam Cox, Daniel Lea, Vasiliki Panagi, Simon Thompson, Philip Quinlan (2024):  
[**TRE-FX Technical Documentation - Primary Implementation**](https://doi.org/10.5281/zenodo.10376658).  
_Zenodo_  
<https://doi.org/10.5281/zenodo.10376658>

Blaise Thomson, Naaman Tammuz, Thomas Giles, Philip Quinlan, Carole Goble (2024):  
[**TRE-FX Technical Documentation - Bitfount Implementation**](https://doi.org/10.5281/zenodo.10376572).  
_Zenodo_  
<https://doi.org/10.5281/zenodo.10376572>

Stuart Wheater, Thomas Giles, Philip Quinlan, Carole Goble (2024):  
[**TRE-FX Technical Documentation - DataSHIELD Implementation**](https://doi.org/10.5281/zenodo.10375984).  
_Zenodo_  
<https://doi.org/10.5281/zenodo.10375984>

Simone Leo, Michael R. Crusoe, Laura Rodríguez-Navas, Raül Sirvent, Alexander Kanitz, Paul De Geest, Rudolf Wittner, Luca Pireddu, Daniel Garijo, José M. Fernández, Iacopo Colonnelli, Matej Gallo, Tazro Ohta, Hirotaka Suetake, Salvador Capella-Gutierrez, Renske de Wit, Bruno de Paula Kinoshita, Stian Soiland-Reyes (2023):  
[**Recording provenance of workflow runs with RO-Crate**](https://arxiv.org/pdf/2312.07852.pdf).  
_arXiv_:2312.07852  
<https://doi.org/10.48550/arXiv.2312.07852>

## Next steps

The work on Federated Analytics and Five Safes Crate is carried forward by the HDR UK [Federated Analytics](https://www.hdruk.ac.uk/research/research-data-infrastructure/federated-analytics/) programme. See also the [Fed-A project pages](https://fed-a.org/).

The Five Safes Crate will be used by EOSC projects [EOSC-ENTRUST](https://esciencelab.org.uk/projects/eosc-entrust/) and [EVERSE](https://everse.software/) as part of secure workflow execution with [WfExS](https://github.com/inab/WfExS-backend).

## Contact

Please email `contact🤠trefx.uk` (replacing 🤠 with @) for any questions.

## Partners

* ELIXIR UK via The University of Manchester -- Carole Goble, Stian Soiland-Reyes
* University of Nottingham -- Philip Quinlan, Thomas Giles, Jonathan Couldridge
* Health Data Research UK (HDR UK) -- Emily Jefferson
* University of Dundee -- Christian Cole
* University of Swansea -- Simon Thompson
* University of Liverpool -- Rebecca Wilson
* University of Birmingham -- Elizabeth Sapey
* Bitfount -- Naaman Tammuz
* Birmingham University Hospitals NHS Trust -- Suzy Gallier
