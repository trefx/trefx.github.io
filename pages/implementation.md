---
title: TRE-FX Implementations
---

## Implementation reports

Tom Giles, Jonathan Couldridge, Sam Cox, Daniel Lea, Vasiliki Panagi, Simon Thompson, Philip Quinlan (2024):  
[**TRE-FX Technical Documentation - Primary Implementation**](https://doi.org/10.5281/zenodo.10376658).  
_Zenodo_
<https://doi.org/10.5281/zenodo.10376658> (in preparation)

Blaise Thomson, Naaman Tammuz, Thomas Giles, Philip Quinlan, Carole Goble (2024):  
[**TRE-FX Technical Documentation - Bitfount Implementation**](https://doi.org/10.5281/zenodo.10376572).  
_Zenodo_
<https://doi.org/10.5281/zenodo.10376572>

Stuart Wheater, Thomas Giles, Philip Quinlan, Carole Goble (2024):  
[**TRE-FX Technical Documentation - DataSHIELD Implementation**](https://doi.org/10.5281/zenodo.10375984).  
_Zenodo_
<https://doi.org/10.5281/zenodo.10375984>

## Planned TRE-FX architecture

The below is the originally planned architecture, for the realized implementations, see reports above.

<a href="/assets/img/architecture.svg"><img src="/assets/img/architecture.svg" alt="Five Safes Queries go to Submission layer, polled by TRE polling Layer. It authenticates the query before queing it, to be picked up by the Controlled Layer inside the Trusted Research Infrastructure. The workflow is executed using WfExS (workflow execution service) with results as an RO-Crate, checked for disclosure control. Results propagate upwards to the Five Safe Results API and submitted through the Transparancy Layer to the HDR Data Use Register." /></a>

1. User submit queries as job packets in a [Five Safes RO-Crate](/5s-crate/) via an API on a publicly available Submission portal. Queries are then presented on a query queue.
2. The job packets are pulled down into a demilitarised polling zone on a TRE via a secure outbound only API connection. Connection between TREs and the Submission Layer are managed by HUTCH.
3. Job packets are authenticated and then presented on an internal queue. 
4. A second outbound only API pulls the job packets into the main Controlled zone of the TRE. 
5. The job packet is passed to WfExS which executes published approved workflows on data, generate results and adds them to the job packet, including workflow information and providence. 	
6. Subject to appropriate disclose control the job packet is returned to the TRE Polling zone and stored. 
7. Further disclosure checks are applied, and the job packet is released back to the submission layer where it is held on a results queue to be collected by the user.
8. Subject to deidentification, the job packet is also published on the HDR data use register.

### Work packages

The TRE-FX project ran for 9 months starting 2023-02-01 until 2023-09-31.

* WP1: PPIE 
* WP2: Transparency
* WP3: Microservice Development
* WP4: TRE integration
* WP5: Federated Analytics Testing
  
