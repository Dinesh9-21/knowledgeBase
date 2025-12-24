Code Commits Analysis – Knowledge Base
________________________________________
1. Application Overview
What is Code Commits Analysis?
Code Commits Analysis is an application that tracks and analyzes weekly code commits made by developers. Every week, commit data is collected and stored in an Excel file, allowing teams to understand individual contribution levels, identify top performers, and highlight areas where improvement may be required.
________________________________________
What problem does this application solve?
The application provides structured, clear, and insightful information about code commits. It helps teams monitor performance, identify trends, and support continuous improvement through data-driven insights.
________________________________________
Who should use this application?
This application can be used by anyone who needs visibility into code commit activity, including developers, managers, and team leads.
________________________________________
What type of data does the application analyze?
The application analyzes commit data stored in Excel files.
________________________________________
How often is the data updated?
Data is updated on a weekly basis.
________________________________________
Where does the application get its data from?
Weekly Excel files are stored and retrieved from SharePoint.
________________________________________
Is this application automated or manual?
Uploading the Excel file is a manual process. Once the file is uploaded, all data processing, automation, and dashboard updates are handled automatically.
________________________________________
2. Data Source & Upload Rules
From where does the application retrieve the Excel file?
The application retrieves Excel files from SharePoint.
________________________________________
Which Teams channel SharePoint location is used?
The data is stored in the current Teams channel named “testing excel”.
Navigate to the Files tab → DataFolder, where all weekly files are stored.
________________________________________
How many Excel files can be uploaded per week?
Only one Excel file per week is allowed.
________________________________________
What happens if I upload more than one Excel file in a week?
The application will generate an error and will not accept additional files.
________________________________________
What kind of error will occur if I upload multiple files?
An error message will appear stating that only one file can be uploaded per week, as this limit is enforced by the application.
________________________________________
What format should the Excel file be in?
The data in the Excel file must be formatted as a table.
________________________________________
Does the Excel file need a specific naming convention?
No manual naming is required. Once uploaded, the file name is automatically updated to reflect the current week’s start date.
________________________________________
What columns are mandatory in the Excel file?
The following columns are mandatory:
•	Name
•	Commits (Last Week)
•	Commits (This Week)
•	Commits (Last Month)
•	Commits (This Month)
•	Commits (12 Weeks)
•	Manager Email
•	NTID
•	Start Date
•	End Date
________________________________________
3. Power Automate & Automation Logic
Does the application use Power Automate?
Yes, the application uses multiple Power Automate flows.
________________________________________
What tasks are automated using Power Automate flows?
Power Automate is used for:
•	Uploading Excel files to SharePoint
•	Generating reports
•	Updating SharePoint lists
•	Retrieving data from SharePoint lists
________________________________________
When do the Power Automate flows get triggered?
Flows are triggered when:
•	The Upload button is clicked
•	The Generate Report option is selected
•	A date is selected from the dropdown and the Get button is clicked
________________________________________
What happens after a new Excel file is uploaded?
A new Excel file is created with the current week’s name. The uploaded file is then processed and formatted automatically according to application requirements.
________________________________________
How long does it take for data to appear in the dashboards after upload?
It may take approximately 5–6 minutes for the data to appear in the dashboards.
________________________________________
What should I do if automation does not run as expected?
Wait for some time and try again. If the issue persists, contact the application administrator for support.
________________________________________
4. Dashboard 1 – Summary Insights
What information is shown in Dashboard 1?
Dashboard 1 displays:
•	Top 10 highest commit contributors
•	Top 10 lowest commit contributors
•	Users with zero commits or commits below the required threshold
________________________________________
What does “Top 10 highest commits” mean?
It represents users who have made the highest number of commits.
________________________________________
What does “Top 10 lowest commits” mean?
It represents users whose commits fall below the defined threshold.
________________________________________
What does “Zero commits” indicate?
It indicates users who have not made any commits.
________________________________________
How are commits classified as high or low?
Commits are classified as low if:
•	Weekly commits are less than 3
•	Monthly commits are less than 12
•	Commits over 12 weeks are less than 36
________________________________________
Why do some users not appear in Dashboard 1?
Only users with the highest commits or those below the threshold are shown. A user may also be missing if they are not present in the weekly data source provided by the admin.
________________________________________
Can I exclude specific users from Dashboard 1?
Yes. You can exclude users by clicking the Skip List option and providing the user’s name along with the reason.
________________________________________
How are exception users handled?
Exception users are stored separately and can be viewed by clicking the Excluded Users button.
________________________________________
Where can I configure exception users?
Exception users can be configured using the Skip List button.
________________________________________
6. Reporting & Downloads
Can I download the commit data as an Excel report?
Yes, commit data can be downloaded as an Excel report.
________________________________________
Where is the download report option available?
Select a specific week, click Details, and then use the Download option.
________________________________________
What data is included in the downloaded Excel file?
•	Sheet 1: Dashboard 1 data
•	Sheet 2: Dashboard 2 data
________________________________________
Does the downloaded report reflect current dashboard data?
Yes, the downloaded report reflects the data for the selected week.
________________________________________
Can I share the downloaded report with others?
Please check with your manager or people lead before sharing the report.
________________________________________
7. Errors, Issues & Troubleshooting
What should I do if the dashboard is not loading?
Reload the browser tab. If the issue persists, contact the administrator.
________________________________________
What should I do if data is not updated?
Reload the application.
________________________________________
Will reloading the application fix common issues?
Yes, reloading often resolves common issues.
________________________________________
When should I reload the application?
Reload the application whenever you encounter an error.
________________________________________
What are common reasons for data not appearing?
Power Automate flows may still be running in the background. Please wait for a few minutes.
________________________________________
What should I do if Power Automate fails?
Contact the administrator.
________________________________________
What should I do if I see incorrect data?
Contact the administrator.
________________________________________
8. Usage Rules & Limitations
Are there any limitations in the application?
Yes, Power Automate flows may experience delays at times.
________________________________________
Can historical data be modified?
Only application owners can modify historical data.
________________________________________
Can previous weeks’ Excel files be replaced?
Yes, owners can modify files by navigating to Files → DataFolder. Files are named based on the week.
________________________________________
Is manual data editing allowed?
Only owners can manually edit data via the SharePoint files.
________________________________________
Is the application read-only for users?
Yes, the application is read-only for non-owners.
________________________________________
9. Security & Access
Who has access to the application?
All users who are part of the Teams channel (owners and members) have access.
________________________________________
Is the data secure?
Yes, the data is secured through SharePoint and Teams access controls.
________________________________________
Who can upload Excel files?
Only owners can upload Excel files.
________________________________________
Can everyone see manager email details?
Yes, manager email details are visible to users.
________________________________________
Is SharePoint access required to use the app?
Yes, SharePoint access is required.
________________________________________
Support Note (Important for Chatbot)
If the requested information is not available in this knowledge base, please contact the application administrator for further assistance

