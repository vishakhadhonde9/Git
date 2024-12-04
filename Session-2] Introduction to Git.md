# Git -
- Git is a DevOps tool used for source code management.
- Git is a free, open-source distributed version control system.
- Git is used to tracking changes in the source code, enabling multiple developers to work together on non-linear development.
- Linus Torvalds created Git in 2005 for the development of the Linux kernel.

# Difference between Git and GitHub-

| **Aspect**         | **Git**                                       | **GitHub**                                |
|--------------------|-----------------------------------------------|-------------------------------------------|
| **What It Is**     | A version control tool/software               | A cloud-based platform to host Git repositories |
| **Main Purpose**   | Track changes and manage versions of files locally on your computer | Store and share Git repositories online, collaborate with others |
| **Where It Works** | On your local computer                        | On the internet (online platform)         |
| **Internet Required** | No, works offline                           | Yes, requires internet to push/pull changes |
| **Usage**          | Used to save, track, and manage file changes  | Used to store, share, and collaborate on code |
| **Collaboration**  | Can work locally, but no built-in collaboration features | Enables easy collaboration by allowing others to access and contribute to your project |
| **Examples**       | Git commands: `git commit`, `git push`, `git pull` | GitHub website, GitHub repositories, GitHub Issues, Pull Requests |




# Installation of Git -

#### Steps to install git on Red-Hat based Systems:
- Update System.
         sudo yum update -y
- Install git package.
         sudo yum install git -y
- Verify the installation.
         git --version
   
# Configure the git -
## git config -
- Git needs to be configured before you can use it.
- The Git config command is used enter the login and email addresses you want to be associated with your commits.
#### sets up Git with your name-
        git config --global user.name "<Your-Full-Name>“

#### sets up Git with your email-
        git config --global user.email "<your-email-address>"
