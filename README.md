# 📅 Workshop Register Notifier (n8n Workflow Automation)
🔍 *n8n • Google Sheets • Gmail • Automation*

## 🚀 Tech Stack & Domains
![n8n](https://img.shields.io/badge/Automation-n8n-orange)
![Google Sheets](https://img.shields.io/badge/Storage-Google%20Sheets-green)
![Gmail](https://img.shields.io/badge/Email-Gmail-red)
![Domain](https://img.shields.io/badge/Domain-Workflow%20Automation%20%26%20Notifications-navy)

---

## 📘 Overview
**Workshop Register Notifier** is an **n8n-based automation workflow** that monitors workshop registration data and automatically sends notification emails.

The workflow checks Google Sheets on a scheduled basis, processes new registration records, and notifies users via Gmail—without any manual intervention.

---

## 🎯 Problem Statement
Workshop organizers often rely on manual checks to track new registrations and send confirmation or notification emails. This process is:
- Time-consuming  
- Easy to miss updates  
- Difficult to scale with growing registrations  

This project automates the entire notification flow using **n8n**.

---

## 🗺️ Workflow Logic

### 🔁 Workflow Steps
1. **Schedule Trigger**
   - Runs at defined intervals

2. **Google Sheets — Read & Clean**
   - Reads registration data
   - Removes or clears previously processed entries

3. **IF Node Validation**
   - If data is empty → workflow stops
   - If data exists → continue processing

4. **Google Sheets — Append**
   - Appends validated data into notifier sheet

5. **Gmail — Send Email**
   - Sends notification email using Gmail

6. **Google Sheets — Log**
   - Stores notification history

---

## 🧰 Tools & Integrations
- **n8n** (workflow orchestration)
- **Schedule Trigger**
- **Google Sheets** (data source + storage)
- **IF Node** (conditional logic)
- **Gmail** (email notifications)

---

## 📤 Output
- Automated **email notifications** sent via Gmail
- Google Sheets updated in real time

---



## 🛠️ Setup & Execution

### Prerequisites
- n8n (localhost or cloud)
- Google account
- Gmail access enabled

### Steps
1. Create a new workflow in n8n
2. Import workflow from file or URL
3. Configure Google Sheets credentials
4. Configure Gmail credentials
5. Set schedule trigger
6. Activate workflow

---

## 🔒 Notes
- Built using **n8n only**
- Works on localhost or cloud n8n setup
- No external backend required
- Fully visual workflow using n8n canvas

