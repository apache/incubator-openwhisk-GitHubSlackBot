# GitHubSlackBot using IBM Bluemix

## Step 1: Create Cloudant Service - GitHubSlackBotCloudant

If you don't have one already, create a new Cloudant NoSQL database by following tutorial on [Creating a Cloudant instance on Bluemix](https://console.ng.bluemix.net/docs/services/Cloudant/tutorials/create_service.html#creating-a-cloudant-instance-on-bluemix) or [GitHub IBM Bluemix docs](https://github.com/IBM-Bluemix/docs/blob/master/services/Cloudant/tutorials/create_service.md).

Also, [create a new database](images/Step1-CreateANewDatabase.png) if you don't have one.

## Step 2: Create Cloudant Package Binding - TrackPRsInCloudant

On IBM Bluemix portal, select **"Browse Public Packages"** to create a new cloudant package.

![Browse Public Package](images/Step2-BrowsePublicPackage.png)

Select **"Cloudant"**:

![Cloudant](images/Step2-PackageCatalog.png)

Select **"Create document"** action:

![Create Document](images/Step2-CloudantPackageSelectAction.png)

Select Cloudant instance we just created in previous step named **"GitHubSlackBotCloudant"** and database.

![Coudant Package Binding](images/Step2-NewPackageBinding.png)

It creates a new package **"GitHubSlackBotCloudant"** and you can view the details:

![Cloudant Package Binding Settings](images/Step2-PackageBindingSettings.png)

## Step 3 - Create an Action - track-pull-requests

![Track Pull Requests](images/Step3-CreateAnAction.png)

Creating an action here results in a track-pull-requests.js file with:

![Track Pull Requests](images/Step3-CreateAnActionEdit.png)

Now, copy code from [track-pull-requests.js](../openwhisk/actions/js/track-pull-requests.js) and paste it here.

![Track Pull Requests](images/Step3-TrackPullRequests.png)

