The following describes the flow of the Canvas Power App created to fit the requirements of 
Project 1, Time off Management App, using the accompanied folder of screenshots.

Screenshot 1: Home Screen
This is the home screen the app opens up to. You can choose to register(Sign Up) or login(Sign In).

Screenshot 2: Sign Up
This is the register screen. Error messages are loaded for the purposes of validating fields.
The submit button will not work if any error messages are visible, displaying a popup warning.

Screenshot 2a: Sign Up (Fields filled)
This demonstrates the validation of fields is working.

Screenshot 3: Profile From Sign Up
Once registration is completed, the app will navigate to the profile of the recently made account.
The profile picture is blank by default and can be set using the "Take Picture" button via webcam
or uploaded using the "Upload" button. Any changes to the profile picture will be saved on clicking
the "Confirm Picture" button.

Screenshot 3a: Profile From Sign Up (Pic From Cam)
This demonstrates the "Take Picture" functionality. 

Screenshot 4: SharePoint Table
This demonstrates that the registered account has successfully been added to the SharePoint table.

Screenshot 5: Make Request
This screen is navigated to from the profile screen using the "Request Time Off" button.
An email will be sent using Power Automate upon submission.

Screenshot 6: Power Automate Flow
This is the flow on Power Automate. When a new request is created on the SharePoint table, an email
will be sent to the supervisor's email(can be seen on 6d) with the option to approve or reject the
request.

Screenshot 6a: Power Automate Flow
After the email has been responded to, the condition will identify whether the request has been
approved or rejected. If it has been approved, the associated record in the SharePoint requests 
table will have the approved field set to Yes. Otherwise, it will be set to false and an email
will be sent to the requester's email informing them of the rejection.

Screenshot 6b: Power Automate Flow
If approved, the time requested will be deducted from the requester's total time off balance in
the SharePoint table of employees.

Screenshot 6c: Power Automate Flow
An email will be sent to the requester informing them of the approval.

Screenshot 6d: Power Automate Flow (Email Received)
This is the email that is sent to the supervisor's email.

Screenshot 7: Sign In
This is the log in screen. An error message will show if the details are not found in the 
SharePoint table.

Screenshot 8: Employee List
This is the employee gallery that an admin will see upon log in. They can navigate to their own
profile from here, an employee's profile, or to the request gallery.

Screenshot 9: Requests List
This is the request gallery that shows the status of requests from the associated SharePoint table.
Initially, functionality to change the requests from here was implemented, but the addition of the
Power Automate flow made for potential bugs and so the function was scrapped.