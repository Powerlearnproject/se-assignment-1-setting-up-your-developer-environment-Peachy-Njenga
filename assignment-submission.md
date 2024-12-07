# Developer Environment Setup

## Tasks

### Select Your Operating System (OS)
- **Operating System**: Arch Linux with Hyprland Desktop Environment

### Install a Text Editor or Integrated Development Environment (IDE)
- **Selected IDE**: Visual Studio Code
- **Installation Steps**:
  1. Download Visual Studio Code from [Visual Studio Code](https://code.visualstudio.com/Download).
  2. Open a terminal and run the following commands:
     ```bash
     sudo pacman -S code
     ```
  3. Launch Visual Studio Code from the application menu or by running `code` in the terminal.

### Set Up Version Control System
- **Version Control System**: Git
- **Steps**:
  1. Install Git:
     ```bash
     sudo pacman -S git
     ```
  2. Configure Git with your information:
     ```bash
     git config --global user.name "Your Name"
     git config --global user.email "youremail@example.com"
     ```
  3. Create a GitHub account at [GitHub](https://github.com).
  4. Initialize a Git repository for your project:
     ```bash
     mkdir my_project
     cd my_project
     git init
     touch README.md
     git add README.md
     git commit -m "Initial commit"
     git remote add origin https://github.com/yourusername/my_project.git
     git push -u origin master
     ```

### Install Necessary Programming Languages and Runtimes
- **Programming Language**: Python
- **Installation Steps**:
  1. Download and install Python from [Python.org](https://www.python.org).
  2. Verify installation:
     ```bash
     python --version
     ```
  3. Install pip (Python package manager):
     ```bash
     sudo pacman -S python-pip
     ```

### Configure a Database (MySQL)
- **Database**: MySQL
- **Installation Steps**:
  1. Download MySQL installer from [MySQL](https://dev.mysql.com/downloads/windows/installer/5.7.html).
  2. Follow the installation wizard to install MySQL.
  3. Start MySQL service:
     ```bash
     sudo systemctl start mysqld
     sudo systemctl enable mysqld
     ```
  4. Secure MySQL installation:
     ```bash
     sudo mysql_secure_installation
     ```

### Set Up Development Environments and Virtualization (Optional)
- **Virtualization Tool**: Docker
- **Installation Steps**:
  1. Install Docker:
     ```bash
     sudo pacman -S docker
     ```
  2. Start and enable Docker service:
     ```bash
     sudo systemctl start docker
     sudo systemctl enable docker
     ```
  3. Add your user to the Docker group:
     ```bash
     sudo usermod -aG docker $USER
     ```

### Explore Extensions and Plugins
- **Visual Studio Code Extensions**:
  1. Python Extension for Visual Studio Code.
  2. GitLens — Git supercharged.
  3. Docker Extension.
  4. Prettier — Code formatter.
  5. ESLint.


## Reflection
### Challenges Faced
1. **Configuring Hyprland**:
   - **Challenge**: Understanding the configuration options for Hyprland.
   - **Solution**: Referenced the [Hyprland Wiki](https://wiki.hyprland.org) and community forums for guidance.

2. **Installing MySQL**:
   - **Challenge**: Ensuring compatibility with Arch Linux.
   - **Solution**: Followed Arch Linux-specific instructions and used the AUR package for installation.

3. **Setting Up Docker**:
   - **Challenge**: Configuring Docker permissions.
   - **Solution**: Added user to the Docker group and ensured Docker service was properly enabled.

### Strategies Employed
- **Research**: Utilized online documentation, forums, and tutorials to resolve issues.
- **Community Support**: Engaged with developer communities for tips and troubleshooting help.
- **Incremental Setup**: Installed and configured tools in stages to isolate and address issues effectively.

## Submission
- **GitHub Repository Link**: [GitHub Repository](https://github.com/Peachy-Njenga/Meowtallica)

