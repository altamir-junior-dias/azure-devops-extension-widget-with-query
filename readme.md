# Development Setup

1. Install **Node.js**: https://nodejs.org/en/download/

2. Install **Node CLI for Azure DevOps**: https://www.npmjs.com/package/tfx-cli

3. Create a **Marketplace Publisher**: https://marketplace.visualstudio.com/manage/createpublisher


# Widget

1. Download this repository

2. Install **Node packages** on command line:
   ```
   npm install
   ```

3. Change the **publisher** property on **vss.extension.json** file with the your published id


# Packaging

### Creating the package from the current version in the command line:
```
tfx extension create
```

### Creating the package increasing the version in the command line: 
```
tfx extension create --rev-version
```

# Publishing

### First package

1. Go the the **Manage Publishers & Extensions** page on **Marketplace**: https://marketplace.visualstudio.com/manage

2. Select the **Publisher** on the left panel

3. Push the **+ New Extension** button and select **Azure DevOps**

4. Select the file generated with the **TFX client**

5. Wait package loading

6. Push the **...** button on the **extension** and select **Share/Unshare** option

7. Push the **+ Organization** and inform the organizarion url

8. Go to your Azure DevOps organization settings page: https://dev.azure.com/YOUR_ORGANIZATION/_settings

9.  Push **Extensions** on the left panel and click on **Shared** tab on the main panel

10. Clique on Extension line and push **Install** button

11. On the **Marketplace Azure DevOps Extension Instalation** page select the organization and push **Install** button

> You need to have be on **Project Collection Administrators** permissions group: https://dev.azure.com/YOUR_ORGANIZATION/_settings/groups to run steps from 7 to 11
>
> Done! Now you can use the widget in a Azure DevOps Dashboard

### Updating package

1. Go the the **Manage Publishers & Extensions** page on **Marketplace**: https://marketplace.visualstudio.com/manage

2. Select the **Publisher** in the left panel

3. Push the **...** button on the **extension** and select **Update** option

4. Select the file generated with the **TFX client**

5. Wait package loading
