# 🚀 My Ansible Learning Journey 📘✨

Welcome to my Ansible learning journey! This repository documents my hands-on exploration of Ansible, from the basics to advanced automation concepts. Each playbook and example here represents a step forward, filled with practical lessons, mistakes, and "aha!" moments. 🌱

---

## 🏁 Getting Started

I began by understanding the **core concepts of Ansible**:  
- Playbooks  
- Inventory files  
- Variables  
- Tasks  
- Loops  
- Conditionals  
- Facts  
- Roles and more!

---

## 📝 What You'll Find in This Repo

- **Playbooks for every concept:**  
  From simple pings to complex variable management and loops.

- **Inventory examples:**  
  See how to define hosts and groups in `inventory.ini` and dynamic inventory with AWS EC2 (`inventory.aws_ec2.yaml`).

- **Variable usage:**  
  Explore different ways to define and override variables (play, task, file, prompt, inventory, command line).

- **Real-world scenarios:**  
  Service installation, package management, and conditional logic based on OS family.

---

## 🗂️ Repository Structure

- `01-playbook.yaml` – My first Ansible playbook (ping a server) 🟢
- `02-helloworld.yaml` – Print "hi world" using Ansible
- `03-nginx.yaml` – Install and start Nginx on the frontend server
- `04-multiplay.yaml` – Multiple plays in a single playbook
- `05-play-vars.yaml` – Play-level variables
- `06-taks-vars.yaml` – Task-level variables
- `07-vars-files.yaml` – Import variables from external files (`course.yaml`)
- `08-vars-prompt.yaml` – Prompt user for variables at runtime
- `09-vars-inventory.yaml` & `10-vars-inventory.yaml` – Variables from inventory
- `11-vars-args.yaml` – Passing variables via command line (`-e`)
- `12-vars-pref.yaml` – Variable precedence demonstration
- `13-data-types.yaml` – Using different data types (strings, lists, dicts, booleans)
- `14-condtion.yaml` & `16-conditon.yaml` – Conditional tasks
- `15-gather-facts.yaml` – Gathering facts and using them in plays
- `17-loops.yaml`, `18-loops.yaml`, `19-loops.yaml` – Looping over lists and dictionaries
- `20-function.yaml` – Using filters and functions
- `21-user.yaml` – User management with conditional logic (check if user exists before creating)
- `23-nginx.yaml` – Nginx installation using dynamic inventory with rolling updates (`serial: 5`)
- `24.ec2-r53.yaml` – AWS EC2 instance creation and Route53 DNS record management
- `course.yaml` – Example variable file
- `inventory.ini` – Example inventory file
- `inventory.aws_ec2.yaml` – Dynamic inventory configuration for AWS EC2 instances

---

## 💡 Key Learnings & Takeaways

- **Variable Precedence:**  
  Explored in [`12-vars-pref.yaml`](12-vars-pref.yaml). Learned how variables from the command line, task, file, prompt, play, and inventory override each other.

- **Prompting for Variables:**  
  Used `vars_prompt` to securely collect sensitive data at runtime ([`08-vars-prompt.yaml`](08-vars-prompt.yaml)).

- **Inventory Variables:**  
  Defined variables directly in `inventory.ini` and used them in playbooks ([`09-vars-inventory.yaml`](09-vars-inventory.yaml), [`10-vars-inventory.yaml`](10-vars-inventory.yaml)).

- **Loops & Conditionals:**  
  Automated repetitive tasks and made plays dynamic with loops and `when` conditions ([`17-loops.yaml`](17-loops.yaml), [`14-condtion.yaml`](14-condtion.yaml)).

- **Facts Gathering:**  
  Used gathered facts to make OS-specific decisions ([`15-gather-facts.yaml`](15-gather-facts.yaml), [`16-conditon.yaml`](16-conditon.yaml)).

- **Functions & Filters:**  
  Leveraged Jinja2 filters for data manipulation ([`20-function.yaml`](20-function.yaml)).

- **User Management:**  
  Implemented conditional user creation with existence checks ([`21-user.yaml`](21-user.yaml)).

- **Dynamic Inventory & Rolling Updates:**  
  Used AWS dynamic inventory and implemented rolling updates for zero-downtime deployments ([`23-nginx.yaml`](23-nginx.yaml)).

- **AWS Integration:**  
  Created EC2 instances and managed Route53 DNS records programmatically ([`24.ec2-r53.yaml`](24.ec2-r53.yaml)).

---

## 🐞 Mistakes & Debugging Moments

- **Variable Precedence Confusion:**  
  Sometimes variables didn't resolve as expected—learned to check the order of precedence!

- **Inventory Formatting:**  
  Missed quotes or wrong group names in `inventory.ini` caused errors.

- **YAML Syntax:**  
  Indentation and colon mistakes led to parsing errors—always double-check YAML!

- **Command Line Variables:**  
  Learned to use `-e "VAR=value"` for passing variables at runtime.

---

## 📚 How to Use This Repo

1. **Clone the repository:**
   ```bash
   git clone <your-repo-url>
   cd learnAnsible
   ```

2. **Set up your inventory:**
Edit inventory.ini with your server details.

3. **Run a playbook:**
   ```bash
   ansible-playbook -i inventory.ini 01-playbook.yaml
   ```
4. **Try different playbooks:**
Explore each YAML file to learn a new concept!

##🌟 Why Learn Ansible?
- Automate repetitive tasks 🛠️
- Ensure consistency across servers 🔄
- Easily manage complex deployments 🚀
- Grow your DevOps skills 📈

## 📖 My Ansible Learning Journey 🚀✨

Explore my continuous learning adventure across these repositories, each showcasing different facets of my Ansible mastery:

- 📘 [learnAnsible](https://github.com/MAHALAKSHMImahalakshmi/learnAnsible.git) – Hands-on tutorials and practical playbooks to build your Ansible foundation.
- 🛠️ [ansibleRoboshop](https://github.com/MAHALAKSHMImahalakshmi/ansibleRoboshop.git) – Real-world microservices automation project applying modular Ansible practices.
- 📦 [rolesAnsibleRoboshop](https://github.com/MAHALAKSHMImahalakshmi/rolesAnsibleRoboshop.git) – Deep dive into reusable Ansible roles and advanced troubleshooting techniques.

Feel free to dive in, contribute, or ask questions anytime! Let’s collaborate and level-up automation skills together! 💡🤝✨

---

## 🙏 Credits & Contact 💬🤗

- Inspired by the innovative Roboshop microservices architecture and design pattern.  
- Automation and documentation craft by [Mahalakshmi](https://github.com/MAHALAKSHMImahalakshmi) 💻❤️

---


