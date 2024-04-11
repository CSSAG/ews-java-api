# EWS JAVA API

The Exchange Web Services (EWS) Java API provides a managed interface for developing Java applications that use EWS.
By using the EWS Java API, you can access almost all the information stored in an Office 365, Exchange Online, or Exchange Server mailbox. However, this API is in sustaining mode, the recommended access pattern for Office 365 and Exchange online data is [Microsoft Graph](https://graph.microsoft.com)

Please see the [Getting Started Guide](https://github.com/OfficeDev/ews-java-api/wiki/Getting-Started-Guide) on the official wiki for an introduction to this library.


**Project structure:**
- fork from [ews-java-api](https://github.com/OfficeDev/ews-java-api)

**Notice:**
- If you are not using the company email on github, you have to pay attention to the following
- You can use eclipse to commit with your company email/name
- You have to push with commandline, because there will be a promt to login in github, this feature is lacking in eclipse

**Build:**
- To create a new version of the ews-java-api.jar, first change the version number in `gradle.properties`. At the beginning there must always be **2.1.***
- Ideally, check that all tests have been passed. To this call `.\gradlew build`
- call `.\gradlew publish -Plocalrepo` to create a new version to the local Maven Repository build/maven
- call `.\gradlew publish` to upload the new version to the nexus