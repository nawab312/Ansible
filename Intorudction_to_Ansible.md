**Ansible** is an open-source configuration management, automation, and orchestration tool developed by Red Hat. 
It allows IT administrators to automate repetitive tasks such as software deployment, infrastructure provisioning, and configuration management across multiple servers. Key Features of Ansible:
- *Agentless*: No need to install any agent on managed nodes; uses SSH for communication.
- *Simple & YAML-based*: Uses human-readable YAML syntax for writing playbooks.
- *Declarative & Idempotent*: Ensures that tasks execute only if changes are needed, avoiding unnecessary operations.

![image](https://github.com/user-attachments/assets/fbca164a-6a9c-49f7-9914-4b8ffe30580a)

### Ansible Architecture ###
Ansible follows a **simple client-server** architecture, but with a **masterless** approach. The control node (Ansible server) connects to managed nodes (target machines) over SSH without requiring any agents. Components of Ansible:
- **Control Node:**
  - The machine where Ansible is installed.
  - Executes playbooks and sends commands to managed nodes via SSH or WinRM.
- **Managed Nodes:**
  - The target machines where configurations are applied.
  - No need for any agent installation; just requires SSH access.
- **Inventory:**
  - A file (`hosts` file) that lists all managed nodes.
  - Can be static (`ini`, `yaml`, `json`) or dynamic (cloud-based).
- **Modules:**
  - Predefined scripts that execute tasks (e.g., `yum`, `apt`, `service`, `copy`).
- **Playbooks:**
  - YAML files that define a set of automation tasks.
- **Tasks:**
  - Individual units of work in a playbook (e.g., installing a package, restarting a service).
- **Handlers:**
  - Triggered only when notified by a task (e.g., restart service after config change).
- **Roles:**
  - A structured way to organize playbooks, tasks, variables, and handlers for reusability.
 
![image](https://github.com/user-attachments/assets/9c8796d6-e3f2-4838-95b6-b42c96c66b5a)

