# Approach to convert a Industry 3.0 device to **Industry 4.0**
1. Data flows from **sensors/actuators** through field bus to **Controllers**
2. From PLCs to **Open Platform Communications** through Control Bus
3. Next it is sent to **IOT Gateway**
4. Then all the information goes to **IOT Hub**
5. Here the data can be **Moniterised, analysed and etc**

[![](https://mermaid.ink/img/eyJjb2RlIjoiZ3JhcGggVERcbkFbU2Vuc29ycyBBY3R1YXRvcnNdLS0-fEZpZWxkIEJ1c3wgQihbUExDLENOQyxETFNdKVxuQiAtLT58Q29udHJvbCBCVVN8IEMoW09QQyBTRVJWRVJdKVxuQyAtLT58T1BDIFVBLCBPUEMgREF8IEQoSU9UIGdhdGV3YXkpXG5EIC0tPnxNUVFUIENvQVAgV0VCU09DS0VUfCBpZDFbKElPVCBIVUIpXSIsIm1lcm1haWQiOnsidGhlbWUiOiJmb3Jlc3QifSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoiZ3JhcGggVERcbkFbU2Vuc29ycyBBY3R1YXRvcnNdLS0-fEZpZWxkIEJ1c3wgQihbUExDLENOQyxETFNdKVxuQiAtLT58Q29udHJvbCBCVVN8IEMoW09QQyBTRVJWRVJdKVxuQyAtLT58T1BDIFVBLCBPUEMgREF8IEQoSU9UIGdhdGV3YXkpXG5EIC0tPnxNUVFUIENvQVAgV0VCU09DS0VUfCBpZDFbKElPVCBIVUIpXSIsIm1lcm1haWQiOnsidGhlbWUiOiJmb3Jlc3QifSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)

**Example of a device**    
[![](https://mermaid.ink/img/eyJjb2RlIjoiZ3JhcGggVERcbkEoKERlbHRhLU1ldGVyKSk6OjpjbGFzczEtLT58UlM0ODV8IEIoW1Jhc3BiZXJyeSBwaWUgM10pXG5CIC0tPnxSSjQ1fCBDW1BDXTo6OmNsYXNzNCAtLT58TVFRVCBDb0FQfCBEWyhJb1QgQ2xvdWQpXTo6OmNsYXNzNVxuQjo6OmNsYXNzMyAtLT58TVFRVCBXRUJTT0NLRVR8RCAtLT4gQ1xuRSgoRW5lcmd5KSkgLS0-QVxuRigoQ3VycnJlbnQpKSAtLT5BXG5mKChWb2x0YWdlKSkgLS0-QVxuICAgICAgY2xhc3NEZWYgY2xhc3MxIGZpbGw6I0Y0QTQ2MCxzdHJva2U6IzMzMyxzdHJva2Utd2lkdGg6NHB4O1xuICAgICAgY2xhc3NEZWYgY2xhc3MyIGZpbGw6I0ZGREFCOSxzdHJva2U6IzMzMyxzdHJva2Utd2lkdGg6NHB4O1xuICAgICAgY2xhc3NEZWYgY2xhc3MzIGZpbGw6XHRcdCM2NDk1RUQsc3Ryb2tlOiMzMzMsc3Ryb2tlLXdpZHRoOjRweDtcbiAgICAgIGNsYXNzRGVmIGNsYXNzNCBmaWxsOiNmOWYsc3Ryb2tlOiMzMzMsc3Ryb2tlLXdpZHRoOjRweDtcbiAgICAgIGNsYXNzRGVmIGNsYXNzNSBmaWxsOlx0I0ZGQjZDMSxzdHJva2U6IzMzMyxzdHJva2Utd2lkdGg6NHB4O1xuICAgIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQifSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoiZ3JhcGggVERcbkEoKERlbHRhLU1ldGVyKSk6OjpjbGFzczEtLT58UlM0ODV8IEIoW1Jhc3BiZXJyeSBwaWUgM10pXG5CIC0tPnxSSjQ1fCBDW1BDXTo6OmNsYXNzNCAtLT58TVFRVCBDb0FQfCBEWyhJb1QgQ2xvdWQpXTo6OmNsYXNzNVxuQjo6OmNsYXNzMyAtLT58TVFRVCBXRUJTT0NLRVR8RCAtLT4gQ1xuRSgoRW5lcmd5KSkgLS0-QVxuRigoQ3VycnJlbnQpKSAtLT5BXG5mKChWb2x0YWdlKSkgLS0-QVxuICAgICAgY2xhc3NEZWYgY2xhc3MxIGZpbGw6I0Y0QTQ2MCxzdHJva2U6IzMzMyxzdHJva2Utd2lkdGg6NHB4O1xuICAgICAgY2xhc3NEZWYgY2xhc3MyIGZpbGw6I0ZGREFCOSxzdHJva2U6IzMzMyxzdHJva2Utd2lkdGg6NHB4O1xuICAgICAgY2xhc3NEZWYgY2xhc3MzIGZpbGw6XHRcdCM2NDk1RUQsc3Ryb2tlOiMzMzMsc3Ryb2tlLXdpZHRoOjRweDtcbiAgICAgIGNsYXNzRGVmIGNsYXNzNCBmaWxsOiNmOWYsc3Ryb2tlOiMzMzMsc3Ryb2tlLXdpZHRoOjRweDtcbiAgICAgIGNsYXNzRGVmIGNsYXNzNSBmaWxsOlx0I0ZGQjZDMSxzdHJva2U6IzMzMyxzdHJva2Utd2lkdGg6NHB4O1xuICAgIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQifSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)
## Architecture of AWS
*  **Solution Architecture**:
The following diagram illustrates the high-level end-to-end solution described in this multi-part post along with the AWS services used in the solution.


![cloud](https://d2908q01vomqb2.cloudfront.net/f6e1126cedebf23e1463aee73f9df08783640400/2019/11/29/image-1.png)
*  **Walkthrough**

   There are five sections in this step-by-step walk-through:

   *  Prerequisites
   *  Setting up KEPServerEX with sample data
   *  Setting up AWS IoT Greengrass and deploying AWS IoT SiteWise gateway software
   *  Modeling your assets in AWS IoT SiteWise
   *  Setting up AWS IoT SiteWise gateway for data ingestion