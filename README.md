<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Code Commits Analysis – Knowledge Base</title>
    <style>
        body { font-family: Arial, sans-serif; line-height: 1.6; margin: 40px; max-width: 900px; }
        h1 { color: #2a5d84; }
        h2 { color: #3c6e91; margin-top: 30px; }
        h3 { color: #4a7ca3; margin-top: 20px; }
        ul { margin-left: 20px; }
        p { margin-bottom: 10px; }
        hr { margin: 30px 0; border: none; border-top: 1px solid #ccc; }
        .support-note { font-weight: bold; margin-top: 40px; color: #d9534f; }
    </style>
</head>
<body>

<h1>Code Commits Analysis – Knowledge Base</h1>
<hr>

<h2>1. Application Overview</h2>

<h3>What is Code Commits Analysis?</h3>
<p>Code Commits Analysis is an application that tracks and analyzes weekly code commits made by developers. Every week, commit data is collected and stored in an Excel file, allowing teams to understand individual contribution levels, identify top performers, and highlight areas where improvement may be required.</p>

<h3>What problem does this application solve?</h3>
<p>The application provides structured, clear, and insightful information about code commits. It helps teams monitor performance, identify trends, and support continuous improvement through data-driven insights.</p>

<h3>Who should use this application?</h3>
<p>This application can be used by anyone who needs visibility into code commit activity, including developers, managers, and team leads.</p>

<h3>What type of data does the application analyze?</h3>
<p>The application analyzes commit data stored in Excel files.</p>

<h3>How often is the data updated?</h3>
<p>Data is updated on a weekly basis.</p>

<h3>Where does the application get its data from?</h3>
<p>Weekly Excel files are stored and retrieved from SharePoint.</p>

<h3>Is this application automated or manual?</h3>
<p>Uploading the Excel file is a manual process. Once the file is uploaded, all data processing, automation, and dashboard updates are handled automatically.</p>

<hr>

<h2>2. Data Source & Upload Rules</h2>

<h3>From where does the application retrieve the Excel file?</h3>
<p>The application retrieves Excel files from SharePoint.</p>

<h3>Which Teams channel SharePoint location is used?</h3>
<p>The data is stored in the current Teams channel named <strong>“testing excel”</strong>. Navigate to <strong>Files tab → DataFolder</strong>, where all weekly files are stored.</p>

<h3>How many Excel files can be uploaded per week?</h3>
<p>Only one Excel file per week is allowed.</p>

<h3>What happens if I upload more than one Excel file in a week?</h3>
<p>The application will generate an error and will not accept additional files.</p>

<h3>What kind of error will occur if I upload multiple files?</h3>
<p>An error message will appear stating that only one file can be uploaded per week, as this limit is enforced by the application.</p>

<h3>What format should the Excel file be in?</h3>
<p>The data in the Excel file must be formatted as a table.</p>

<h3>Does the Excel file need a specific naming convention?</h3>
<p>No manual naming is required. Once uploaded, the file name is automatically updated to reflect the current week’s start date.</p>

<h3>What columns are mandatory in the Excel file?</h3>
<ul>
    <li>Name</li>
    <li>Commits (Last Week)</li>
    <li>Commits (This Week)</li>
    <li>Commits (Last Month)</li>
    <li>Commits (This Month)</li>
    <li>Commits (12 Weeks)</li>
    <li>Manager Email</li>
    <li>NTID</li>
    <li>Start Date</li>
    <li>End Date</li>
</ul>

<hr>

<h2>3. Power Automate & Automation Logic</h2>

<h3>Does the application use Power Automate?</h3>
<p>Yes, the application uses multiple Power Automate flows.</p>

<h3>What tasks are automated using Power Automate flows?</h3>
<ul>
    <li>Uploading Excel files to SharePoint</li>
    <li>Generating reports</li>
    <li>Updating SharePoint lists</li>
    <li>Retrieving data from SharePoint lists</li>
</ul>

<h3>When do the Power Automate flows get triggered?</h3>
<ul>
    <li>The Upload button is clicked</li>
    <li>The Generate Report option is selected</li>
    <li>A date is selected from the dropdown and the Get button is clicked</li>
</ul>

<h3>What happens after a new Excel file is uploaded?</h3>
<p>A new Excel file is created with the current week’s name. The uploaded file is then processed and formatted automatically according to application requirements.</p>

<h3>How long does it take for data to appear in the dashboards after upload?</h3>
<p>It may take approximately 5–6 minutes for the data to appear in the dashboards.</p>

<h3>What should I do if automation does not run as expected?</h3>
<p>Wait for some time and try again. If the issue persists, contact the application administrator for support.</p>

<hr>

<h2>4. Dashboard 1 – Summary Insights</h2>

<h3>What information is shown in Dashboard 1?</h3>
<ul>
    <li>Top 10 highest commit contributors</li>
    <li>Top 10 lowest commit contributors</li>
    <li>Users with zero commits or commits below the required threshold</li>
</ul>

<h3>What does “Top 10 highest commits” mean?</h3>
<p>It represents users who have made the highest number of commits.</p>

<h3>What does “Top 10 lowest commits” mean?</h3>
<p>It represents users whose commits fall below the defined threshold.</p>

<h3>What does “Zero commits” indicate?</h3>
<p>It indicates users who have not made any commits.</p>

<h3>How are commits classified as high or low?</h3>
<p>Commits are classified as low if:</p>
<ul>
    <li>Weekly commits are less than 3</li>
    <li>Monthly commits are less than 12</li>
    <li>Commits over 12 weeks are less than 36</li>
</ul>

<h3>Why do some users not appear in Dashboard 1?</h3>
<p>Only users with the highest commits or those below the threshold are shown. A user may also be missing if they are not present in the weekly data source provided by the admin.</p>

<h3>Can I exclude specific users from Dashboard 1?</h3>
<p>Yes. You can exclude users by clicking the <strong>Skip List</strong> option and providing the user’s name along with the reason.</p>

<h3>How are exception users handled?</h3>
<p>Exception users are stored separately and can be viewed by clicking the <strong>Excluded Users</strong> button.</p>

<h3>Where can I configure exception users?</h3>
<p>Exception users can be configured using the <strong>Skip List</strong> button.</p>

<hr>

<h2>5. Reporting & Downloads</h2>

<h3>Can I download the commit data as an Excel report?</h3>
<p>Yes, commit data can be downloaded as an Excel report.</p>

<h3>Where is the download report option available?</h3>
<p>Select a specific week, click <strong>Details</strong>, and then use the <strong>Download</strong> option.</p>

<h3>What data is included in the downloaded Excel file?</h3>
<ul>
    <li>Sheet 1: Dashboard 1 data</li>
    <li>Sheet 2: Dashboard 2 data</li>
</ul>

<h3>Does the downloaded report reflect current dashboard data?</h3>
<p>Yes, the downloaded report reflects the data for the selected week.</p>

<h3>Can I share the downloaded report with others?</h3>
<p>Please check with your manager or people lead before sharing the report.</p>

<hr>

<h2>6. Errors, Issues & Troubleshooting</h2>

<h3>What should I do if the dashboard is not loading?</h3>
<p>Reload the browser tab. If the issue persists, contact the administrator.</p>

<h3>What should I do if data is not updated?</h3>
<p>Reload the application.</p>

<h3>Will reloading the application fix common issues?</h3>
<p>Yes, reloading often resolves common issues.</p>

<h3>When should I reload the application?</h3>
<p>Reload the application whenever you encounter an error.</p>

<h3>What are common reasons for data not appearing?</h3>
<p>Power Automate flows may still be running in the background. Please wait for a few minutes.</p>

<h3>What should I do if Power Automate fails?</h3>
<p>Contact the administrator.</p>

<h3>What should I do if I see incorrect data?</h3>
<p>Contact the administrator.</p>

<hr>

<h2>7. Usage Rules & Limitations</h2>

<h3>Are there any limitations in the application?</h3>
<p>Yes, Power Automate flows may experience delays at times.</p>

<h3>Can historical data be modified?</h3>
<p>Only application owners can modify historical data.</p>

<h3>Can previous weeks’ Excel files be replaced?</h3>
<p>Yes, owners can modify files by navigating to <strong>Files → DataFolder</strong>. Files are named based on the week.</p>

<h3>Is manual data editing allowed?</h3>
<p>Only owners can manually edit data via the SharePoint files.</p>

<h3>Is the application read-only for users?</h3>
<p>Yes, the application is read-only for non-owners.</p>

<hr>

<h2>8. Security & Access</h2>

<h3>Who has access to the application?</h3>
<p>All users who are part of the Teams channel (owners and members) have access.</p>

<h3>Is the data secure?</h3>
<p>Yes, the data is secured through SharePoint and Teams access controls.</p>

<h3>Who can upload Excel files?</h3>
<p>Only owners can upload Excel files.</p>

<h3>Can everyone see manager email details?</h3>
<p>Yes, manager email details are visible to users.</p>

<h3>Is SharePoint access required to use the app?</h3>
<p>Yes, SharePoint access is required.</p>

<hr>

<p class="support-note">Support Note: If the requested information is not available on this page, please contact the application administrator for further assistance.</p>

</body>
</html>
