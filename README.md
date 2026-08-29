### Hosting-Static-Website

This SOP explains how to create an Azure resource group, configure a storage account for static website hosting, upload website files to the $web container, and verify the site using the generated primary endpoint. It also includes how to access and edit the uploaded site files later if changes are needed.

### Key Steps

### Link to Loom

<https://loom.com/share/5986535597694b65854d685e6644d144>

**1. Create a Resource Group in Azure** [0:08](https://loom.com/share/5986535597694b65854d685e6644d144?t=8)

- In the Azure portal, create a **new resource group** to keep all related resources organized.
- Use a clear, descriptive name so the project is easy to identify later.
- Wait for the resource group to finish loading/creating before moving to the next step.


**2. Create a Storage Account for the Static Website** [0:34](https://loom.com/share/5986535597694b65854d685e6644d144?t=34)

- While the resource group is loading, create a **Storage Account**.
- Choose **Blob Storage** because the website files will be stored there.
- Confirm the storage account is created successfully before continuing.

 

**3. Enable Static Website Hosting** [1:36](https://loom.com/share/5986535597694b65854d685e6644d144?t=96)

- Open the newly created storage account.
- Find and select the **Static website** option.
- Click **Enabled** to turn on static website hosting.
- Set the default document names: 
  - **index.html** as the main entry page.
  - **404.html** as the error page.
- Save the configuration so Azure generates the website hosting setup.

 

**4. Prepare the Website Code** [2:30](https://loom.com/share/5986535597694b65854d685e6644d144?t=150)

- Create or open the website code locally.
- Make sure the main HTML file is saved as **index.html**.
- Save your changes before uploading.
- Keep the file ready for upload to Azure Blob Storage.

 

**5. Upload the Website Files to the $web Container** [3:01](https://loom.com/share/5986535597694b65854d685e6644d144?t=181)

- In the storage account, go to **Blob Storage** and open the **Containers** section.
- Select the **$web** container, which is used for static website content.
- Click **Upload**.
- Browse to the saved website file location and select **index.html**.
- Click **Upload** again to complete the transfer.
- Refresh the container view to confirm the file appears in the list.

 

**6. Verify the Website Using the Primary Endpoint** [3:56](https://loom.com/share/5986535597694b65854d685e6644d144?t=236)

- Return to the static website settings and locate the **Primary endpoint**.
- Open the endpoint URL in a browser.
- Confirm the website loads correctly from Azure.
- If the page displays as expected, the static website is successfully hosted.

 

**7. Edit the Website After Upload if Needed** [4:09](https://loom.com/share/5986535597694b65854d685e6644d144?t=249)

- In the uploaded file list, locate the file you want to change.
- Use the **three-dot menu** next to the file.
- Select **View/Edit** to open the file contents.
- Make the required changes and save them.
- Recheck the website through the primary endpoint to confirm the update is live.

### Cautionary Notes

- Ensure the static website feature is enabled before uploading files; otherwise, the site will not serve correctly.
- The main file must be named **index.html** for the website to load properly.
- Upload files to the **$web** container only; other containers will not serve as the static website root.
- Always save changes after editing files so updates are reflected on the live site.
- Verify the primary endpoint after each major change to catch configuration issues early.

### Tips for Efficiency

- Prepare the HTML files locally before configuring Azure to reduce setup time.
- Use clear naming conventions for the resource group and storage account to simplify future maintenance.
- Keep the primary endpoint bookmarked for quick testing.
- Refresh the container view after uploads to confirm files were added successfully.
- Use the built-in View/Edit option for quick content changes instead of re-uploading files when only small edits are needed.

### Link to Loom

<https://loom.com/share/5986535597694b65854d685e6644d144>
