PPT - Production Project Tracker

Overview:
	Tracks Production Project tasks.  Keeps track of tasks performed on a project, employees who worked on that project and session information about the task.

Primary Functions:
	1. Edit / View Project Information:
		- Shows Current Production Projects Only by default.  click filter button to Off to see all past projects as well.
		- Select Project with drop down menu for titles, or via navigation buttons at bottom of form.
		- Shows total of Hours spent from all tasks and sessions for selected project.
		- Enter Tasks and date info for the selected project.
		- Select a task and click the 'Session Details' button for details about the task or to enter session info.
		- Click the 'Freelance Summary' button for a summation of freelance work for the selected title.
		- Click 'Print' button on Freelance form to print out the summation.
		- Click 'Project Report' button to preview a detailed report for the selected project.
		
	2. View Employee Time Cards:
		- Must select a date range to enter the form.
		- Once chosen the form reflects information for the selected date range.
		- Browse employees for the selected date range with the drop down Employees box, or via the navigation bars at botom of form.
		- Print the information for a selected employee by clicking the 'Print' button.

	3. View / Print Reports:
		- Preview a variety of reports:
			- Complete info on Current Production Projects.
			- Complete info on Current Production Projects by Date Range.
			- Task Hour Summary for all Production Projects.
			- Task Hour Summary for Current Production Projects.
			- Project Hour Summary for all Production Projects.
			- Project Hour Summary for Current Production Projects.
			- Summary of all employee activity for Current Production Projects
			- Summary of all employee activity for Current Production Project by Date Range.
			- List of all Current Production Projects.
		- Print the report to your default printer or use 'Print Setup..' to select printer.

	4. Edit the Employee List:
		- Add new employees to the list.
		- Delete any employee from the list.
		- Edit any employee's info.
		
	5. Edit the Task Codes List:
		- Add new Task Codes to the list.
		- Delete any Task Code from the list.
		
	6. View the documentation:
		- ReadMe: this file.
		- Release Notes: info on release version.
		- Maintenance: tech info for db maintenance.
		- About...: designer notes and info.

Basic Structure:

	CDSData[tblTitles] linked and queried for 'forthcoming' flag set to 'yes'.

	1	to	Many
	Title		Tasks
	Task		Sessions
	Employee	Sessions, Tasks
	Task Code	Sessions, Tasks

Interface:
	- Main Menu drives the program.  Hides when inactive.
	- Titles form (Production Projects) shows primary info.  Linked forms show details and reports.
	- Time Cards form is read-only for the specified date range.
	- Reports Menu provides selection area for viewing / printing reports.
	- Employee and Task Code forms allow editing of look-up tables.
	- Help Menu provides hyperlinks to documentation.
	- Exit button closes the whole application.

	