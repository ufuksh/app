# Jenkins and Ansible Project

This project demonstrates the integration of Jenkins and Ansible for continuous integration and deployment.

## Project Structure

```
jenkins-ansible-project
├── jenkins
│   └── Jenkinsfile
├── ansible
│   ├── playbook.yml
│   ├── inventory.ini
│   └── roles
│       └── common
│           ├── tasks
│           │   └── main.yml
│           └── templates
│               └── config.j2
└── README.md
```

## Prerequisites

- Jenkins installed and configured
- Ansible installed on the Jenkins server
- Access to target machines for deployment

## Setup Instructions

1. **Clone the repository**:
   ```
   git clone <repository-url>
   cd jenkins-ansible-project
   ```

2. **Configure Ansible Inventory**:
   Edit the `ansible/inventory.ini` file to add your target hosts.

3. **Define Ansible Playbook**:
   Modify the `ansible/playbook.yml` file to include the necessary tasks and roles.

4. **Jenkins Pipeline**:
   The `jenkins/Jenkinsfile` defines the CI/CD pipeline. Configure your Jenkins job to use this file.

## Usage Guidelines

- Trigger the Jenkins job to start the pipeline.
- Monitor the build process in Jenkins.
- Ensure that Ansible can connect to the target hosts as specified in the inventory.

## License

This project is licensed under the MIT License.