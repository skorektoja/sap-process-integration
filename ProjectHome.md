This project will provide usefull tools to work with SAP's SOA Middleware and Integration Platform: SAP Process Integration (SAP PI) or formerly know as SAP XI (SAP Exchange Infrastructure)

The project contains currently one tool:

  * Http Post Tool with local storage [Usage](http://code.google.com/p/sap-process-integration/wiki/Usage), [Download](http://code.google.com/p/sap-process-integration/downloads/detail?name=HttpPostTool_v1.zip&can=2&q=). This tool can be used to post mutiple XML Messages to PI for test purposes. The current version also supports SAP PI 7.3's Java based HTTP Adapter with GET/POST requests.

**Note!** _The Http Post Tool worked quite well with older browser generations. Due to more strict cross domain checking (especially in Firefox), i am currently working on a rewrite._

  * Audit Logger Adapter Module: Trace Payloads as they flow in or out of your adapter engine. This is foremost important with the new AEX setups and with synchronous messages you want to trace on specific channels. Mainly for testing/debuging issues.
In order to use it, build an ear file with these projects and deploy it on your SAP Java Web AS on which PI is running. You should be able to insert the module then within the channel modules with the lookup name "AuditLogger"

_italic_
Note: This will increase your memory for auditlogs when used for big payloads, so use with care!
_italic_

Download EJB/EAR NWDS project (simply unzip): http://code.google.com/p/sap-process-integration/downloads/detail?name=AuditLogger.zip&can=2&q=#makechanges