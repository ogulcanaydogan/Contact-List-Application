
# Contact List Application

This Contact List Application is a simple web-based tool that allows users to manage their contacts efficiently. With a clean and intuitive interface, users can add, update, delete, and view contacts with ease. The application is built using modern web technologies to provide a responsive and interactive experience.

## Features

- **Add Contacts**: Quickly add new contacts by providing details such as name, phone number, and email address.
- **Edit Contacts**: Update existing contact information easily.
- **Delete Contacts**: Remove contacts from the list when they are no longer needed.
- **View Contacts**: Access the list of all saved contacts with a simple interface.
- **Search Functionality**: Search through your contacts to find specific entries efficiently.

## Technologies Used

- **Front-End**:
  - HTML5
  - CSS3
  - JavaScript (React.js, Vue.js, or vanilla JS) *(Specify based on your implementation)*
  
- **Back-End**:
  - Node.js / Express *(if applicable)*
  - REST API *(if applicable)*

- **Database**:
  - MySQL hosted on AWS RDS

- **Deployment**:
  - AWS EC2 for application hosting
  - Terraform for infrastructure as code (IaC) to automate AWS resource provisioning

## Setup and Installation

### Local Setup

1. Clone the repository:
    \`\`\`bash
    git clone https://github.com/ogulcanaydogan/Contact-List-Application.git
    \`\`\`

2. Navigate into the project directory:
    \`\`\`bash
    cd Contact-List-Application
    \`\`\`

3. Install the required dependencies:
    \`\`\`bash
    npm install
    \`\`\`

4. Start the application:
    \`\`\`bash
    npm start
    \`\`\`

5. Open your browser and navigate to \`http://localhost:3000\` to start using the Contact List Application.

### Running on AWS using Terraform

The application is designed to be deployed on AWS using Terraform to provision the required infrastructure. Here’s an overview of the AWS services used and how Terraform manages them:

- **EC2**: Hosts the Flask web application.
- **RDS**: Manages the MySQL database for storing contact information.
- **Security Groups**: Ensure secure access to EC2 instances and RDS databases.
- **VPC**: Provides network isolation for the application.

#### Steps to Deploy on AWS:

1. **Install Terraform**:
   Ensure Terraform is installed on your local machine. You can follow the official [Terraform installation guide](https://learn.hashicorp.com/tutorials/terraform/install-cli).

2. **AWS Configuration**:
   Set up your AWS credentials by running:
   \`\`\`bash
   aws configure
   \`\`\`

3. **Initialize Terraform**:
   Navigate to the directory containing the Terraform files and initialize Terraform:
   \`\`\`bash
   terraform init
   \`\`\`

4. **Apply Terraform Configuration**:
   Run the following command to provision the AWS infrastructure and deploy the application:
   \`\`\`bash
   terraform apply
   \`\`\`
   Confirm the actions when prompted.

5. **Access the Application**:
   Once Terraform finishes deploying, you can access the application using the public IP or DNS of the provisioned EC2 instance.

## Usage

- **Adding a Contact**: Fill in the form with the contact's details and click the "Add" button.
- **Editing a Contact**: Click the "Edit" button next to the contact you want to update, modify the details, and save the changes.
- **Deleting a Contact**: Click the "Delete" button next to the contact you wish to remove.
- **Searching for a Contact**: Use the search bar to filter contacts by name or other details.

## Contributing

If you want to contribute to the project:

1. Fork the repository.
2. Create a new feature branch (\`git checkout -b feature/new-feature\`).
3. Commit your changes (\`git commit -m 'Add some new feature'\`).
4. Push the branch (\`git push origin feature/new-feature\`).
5. Create a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
