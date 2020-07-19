# Approach to convert a Industry 3.0 device to **Industry 4.0**
1. Data flows from **sensors/actuators** through field bus to **Controllers**
2. From PLCs to **Open Platform Communications** through Control Bus
3. Next it is sent to **IOT Gateway**
4. Then all the information goes to **IOT Hub**
5. Here the data can be **Moniterised, analysed and etc**

[![](https://mermaid.ink/img/eyJjb2RlIjoiZ3JhcGggVERcbkFbU2Vuc29ycyBBY3R1YXRvcnNdLS0-fEZpZWxkIEJ1c3wgQihbUExDLENOQyxETFNdKVxuQiAtLT58Q29udHJvbCBCVVN8IEMoW09QQyBTRVJWRVJdKVxuQyAtLT58T1BDIFVBLCBPUEMgREF8IEQoSU9UIGdhdGV3YXkpXG5EIC0tPnxNUVFUIENvQVAgV0VCU09DS0VUfCBpZDFbKElPVCBIVUIpXSIsIm1lcm1haWQiOnsidGhlbWUiOiJmb3Jlc3QifSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoiZ3JhcGggVERcbkFbU2Vuc29ycyBBY3R1YXRvcnNdLS0-fEZpZWxkIEJ1c3wgQihbUExDLENOQyxETFNdKVxuQiAtLT58Q29udHJvbCBCVVN8IEMoW09QQyBTRVJWRVJdKVxuQyAtLT58T1BDIFVBLCBPUEMgREF8IEQoSU9UIGdhdGV3YXkpXG5EIC0tPnxNUVFUIENvQVAgV0VCU09DS0VUfCBpZDFbKElPVCBIVUIpXSIsIm1lcm1haWQiOnsidGhlbWUiOiJmb3Jlc3QifSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)

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