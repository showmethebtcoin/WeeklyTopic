# WeeklyTopic

## Description

The **WeeklyTopic** automation reads a Google Sheet that contains the names and email addresses of each student, along with a column where the topic for the next class is updated every week. The tutor only needs to update this column, and once a week, the automation reads the spreadsheet and sends an email to each student (in HTML format generated by GPT), informing them of the upcoming class topic.

## Features

- Automates the writing and sending of weekly emails to each student.
- Integration with Google Sheets to manage student information and class topics.
- Emails are personalized and formatted in HTML, generated by a custom GPT model.
- Reduces the time a private online language tutor spends drafting and sending emails by simply updating the topic in the Google Sheet.

## Installation

1. **Access to Make**:
   - In order to replicate or use this automation, you will need to have an account in Make.

2. **Import the flow**:
   - In Make, when creating a new scenario, you'll find a section called **Controls** with three dots ("..."). By clicking on it, you'll have the option to **import a JSON file**. You can use this option to import the flow from [WeeklyTopic.json](./flow/WeeklyTopic.json).

3. **Set up credentials**:
   - Since the API connections are personal, they cannot be shared for security reasons. You will need to set up your own credentials for:
     - **Google Sheets**: To access and read the student names, emails, and weekly topics.
     - **Gmail**: To send personalized emails to each student with the topic for the upcoming class.

## Usage

- The automation runs every Sunday at noon, reads the Google Sheet, and automatically sends personalized emails to each student.
- The tutor only needs to update the "Class Topic" column in the Google Sheet to ensure the correct information is sent out.
- Emails are generated in HTML format by GPT, and each email is personalized with the student's name and the topic for the next class.

## Flow Screenshots

![WeeklyTopic](https://github.com/user-attachments/assets/d866d137-4cea-45e7-84e2-8225078287a1)


## Technologies Used

- **Make**: For creating the workflow.
- **Google Sheets API**: For managing student data and weekly class topics.
- **Gmail API**: For sending personalized HTML emails to students.

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
