# CMPG-323-Overview-38546817

## Repositories
The following repositories will be created and used for each project:

- Web API Repository: Contains the code for the Web API that stores telemetry data linked to projects and clients.
- Web Application Repository: Contains the code for the web application that handles CRUD (Create, Read, Update, Delete) operations on projects and clients.
- RPA Testing Repository: Contains the RPA bot code used for testing the web application functionality.
- Reporting Repository: Contains the code for the reporting component that visualizes time and cost savings per project and client.
  
## Documentation
All documentation related to the projects can be found here.

## Branching Strategy
Each repository will follow a branching strategy to ensure efficient and organized development:

- Main Branch: The default branch containing the production-ready code.
- Development Branch: Used for integrating features before they are merged into the main branch.
- Feature Branches: Created for each new feature or bug fix. Named using the format feature/feature-name or bugfix/issue-description.
- Release Branches: Created when preparing for a new production release. Named using the format release/version-number.
  
## Workflow
Create a feature branch from the development branch.
Work on the feature and commit changes.
Create a pull request to merge the feature branch into the development branch.
Once the feature is tested and reviewed, merge it into the development branch.
When ready for production, create a release branch from the development branch and test thoroughly.
Merge the release branch into the main branch after successful testing.

## .gitignore File
Each project repository will include a .gitignore file to specify files and directories that should be ignored by Git. This includes:

- Sensitive files: Such as configuration files with credentials.
- Build and dependency directories: Such as node_modules, bin/, obj/.
- System files: Such as .DS_Store, Thumbs.db.
- Logs and temporary files: Such as *.log, *.tmp.

## Storage of Credentials and Sensitive Information
Credentials and sensitive information will not be stored directly in the codebase. Instead:

- Environment Variables: Used to store sensitive information securely. These are set on the deployment server and accessed within the code using environment variable references.
- Configuration Management: Tools such as AWS Secrets Manager, Azure Key Vault, or HashiCorp Vault can be used to manage and access sensitive data securely.
- Encrypted Files: If sensitive information must be stored in a file, the file will be encrypted, and the decryption key will be stored securely.


## Burndown Chart
![image](https://github.com/user-attachments/assets/e6a912c9-2531-4f73-a47b-224eee7fa962)


