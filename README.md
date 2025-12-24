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
        pre { background-color: #f4f4f4; padding: 10px; border-radius: 5px; }
    </style>
</head>
<body>

<h1>Code Commits Analysis – Knowledge Base</h1>
<hr>

<h2>1. Application Overview</h2>

<h3>Q: What is Code Commits Analysis?</h3>
<p>A: It is an application that tracks and analyzes weekly code commits from developers using Excel data stored in SharePoint.</p>

<h3>Q: What problem does it solve?</h3>
<p>A: It provides structured insights into commit activity, helping teams monitor performance and identify trends.</p>

<h3>Q: Who can use this application?</h3>
<p>A: Developers, managers, and team leads who need visibility into commit activity.</p>

<h3>Q: How often is data updated?</h3>
<p>A: Weekly.</p>

<hr>

<h2>2. Data Source & Upload Rules</h2>

<h3>Q: Where does the application get its data from?</h3>
<p>A: From Excel files stored in SharePoint.</p>

<h3>Q: Where are Excel files stored?</h3>
<p>A: Navigate to Teams → Files tab → DataFolder in the channel named “testing excel”.</p>

<h3>Q: How many Excel files can I upload per week?</h3>
<p>A: Only one Excel file per week is allowed.</p>

<h3>Q: What happens if I upload more than one file?</h3>
<p>A: The application will show an error: “Only one file can be uploaded per week.”</p>

<h3>Q: What format should the Excel file be in?</h3>
<p>A: The data must be formatted as a table.</p>

<h3>Q: Does the file need a specific name?</h3>
<p>A: No manual naming is required; the system renames it automatically.</p>

<h3>Q: Mandatory columns in Excel file?</h3>
<pre>
Name
Commits (Last Week)
Commits (This Week)
Commits (Last Month)
Commits (This Month)
Commits (12 Weeks)
Manager Email
NTID
Start Date
End Date
</pre>

<hr>

<h2>3. Automation & Power Automate</h2>

<h3>Q: Does the app use Power Automate?</h3>
<p>A: Yes, for uploading files, generating reports, updating SharePoint lists, and retrieving data.</p>

<h3>Q: When do flows trigger?</h3>
<p>A: On Upload, Generate Report, or Get Data actions.</p>

<h3>Q: How long for dashboards to update after upload?</h3>
<p>A: About 5–6 minutes.</p>

<hr>

<h2>4. Dashboard Insights</h2>

<h3>Q: What does Dashboard 1 show?</h3>
<ul>
    <li>Top 10 highest commit contributors</li>
    <li>Top 10 lowest commit contributors</li>
    <li>Users with zero commits</li>
</ul>

<h3>Q: How are low commits defined?</h3>
<ul>
    <li>Weekly < 3</li>
    <li>Monthly < 12</li>
    <li>12 Weeks < 36</li>
</ul>

<hr>

<h2>5. Reporting & Downloads</h2>

<h3>Q: Can I download commit data?</h3>
<p>A: Yes, as an Excel report with Dashboard 1 and Dashboard 2 data.</p>

<h3>Q: Where is the download option?</h3>
<p>A: Select a week → Click Details → Click Download.</p>

<hr>

<h2>6. Errors & Troubleshooting</h2>

<h3>Q: Dashboard not loading?</h3>
<p>A: Reload the browser. If issue persists, contact admin.</p>

<h3>Q: Data not updated?</h3>
<p>A: Reload the app and wait for flows to finish.</p>

<hr>

<h2>7. Usage Rules</h2>

<h3>Q: Can historical data be modified?</h3>
<p>A: Only by owners.</p>

<h3>Q: Is the app read-only for users?</h3>
<p>A: Yes, except owners.</p>

<hr>

<h2>8. Security & Access</h2>

<h3>Q: Who can upload files?</h3>
<p>A: Only owners.</p>

<h3>Q: Is SharePoint access required?</h3>
<p>A: Yes.</p>

<hr>

<p class="support-note">Support Note: If the requested information is not available on this page, please contact the application administrator for further assistance.</p>

</body>
</html>
