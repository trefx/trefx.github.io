---
title: TRE-FX Implementation plan
---

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

The TRE-FX project runs for 9 months starting 2023-02-01 until 2023-09-31.

Plan:

* WP1: PPIE 
  - Promote the inclusion of under-represented groups (as required)
  - ✓ Plan PPIE engagement events for external audiences 
  - Provide bespoke support to peoples (as required)
  - Promote public engagement work across TRE-FX
  - Host PPIE engagement events for external audiences 
  - Deliver a PPIE video discussing the implementation
* WP2: Transparency
  - ✓ Develop a [Five Safes RO-Crate](/5s-crate/)
  - ✓ Plan [workshop](/2023-07-11-tre-stakeholder-workshop) to explore Five Safes RO-Crate requirements with all Stakeholders
  - Develop a whitepaper based on the Five Safes RO-Crate 
  - ✓ Review the current mechanisms of accessing the HDR Data Use Register 
  - Develop HDR data use register to accept Five Safes RO-Crate 
  - ✓ Deliver a workshop on RO-Crate profile requirements with external Stakeholders
  - Deliver the whitepaper based on the Five Safes RO-Crate 
  - Deliver HDR data use register for Five Safes RO-Crate API integration 
* WP3: Microservice Development
  - Development of Controlled layer APIs and microservices 
  - ✓ Development of TRE polling layer  APIs and microservices
  - ✓ Development of Submission layer APIs and microservices
  - Continued development and bug fixing
  - Deliver working version of polling and controlled layer APIs and microservices 
  - Deliver working version of submission layer APIs and microservices
* WP4: TRE integration
  - ✓ Informed system design of reference implementation
  - Review final release of reference implementation with TREs and other Stakeholders
  - Deploy the API and microservices architecture on TREs
  - Review architecture implementation with external Stakeholders
  - TRE polling and controlled layer components deployed across the TREs
  - Outbound communication with submission layer established
* WP5: Federated Analytics Testing
  - Development and testing of federated analytic workflows 
  - Testing on queries on reference implementation across TREs
  - Basic user authentication and disclosure control testing
  - Publish DataSHIELD and Bitfount WfExS open-source workflow to workflowhub.eu
  - Federated analytic workflows validated on TREs
  
_Work package plans are subject to change_
