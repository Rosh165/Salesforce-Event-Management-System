# Salesforce Event Management System

A Salesforce CRM project for organizing event-related information using custom objects, relationships, and validation rules.

## About the Project

The Salesforce Event Management System demonstrates how Salesforce can be customized to manage event data, connect related records, and maintain data quality through validation rules.

This project uses Salesforce Developer Edition, Salesforce DX, Salesforce CLI, and GitHub for source control.

## Features

- **Custom Objects:** Organize event-related information.
- **Object Relationships:** Connect related Salesforce records.
- **Validation Rules:** Prevent invalid data based on defined business rules.
- **Salesforce DX:** Maintain metadata in a structured project format.
- **Version Control:** Track changes using Git and GitHub.

## Technologies Used

- Salesforce Developer Edition
- Salesforce Lightning Experience
- Salesforce DX and Salesforce CLI
- Git and GitHub
- Visual Studio Code (recommended)

## Project Structure

```text
Salesforce-Event-Management-System/
├── config/
├── force-app/
│   └── main/
│       └── default/
│           ├── applications/
│           ├── classes/
│           ├── layouts/
│           ├── lwc/
│           ├── objects/
│           ├── permissionsets/
│           ├── tabs/
│           └── triggers/
├── scripts/
├── .gitignore
├── package.json
├── README.md
└── sfdx-project.json
```

## Prerequisites

Install the following tools before running the project:

1. Salesforce CLI
2. Git
3. A Salesforce Developer Edition org
4. Visual Studio Code with the Salesforce Extension Pack (recommended)

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/Rosh165/Salesforce-Event-Management-System.git
cd Salesforce-Event-Management-System
```

### 2. Log in to Salesforce

For a Developer Edition org, run:

```bash
sf org login web --alias TechFestOrg --instance-url https://login.salesforce.com
```

Follow the browser prompts to authenticate.

### 3. Verify your connection

```bash
sf org list
```

### 4. Deploy Salesforce metadata

After checking the target org and project configuration, run:

```bash
sf project deploy start --target-org TechFestOrg --source-dir force-app
```

Review the command output to confirm whether deployment succeeded.

### 5. Open the Salesforce org

```bash
sf org open --target-org TechFestOrg
```

## Testing Checklist

- [ ] Verify that custom objects are deployed.
- [ ] Check fields and object relationships.
- [ ] Test validation rules with valid and invalid data.
- [ ] Verify record creation and updates.
- [ ] Confirm that users have appropriate permissions.

## Future Enhancements

- Event registration and attendee tracking
- Email notifications and reminders
- Calendar integration
- Reports and dashboards
- Improved user interface using Lightning Web Components

*These are proposed enhancements and may not be implemented in the current version.*

## Repository

[View this project on GitHub](https://github.com/Rosh165/Salesforce-Event-Management-System)

## Author

**Roshan S.**  
Department of Artificial Intelligence and Data Science  
St. Joseph College of Engineering

## License

No license has been specified yet. Add a license if you intend to permit public reuse or modification of this project.
