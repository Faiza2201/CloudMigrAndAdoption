# 1- On-Prem infrastructure design
Here are the differents parts of our infrastructure:

<img width="374" height="388" alt="image" src="https://github.com/user-attachments/assets/092bd9cb-dd5c-4ca4-b319-523262e3c25d" />

Here we can identify resources that need to be migrated, these would be network configuration that fits IAAS, same for File storage, the web app server and Database ones would certainly fit PAAS model and finaly email that best representation would be as a SAAS model.

# 1- On-Prem infrastructure design
 ## 1. Propose of the migration strategie for each of the components
  Here is the best illustration of the migration best fit in regard of cloud model for each component:
  1. Web Application → best fit for the web App would be PAAS service, so that cloud provider would handle all what is related to VM maintenance, middlewares and the developpers can focus on coding only. This cloud-native App can be provided by Azure web App, AWS Elastic beans or Google app Engine
  2. Database → the best cloud representation for the database would be PAAS model, this helps you to work only on databases and queries while the provider will manage OS, patching, HA, scaling... This can be ofered by Azure SQL database and Azure SQL managed Instance, Amazon RDS for SQL Server/MySQL/PostgreSQL or Google Cloud SQL.
  3. File Storage → the IAAS model would fit the file storage representation in the cloud, but a PAAS model would also fit if we plan to use a cloud-native storage solution as Azure files, Amazon EFS or Google Filestore.
  4. Networking → would be represented by the Cloud-native networking
  5. Email service → as email is a fully hosted and managed software applications that users access over the internet, this last would be represented by SAAS model in cloud, we may use SES, SendGrid, ACS.
 ## 2. Considering an Hybrid migration of components
 Hybrid migration doesn't impact the production and App process and the workflow, what would be emphasysed here is that in the IAAS model the maintenance related to VM OS, patching, runtimes and so one would be on charge of the client and not the cloud provider.
 ## 3. Migration plan

  In the migration plan, here what we can consider as a step to move components to the cloud:
   Web Application → There would be some coding to consider here and to take in consideration with the development team.
   Database → there would be here minor changes on the host.
   File Storage → Would be here a Replace (Rehost)
   Networking → our network appliances would be Retired.
   Email service → Retirement of the solution that will be replaced by a cloud service.
   
<img width="391" height="260" alt="image" src="https://github.com/user-attachments/assets/7344e33c-5143-48bc-b69e-125635349c88" />
