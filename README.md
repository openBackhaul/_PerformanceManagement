# _PerformanceManagement
UserDemand for an interface that is streaming MW Performance Data  

### Driver  
Replacement of ComarchOSS  

### In Scope
- Interface (exposed at API GW) that is streaming (to be agreed with consumers) performance data to the following out-of-domain software:  
  - [APT](./additional_description/APT.md)
  - [Mycom](./additional_description/Mycom.md)
  - [Netexplorer](./additional_description/Netexplorer.md)
- The data  
  - shall be collected with a high level of completeness  
  - shall be harmonized in its format and its semantical meaning  
  - relate to time periods that have been completed in past (historical performance values)  
  - shall be filtered from obviously unrealistic values  
- Activate the performance measurement function on the devices wherever required
- Aggregate data and calculate key performance indicators (e.g., interval capacity) as far as they are harmonized across the consumers  
- Complement with configuration and status data as far as can be harmonized across the consumers  

### Out of Scope
- Providing current performance and counter values  
- Long term storage of performance data  
- Graphical user interface for analyzing performance data  
- Providing an interface for ad-hoc definition of aggregation methods and analysis metrics

