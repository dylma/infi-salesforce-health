# infi-salesforce-health
Infinitus Mulesoft Repository for Salesforce Health Cloud APIs

This repo contains all the experience, process, and system APIs for inerfacing with Salesforce Health Cloud.  These APIs are re-usable assets and will be published to Anypoint Exchange.

[SetUp]
1. Import this repository into Anypoint Studio
2. Double check the connection details in the secure yaml file(s) are still valid
3. Run the application locally or deploy it to CloudHub
4. Use an API client to test the Mulesoft APIs

[DesignDocument]
[infi-salesforce-health Design Doc.pdf](https://github.com/user-attachments/files/18519511/infi-salesforce-health.Design.Doc.pdf)

[Assumptions]
1. We're assuming the client can send in bulk
2. No transformation mapping sheet was provided so we inferred the transformation between source and target systems

[Challenges]
1. Salesforce Administration.  Had to create robot users, connected app, permission sets, and profiles and assign them appropriate to be able to invoke the Health Cloud platform APIs
2. ID from CareBenefitVerifyRequest creation is hidden in mulesoft response (workaround needed to fetch this)
