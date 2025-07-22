# _PerformanceManagement
UserDemand for MW SDN based Performance Management

### Scope  
The current ComarchOSS based Performance Management is to be replaced by a set of microservices integrated into the application layer of the MW SDN domain.  

The API Gateway will be the demarkation between the SDN domain and external applications/tools, which will be consuming the provided MW performance data.  
Currently the following consumers are within the scope:  
- [Netexplorer](./additional_description/Netexplorer.md)
- [APT](./additional_description/APT.md)
- [Mycom](./additional_description/Mycom.md)

Depending on the needs of the different consumers, different services for data provisioning can be exposed.  
While devices only provide raw data, implementing (simple) aggregations or formulas would also be possible if needed.  
