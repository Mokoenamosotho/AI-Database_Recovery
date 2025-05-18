# AI-Database_Recovery

# Reflection on Repository Improvement and Open-Source Collaboration

# 💾 AI-Database_Recovery System

An intelligent, automated **Hospital Database Management System** that integrates **AI-driven failure prediction**, **secure backup and recovery**, and **regulatory compliance** (POPIA, HIPAA). This project demonstrates how to design, model, and implement a resilient database infrastructure using **UML class diagrams**, **creational design patterns**, and **unit-tested C# code**.

---

## 📌 Project Overview

This system is designed to support hospital or enterprise IT environments by:
- Automatically backing up databases every 24 hours.
- Predicting failures using AI and alerting IT staff proactively.
- Supporting manual and automated recovery with RTO ≤ 30 mins and RPO ≤ 1 hour.
- Ensuring end-to-end encryption and detailed audit logging for compliance.


## 1. Improving the Repository Based on Peer Feedback

After sharing my Hospital Database Management System repository with peers, their feedback significantly improved the project’s quality and accessibility. Initially, the contribution guidelines were quite basic, which made onboarding new contributors difficult. Based on feedback, I expanded the `CONTRIBUTING.md` file to include detailed setup instructions, coding standards, and a clear, step-by-step guide on picking issues and submitting pull requests. This made it easier for newcomers to get started and understand expectations.

Peers also highlighted the importance of issue labeling for discoverability. To address this, I added labels such as `good-first-issue` for beginner-friendly tasks and `feature-request` for desired enhancements. This helped contributors quickly identify tasks suited to their experience and interests, encouraging more diverse participation.

Furthermore, a suggestion to include a `ROADMAP.md` was invaluable. The roadmap provides transparency around future features and priorities, helping contributors align their efforts with the project’s goals. Finally, integrating GitHub templates for issues and pull requests improved communication and standardized contributions, making the review process smoother and more efficient.

## 2. Challenges in Onboarding Contributors

Onboarding contributors presented several challenges. The domain—hospital database management—is inherently complex, which sometimes overwhelmed newcomers unfamiliar with healthcare or database concepts. To mitigate this, thorough documentation was necessary to simplify domain knowledge and clearly define manageable tasks for beginners.

Maintaining code quality and consistency across contributions was another challenge. Multiple contributors bring diverse coding styles and approaches, so establishing and enforcing coding standards through linters, tests, and contribution guidelines became essential. Setting up automated CI pipelines to run tests helped uphold these standards but required careful configuration.

Effective communication was also a hurdle. Explaining architectural decisions and guiding contributors through complex issues required patience and clarity. Creating detailed documentation and examples helped, but direct engagement and responsiveness were key to keeping contributors motivated and productive.

Lastly, sustaining contributor motivation beyond initial contributions is a common challenge. Building a welcoming and inclusive community environment is vital for long-term engagement.

## 3. Lessons Learned About Open-Source Collaboration

This experience reinforced that successful open-source projects rely equally on technical excellence and strong community management. Clear, comprehensive documentation is the foundation—it lowers barriers to entry and empowers contributors. Issue labeling and project roadmaps increase transparency and help contributors find suitable tasks aligned with their skills and interests.

Community interaction matters greatly. Prompt, constructive feedback and open communication foster trust and encourage participation. Collaboration thrives in an environment where contributors feel heard and supported.

Finally, I learned that open-source projects evolve through continuous, incremental improvements. No project starts perfect. Incorporating feedback, adapting workflows, and transparently sharing the project’s direction help build a sustainable, vibrant community over time.

🧠 Features

| Feature                  | Description                                                    |
| ------------------------ | -------------------------------------------------------------- |
| 🔁 Auto Backup           | Schedules encrypted backups every 24 hours                     |
| ⚠️ AI Failure Prediction | Uses AIModel to predict failures with 95% accuracy             |
| 🧩 Manual Override       | Allows DBAs to manually trigger or override recovery processes |
| 📈 Real-time Monitoring  | Dashboard view of live database health                         |
| 🔐 AES-256 Encryption    | Ensures all backups are securely stored                        |
| 📜 Compliance Reports    | POPIA/HIPAA-compliant audit trail and reports                  |
| 🧪 Unit Tested           | All object creation logic validated via NUnit tests            |
| 🏗️ Design Patterns      | Implements all six major creational patterns (see below)       |

---
Creational Design Patterns Used

| Pattern              | Purpose                                            |
| -------------------- | -------------------------------------------------- |
| Simple Factory 🏭    | Central object creation (e.g., Backup or Database) |
| Factory Method 🧱    | Different recovery strategies                      |
| Abstract Factory 🏗️ | UI component rendering (e.g., Windows/Mac buttons) |
| Builder 🍕           | Build complex backup configurations step-by-step   |
| Prototype 🧬         | Clone configured Database objects quickly          |
| Singleton 🔒         | Maintain single active DB connection instance      |


| Module                  | Open for Contribution? | Suggestions                                            |
| ----------------------- | ---------------------- | ------------------------------------------------------ |
| AIModel Training Logic  | ✅                      | Improve accuracy or switch to real ML frameworks       |
| Storage Abstraction     | ✅                      | Add SQL/NoSQL repositories to replace in-memory        |
| Compliance Reporting UI | ✅                      | Add frontend dashboard for report visualization        |
| Monitoring Dashboard    | ✅                      | Integrate real-time health metrics via SignalR or gRPC |
| Recovery Optimization   | ✅                      | Test against large-scale database simulations          |

📂 Folder Structure
/AI-Database_Recovery
│
├── /DesignPatterns         # Creational pattern examples
├── /DomainModels           # Core entities (Database, Backup, etc.)
├── /Repositories           # In-memory and factory-based storage
├── /Tests                  # NUnit test cases
├── README.md
└── ... (Solution files)


## 🚀 Getting Started

### Prerequisites
- [.NET SDK 7+](https://dotnet.microsoft.com/)
- Visual Studio or any C# IDE
- NUnit or preferred test runner for unit tests

### Setup Instructions
```bash
git clone https://github.com/Mokoenamosotho/AI-Database_Recovery.git
cd AI-Database_Recovery
dotnet restore
dotnet build
dotnet test




## Getting Started

### Clone and Build
```bash
git clone https://github.com/Mokoenamosotho/hospital-dbms.git
cd hospital-dbms
dotnet restore
dotnet build
