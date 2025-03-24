In this project, I set up a web server in the cloud as part of my DevOps hands-on experience. This work lays the foundation for future projects involving file directories in Linux.

🔧 Key Tools Used: One of the critical tools I used was MobaXterm—a versatile IDE that helps manage software and cloud web servers. Although MobaXterm is not an AWS service, it plays an important role in enabling seamless interaction with cloud infrastructure.
Launching the EC2 Instance: To kick off, I launched an EC2 instance, as I needed a virtual machine in the cloud to house my web server and files. Without the EC2 instance, there would be no location to set up the web server.

I enabled SSH@port22, which authenticates users and hosts via SSH. After this, I installed MobaXterm, which allowed me to easily connect to the EC2 instance. With MobaXterm, I could create and edit web server files directly within the instance.
🔍 First Steps with Linux Commands: The first terminal command I ran was:pwd This prints the working directory, helping me verify my current file location.

I proceeded to create users and assign them to groups, ensuring proper access control. To manage these groups, I ran:getent group andrews. getent stands for 'get entries'. This command retrieves details about specific groups, such as andrews, from system databases like /etc/passwd or /etc/group.
📁 Creating Company Directories: Using the mkdir command, I structured the company directories and ensured parent directories were created seamlessly with the -p option:sudo mkdir -p /company_data/finance_budgets. This command allows the creation of the entire directory path, including any missing parent directories. Without the -p flag, the command would fail if /company_data didn't exist.
🔑 Managing File Ownership and Permissions: To assign ownership and permissions, I used:sudo chown: To change the ownership of files and directories and 
sudo chmod: To set access permissions (read, write, execute) for files or directories. These commands ensured the right access levels for the company's data storage.
🌐 Final Steps: I completed the project by creating directories inside the EC2 web server to organize company documents. These directories were set up to store company data while applying proper access permissions to ensure security and functionality.
