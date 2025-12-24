# Code Commits Analysis – Knowledge Base

---

## 1. Application Overview

### What is Code Commits Analysis?
Code Commits Analysis is an application that tracks and analyzes weekly code commits made by developers. Every week, commit data is collected and stored in an Excel file, allowing teams to understand individual contribution levels, identify top performers, and highlight areas where improvement may be required.

### What problem does this application solve?
The application provides structured, clear, and insightful information about code commits. It helps teams monitor performance, identify trends, and support continuous improvement through data-driven insights.

### Who should use this application?
This application can be used by anyone who needs visibility into code commit activity, including developers, managers, and team leads.

### What type of data does the application analyze?
The application analyzes commit data stored in Excel files.

### How often is the data updated?
Data is updated on a weekly basis.

### Where does the application get its data from?
Weekly Excel files are stored and retrieved from SharePoint.

### Is this application automated or manual?
Uploading the Excel file is a manual process. Once the file is uploaded, all data processing, automation, and dashboard updates are handled automatically.

---

## 2. Data Source & Upload Rules

### From where does the application retrieve the Excel file?
The application retrieves Excel files from SharePoint.

### Which Teams channel SharePoint location is used?
The data is stored in the current Teams channel named **“testing excel”**.  
Navigate to **Files tab → DataFolder**, where all weekly files are stored.

### How many Excel files can be uploaded per week?
Only one Excel file per week is allowed.

### What happens if I upload more than one Excel file in a week?
The application will generate an error and will not accept additional files.

### What kind of error will occur if I upload multiple files?
An error message will appear stating that only one file can be uploaded per week, as this limit is enforced by the application.

### What format should the Excel file be in?
The data in the Excel file must be formatted as a **table**.

### Does the Excel file need a specific naming convention?
No manual naming is required. Once uploaded, the file name is automatically updated to reflect the current week’s start date.

### What columns are mandatory in the Excel file?
- Name  
- Commits (Last Week)  
- Commits (This Week)  
- Commits (Last Month)  
- Commits (This Month)  
- Commits (12 Weeks)  
- Manager Email  
- NTID  
- Start Date  
- End Date  

---

## 3. Power Automate & Automation Logic

### Does the application use Power Automate?
Yes, the application uses multiple Power Automate flows.

### What tasks are automated using Power Automate flows?
- Uploading Excel files to SharePoint  
- Generating reports  
- Updating SharePoint lists  
- Retrieving data from SharePoint lists  

### When do the Power Automate flows get triggered?
Flows are triggered when:  
- The Upload button is clicked  
- The Generate Report option is selected  
- A date is selected from the dropdown and the Get button is clicked  

### What happens after a new Excel file is uploaded?
A new Excel file is created with the current week’s name. The uploaded file is then processed and formatted automatically according to application requirements.

### How long does it take for data to appear in the dashboards after upload?
It may take approximately 5–6 minutes for the data to appear in the dashboards.

### What should I do if automation does not run as expected?
Wait for some time and try again. If the issue persists, contact the application administrator for support.

---

## 4. Dashboard 1 – Summary Insights

### What information is shown in Dashboard 1?
Dashboard 1 displays:  
- Top 10 highest commit contributors  
- Top 10 lowest commit contributors  
- Users with zero commits or commits below the required threshold  

### What does “Top 10 highest commits” mean?
It represents users who have made the highest number of commits.

### What does “Top 10 lowest commits” mean?
It represents users whose commits fall below the defined threshold.

### What does “Zero commits” indicate?
It indicates users who have not made any commits.

### How are commits classified as high or low?
Commits are classified as low if:  
- Weekly commits are less than 3  
- Monthly commits are less than 12  
- Commits over 12 weeks are less than 36  

### Why do some users not appear in Dashboard 1?
Only users with the highest commits or those below the threshold are shown. A user may also be missing if they are not present in the weekly data source provided by the admin.

### Can I exclude specific users from Dashboard 1?
Yes. You can exclude users by clicking the **Skip List** option and providing the user’s name along with the reason.

### How are exception users handled?
Exception users are stored separately and can be viewed by clicking the **Excluded Users** button.

### Where can I configure exception users?
Exception users can be configured using the **Skip List** button.

---

## 5. Reporting & Downloads

### Can I download the commit data as an Excel report?
Yes, commit data can be downloaded as an Excel report.

### Where is the download report option available?
Select a specific week, click **Details**, and then use the **Download** option.

### What data is included in the downloaded Excel file?
- **Sheet 1:** Dashboard 1 data  
- **Sheet 2:** Dashboard 2 data  

### Does the downloaded report reflect current dashboard data?
Yes, the downloaded report reflects the data for the selected week.

### Can I share the downloaded report with others?
Please check with your manager or people lead before sharing the report.

---

## 6. Errors, Issues & Troubleshooting

### What should I do if the dashboard is not loading?
Reload the browser tab. If the issue persists, contact the administrator.

### What should I do if data is not updated?
Reload the application.

### Will reloading the application fix common issues?
Yes, reloading often resolves common issues.

### When should I reload the application?
Reload the application whenever you encounter an error.

### What are common reasons for data not appearing?
Power Automate flows may still be running in the background. Please wait for a few minutes.

### What should I do if Power Automate fails?
Contact the administrator.

### What should I do if I see incorrect data?
Contact the administrator.

---

## 7. Usage Rules & Limitations

### Are there any limitations in the application?
Yes, Power Automate flows may experience delays at times.

### Can historical data be modified?
Only application owners can modify historical data.

### Can previous weeks’ Excel files be replaced?
Yes, owners can modify files by navigating to **Files → DataFolder**. Files are named based on the week.

### Is manual data editing allowed?
Only owners can manually edit data via the SharePoint files.

### Is the application read-only for users?
Yes, the application is read-only for non-owners.

---

## 8. Security & Access

### Who has access to the application?
All users who are part of the Teams channel (owners and members) have access.

### Is the data secure?
Yes, the data is secured through SharePoint and Teams access controls.

### Who can upload Excel files?
Only owners can upload Excel files.

### Can everyone see manager email details?
Yes, manager email details are visible to users.

### Is SharePoint access required to use the app?
Yes, SharePoint access is required.

---

## Support Note (Important for Chatbot)
If the requested information is not available in this knowledge base, please contact the application administrator for further assistance.
