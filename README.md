# Terraform-GCP-VM-provisioning-project
Terraform GCP VM provisioning projec


```markdown
# 🚀 GCP VM Provisioning with Terraform

This project automates the provisioning of **multiple Virtual Machines (VMs)** on **Google Cloud Platform (GCP)** using **Terraform**. It follows a modular and clean structure suitable for scaling and reuse.

## 📂 Project Structure

```
terraform-gcp-vm/
├── main.tf              # Core logic to provision GCP VM instances
├── provider.tf          # GCP provider setup with credentials & project info
├── variables.tf         # Input variables declaration (region, VM count, etc.)
├── terraform.tfvars     # Values assigned to the declared variables
├── output.tf            # Outputs such as VM names and external IPs
├── main-connect.sh      # (Optional) Bash script to SSH into the provisioned VMs
├── .gitignore           # Ignore sensitive or local files (e.g., credentials)
└── README.md            # Project overview and usage instructions
```

---

## ✅ What This Does

- Provisions **5 Virtual Machines** (configurable) on GCP
- Uses Terraform to fully automate infra lifecycle
- Cleanly separates configuration into manageable files
- Optionally includes a connection script for SSH access

---

## ⚙️ Prerequisites

- A GCP account with billing enabled
- A service account key file (JSON) with Compute Admin permissions
- Terraform installed on your local machine

---

## 🚀 How to Use

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/terraform-gcp-vm.git
   cd terraform-gcp-vm
   ```

2. **Update terraform.tfvars**
   ```hcl
   project_id   = "your-gcp-project-id"
   region       = "us-central1"
   zone         = "us-central1-a"
   vm_count     = 5
   machine_type = "e2-medium"
   ```

3. **Export your service account credentials**
   ```bash
   export GOOGLE_APPLICATION_CREDENTIALS="path/to/your-service-account-key.json"
   ```

4. **Run Terraform Commands**
   ```bash
   terraform init
   terraform plan
   terraform apply
   ```

5. **(Optional) SSH into VMs**
   ```bash
   bash main-connect.sh
   ```

6. **To Destroy the Setup**
   ```bash
   terraform destroy
   ```

---


---

## 🙌 Contributions

Feel free to fork the repo, raise PRs, or suggest improvements. Let’s build better infra together! 🚀

---

## 📬 Contact

Reach out to me on [LinkedIn](www.linkedin.com/in/shivaknya-kadam1234) if you have any questions or just want to connect!

---

## 🏷️ Tags

`Terraform` `GCP` `DevOps` `IaC` `Automation` `VM Provisioning` `Google Cloud`

```

--
