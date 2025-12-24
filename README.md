
<h1>📘 Code Commits Analysis – Knowledge Base</h1>

<hr>

<h2>1. Application Overview</h2>
<ul>
  <li><strong>What is Code Commits Analysis?</strong><br>
    Code Commits Analysis is an application that tracks and analyzes weekly code commits made by developers. Every week, commit data is collected and stored in an Excel file, allowing teams to understand individual contribution levels, identify top performers, and highlight areas where improvement may be required.
  </li>
  <li><strong>What problem does this application solve?</strong><br>
    It provides structured, clear, and insightful information about code commits. It helps teams monitor performance, identify trends, and support continuous improvement through data-driven insights.
  </li>
  <li><strong>Who should use this application?</strong><br>
    Developers, managers, and team leads who need visibility into commit activity.
  </li>
  <li><strong>What type of data does the application analyze?</strong><br>
    Commit data stored in Excel files.
  </li>
  <li><strong>How often is the data updated?</strong><br>
    Weekly.
  </li>
  <li><strong>Where does the application get its data from?</strong><br>
    Weekly Excel files stored in SharePoint.
  </li>
  <li><strong>Is this application automated or manual?</strong><br>
    Uploading the Excel file is manual. Once uploaded, all processing and dashboard updates are automated.
  </li>
</ul>

<hr>

<h2>2. Data Source & Upload Rules</h2>
<ul>
  <li><strong>Where does the application retrieve the Excel file?</strong><br>
    From SharePoint.
  </li>
  <li><strong>Where are Excel files stored?</strong><br>
    Navigate to <code>Teams → Files tab → DataFolder</code> in the channel named <strong>“testing excel”</strong>.
  </li>
  <li><strong>How many Excel files can I upload per week?</strong><br>
    <span style="color:green;font-weight:bold;">Only one Excel file per week is allowed.</span>
  </li>
  <li><strong>What happens if I upload more than one Excel file?</strong><br>
    The application will generate an error: <em>“Only one file can be uploaded per week.”</em>
  </li>
  <li><strong>What format should the Excel file be in?</strong><br>
    The data must be formatted as a <strong>table</strong>.
  </li>
  <li><strong>Does the Excel file need a specific naming convention?</strong><br>
    No manual naming is required; the system renames it automatically.
  </li>
  <li><strong>Mandatory columns in the Excel file:</strong>
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
  </li>
</ul>

<hr>

<h2>3. Power Automate & Automation Logic</h2>
<ul>
  <li><strong>Does the application use Power Automate?</strong><br>
    Yes, for uploading files, generating reports, updating SharePoint lists, and retrieving data.
  </li>
  <li><strong>When do flows trigger?</strong><br>
    On <em>Upload</em>, <em>Generate Report</em>, or <em>Get Data</em> actions.
  </li>
  <li><strong>How long for dashboards to update after upload?</strong><br>
    Approximately 5–6 minutes.
  </li>
</ul>

<hr>

<h2>4. Dashboard 1 – Summary Insights</h2>
<ul>
  <li><strong>What does Dashboard 1 show?</strong><br>
    <ul>
      <li>Top 10 highest commit contributors</li>
      <li>Top 10 lowest commit contributors</li>
      <li>Users with zero commits</li>
    </ul>
  </li>
  <li><strong>Low commits criteria:</strong><br>
    Weekly &lt; 3, Monthly &lt; 12, 12 Weeks &lt; 36.
  </li>
</ul>

<hr>

<h2>6. Reporting & Downloads</h2>
<ul>
  <li><strong>Can I download commit data?</strong><br>
    Yes, as an Excel report with Dashboard 1 and Dashboard 2 data.
  </li>
  <li><strong>Where is the download option?</strong><br>
    Select a week → Click <em>Details</em> → Click <em>Download</em>.
  </li>
</ul>

<hr>

<h2>7. Errors & Troubleshooting</h2>
<ul>
  <li><strong>Dashboard not loading?</strong><br>
    Reload the browser. If issue persists, contact admin.
  </li>
  <li><strong>Data not updated?</strong><br>
    Reload the app and wait for flows to finish.
  </li>
</ul>

<hr>

<h2>8. Usage Rules & Limitations</h2>
<ul>
  <li>Historical data can only be modified by owners.</li>
  <li>The app is read-only for non-owners.</li>
</ul>

<hr>

<h2>9. Security & Access</h2>
<ul>
  <li><strong>Who can upload files?</strong><br>
    Only owners.
  </li>
  <li><strong>Is SharePoint access required?</strong><br>
    Yes.
  </li>
</ul>

<hr>

<h3>📌 Support Note</h3>
<p>If the requested information is not available in this knowledge base, please contact the application administrator for further assistance.</p>
