# Microsoft Teams Tab Authentication
This sample demonstrates how to build a custom tab for Microsoft Teams that performs OAuth against Azure AD and makes calls into the Microsoft Graph. You could change out Azure AD/Microsoft Graph for any identity provider/service. Use the following steps to run the sample:

1. Clone the repo
2. (optional) register a new Azure AD application with permissions to read the profile for the signed in user. The app should also be configured to allow implicit flow. This step is optional because the code checked in is pre-configured with a multi-tenant application that should work with any Office 365 tenant.
3. (optional) if you don't have gulp run the following command
```
npm install -g gulp
```
4. Open command prompt to root and run the following
```
npm install
gulp serve-static
```
5. Log into Microsoft Teams and select the "View Team" option in the contextual menu of a team
6. Go to the Developer tab in Team settings
7. Upload the TabPackage.zip to the Tabs in Development list
8. Go back to the Team and add the new tab to a channel and test

Note: you might need to open a browser to https://localhost:8443 to allow the untrusted https cert