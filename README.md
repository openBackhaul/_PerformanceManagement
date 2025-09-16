# _PerformanceManagement  
UserDemand for an interface that is streaming MW Performance Data  

### Driver  
Replacement of ComarchOSS  

### Scope to be delivered in the first three consecutive iterations  

- Interface (exposed at API GW) that is streaming (to be agreed with Consumers) performance data to the following out-of-domain software:  
  - [APT](./additional_description/APT.md)  
  - [Netexplorer](./additional_description/Netexplorer.md)  
  - [Mycom](./additional_description/Mycom.md) (to be clarified)  
  - TechnologyDataLake (to be clarified)  

- Functions to be provided by the PM Interface:  
  - AirInterface (microwave radio interface) and EthernetContainer (Layer 2) shall be covered  
  - Regular uploading:  
    - The PM data shall be collected from all connected devices and be forwarded to the Consumers (see above list of out-of-domain software)  
    - In case of incompleteness, it shall be autonomously attempted to complete the data  
    - The PM data shall be provided with a maximum delay (age of the oldest value set) of 6 hours  
      (an improvement to a maximum delay of 3 hours shall be attempted)  
  - On-demand upload of latest PM data of individual traffic interfaces shall be supported  
  - Plausibility:  
    - Uploaded PM data shall be checked for plausibility  
    - Unplausible data shall be replaced or deleted according to generic rules  
    - Documentation of these generic rules shall be made available to the users  
  - Semantic:  
    - The semantical meaning of data must be defined and documented  
    - Documentation of this meaning shall be made available to the users  
    - Data shall be harmonized in its format and its semantical meaning  
  - Activation on the device:  
    - Measurement of PM data shall be autonomously activated on active traffic interfaces  
    - Measurement of PM data shall be autonomously de-activated on inactive traffic interfaces  
  - Capability:  
    - Provide information about the individual traffic interface's capabilities for providing individual performance values  
      (ONF default values and Capability information is used to determine the interface's capabilities)  
  - Aggregation:  
    - Calculation of derived KPIs shall be supported (as far as they get used by the majority of Consumers)  
  - Completion:  
    - Complement with configuration data as far as it can be harmonized across the Consumers  
  - Service Quality Monitoring:  
    - Statistics about the completeness and quality of the PM data shall be provided  

### Scope to be delivered in a future fourth iteration  
- Semantical harmonization of PM data deformed by PowerSaving  

### Out of Scope
- Providing current performance and counter values  
- Long term storage of performance data  
- Graphical user interfaces for analyzing performance data  
- Providing an interface for ad-hoc definition or change of aggregation methods and analysis metrics  
