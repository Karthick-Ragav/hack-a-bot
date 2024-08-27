# hack-a-bot

---

# *Support Ticket System for Educational Institutions*

## *Introduction*
This project implements an automated support ticket system tailored for educational institutions using UiPath. The system categorizes tickets based on priority and department, facilitating efficient issue resolution. It includes robust error handling through a global exception handler to ensure reliability and resilience.

## *Features*
- *Ticket Classification*: Automatically categorizes tickets by priority and department using AI Center.
- *Global Exception Handling*: Captures and manages errors across the workflow to ensure smooth operation.
- *Email Notifications*: Sends alerts to the IT support team or administrators upon encountering critical issues.
- *Retry Mechanism*: Attempts to recover from transient errors by retrying failed actions.
- *Customizable Workflow*: Easily adaptable to different educational environments.

## *Architecture*
The system architecture consists of several key components:
- *UiPath Workflows*: Automates the processing of support tickets.
- *AI Center Integration*: Leverages machine learning models to classify tickets.
- *Global Exception Handler*: Manages errors and ensures that the system responds appropriately.
- *Orchestrator*: Schedules, monitors, and manages the automated workflows.

## *Installation*

### *Prerequisites*
- *UiPath Studio*: Version 21 or higher.
- *UiPath Orchestrator*: For deployment and management.
- *AI Center*: For machine learning model deployment and management.
- *Email Server*: Configured for sending notifications.

### *Steps*
1. *Clone the Repository*
   bash
   git clone 
   cd support-ticket-system
   
2. *Open in UiPath Studio*
   - Open the project in UiPath Studio by navigating to the support-ticket-system folder and opening the .xaml files.

3. *Configure the Project*
   - Update the project settings in UiPath Studio to match your environment, including AI Center connections and email server details.

4. *Deploy to Orchestrator*
   - Publish the project to UiPath Orchestrator to schedule and manage the automation.

5. *Run the Workflow*
   - Start the workflow from UiPath Orchestrator or UiPath Assistant and monitor the logs.

## *Usage*
1. *Ticket Submission*:
   - Users submit support tickets through the institution's ticketing platform.
2. *Ticket Processing*:
   - The system classifies tickets based on department and priority using the AI model.
3. *Error Handling*:
   - The global exception handler manages any errors that occur during processing, logs them, and sends notifications as needed.
4. *Ticket Resolution*:
   - Classified tickets are routed to the appropriate department for resolution.

## *Global Exception Handling*
The project includes a comprehensive global exception handler to manage errors during workflow execution. It logs errors, sends email notifications to the support team, and includes a retry mechanism for transient issues. For more details, see the GlobalExceptionHandler.xaml file.

### *Key Components*
- *Logging*: Records error details in the logs.
- *Retry Mechanism*: Automatically retries failed actions to handle transient errors.

