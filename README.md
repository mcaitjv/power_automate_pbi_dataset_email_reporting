# Power Automate Email Reporting
Project Overview

This Power Automate flow automatically fetches data from a Power BI Dataset, formats it into a clean HTML table with aligned numeric values, and sends the table as the body of an email. This is used primarily for distributing formatted reports to designated recipients on a scheduled basis.
Features

    Automated Data Retrieval: Fetches the latest sales data from a configured Power BI dataset.
    Data Formatting: Applies number formatting to ensure sales figures are readable (e.g., adding thousands separators and limiting to two decimal places).
    Automated Email Dispatch: Sends out an email with the formatted data in an HTML table where the sales figures are right-aligned.

Flow Components

    Recurrence: Triggers the flow based on the configured schedule.
    Data Fetch: Executes a query against a Power BI dataset to retrieve current sales data.
    Data Processing:
        Formats data using expressions.
        Constructs an HTML table with style specifications for proper display of data.
    Email Dispatch: Composes and sends the email to a predefined list of recipients with the HTML table embedded in the email body.

Prerequisites

    Access to Microsoft Power Automate.
    A Power BI dataset setup with sales data available.
    Permissions to send emails using Outlook or another email client setup within Power Automate.

Setup and Configuration

    Clone the Repository: Download the project files to your local machine or your preferred environment where Power Automate flows are managed.
    Configure Data Source:
        Modify the data fetching step to point to your specific Power BI dataset.
    Set up Recurrence:
        Adjust the recurrence scheduling based on your reporting needs (daily, weekly, etc.).
    Email Configuration:
        Set up the 'Send an Email' action with appropriate recipient emails, subject line, and body configurations.

Usage

Once set up, the flow will run at the scheduled intervals:

    It will retrieve the latest data from the Power BI dataset.
    Format the data and construct an HTML formatted email.
    Send the email to all configured recipients automatically.

Customizations

    Modify the HTML structure or styles in the email formatting step as needed.
    Adjust the numeric formatting in the data processing step to match different regional standards or preferences.

