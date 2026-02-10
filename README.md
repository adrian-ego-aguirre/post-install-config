<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket Logo"/>
</p>

<h1 align="center">osTicket – Phase 2: Post-Installation Configuration</h1>

<p>
This lab documents the post-installation configuration of <strong>osTicket</strong>, transforming the platform from an initial (Alpha) installation into a fully functional help desk capable of handling real-world support tickets, users, and service workflows.
</p>

---

<h2>🛠 Environments & Technologies Used</h2>

<ul>
  <li>Microsoft Azure (Virtual Machines)</li>
  <li>Remote Desktop Protocol (RDP)</li>
  <li>Internet Information Services (IIS)</li>
  <li>osTicket Help Desk System</li>
</ul>

---

<h2>💻 Operating Systems Used</h2>

<ul>
  <li>Windows 10 (21H2)</li>
</ul>

---

<h1>📌 Phase 2 Overview – Post-Installation Configuration</h1>

<p>
<strong>Goal:</strong> Configure core osTicket components to support structured ticket intake, prioritization, escalation, and resolution in a simulated enterprise help desk environment.
</p>

<p>
This phase focuses on configuring internal workflows, access controls, and service policies required for daily IT operations.
</p>

---

<h2>Key Components Configured</h2>

<ul>
  <li><strong>Roles:</strong> Define agent permissions and administrative access.</li>
  <li><strong>Departments:</strong> Route tickets based on organizational responsibility.</li>
  <li><strong>Teams:</strong> Group agents by support tier or function.</li>
  <li><strong>Agents:</strong> Staff members responsible for ticket resolution.</li>
  <li><strong>Users:</strong> End users who submit support requests.</li>
  <li><strong>SLAs:</strong> Enforce response and resolution timeframes.</li>
  <li><strong>Help Topics:</strong> Categorize and route incoming tickets.</li>
</ul>

---

<h2>Configuration Outline</h2>


<h2>1️⃣ Configure Roles</h2>
<img width="962" height="737" alt="P2-1-Roles" src="https://github.com/user-attachments/assets/6fe24816-63b7-47cc-ad0b-a88a53f69f66" />

<ul>
  <li>Navigate to: <em>Admin Panel → Agents → Roles</em></li>
  <li>Create an administrative role with full permissions (e.g., <strong>Supreme Admin</strong>).</li>
  <li>Assign permissions to manage tickets, users, and system settings.</li>
</ul>

---

<h2>2️⃣ Configure Departments</h2>
<img width="960" height="855" alt="P2-2-Departments" src="https://github.com/user-attachments/assets/1bdc29f8-c920-42ec-9834-7c1de932bb5c" />

<ul>
  <li>Navigate to: <em>Admin Panel → Agents → Departments</em></li>
  <li>Create a department named <strong>System Administrators</strong>.</li>
  <li>Assign department-level visibility and escalation rules.</li>
</ul>

---

<h2>3️⃣ Configure Teams</h2>
<img width="960" height="710" alt="P2-3-Teams" src="https://github.com/user-attachments/assets/b03f456a-2894-47d8-8d1c-81b0dcab795e" />

<ul>
  <li>Navigate to: <em>Admin Panel → Agents → Teams</em></li>
  <li>Create <strong>Level I Support</strong> and <strong>Level II Support</strong> teams.</li>
  <li>Assign agents based on escalation level.</li>
</ul>

---

<h2>4️⃣ Configure Agents (Support Staff)</h2>
<img width="957" height="926" alt="P2-4-Agents" src="https://github.com/user-attachments/assets/caab82b8-9db3-402e-8dbf-7b3edd02779f" />

<ul>
  <li>Navigate to: <em>Admin Panel → Agents → Add New</em></li>
  <li>Create agents (e.g., Jane, John).</li>
  <li>Assign roles, departments, and teams accordingly.</li>
</ul>

---

<h2>5️⃣ Configure Users (End Customers)</h2>
<img width="644" height="393" alt="P2-5-Users" src="https://github.com/user-attachments/assets/f272cd6e-3f82-48db-bb7f-45fbe304a920" />

<ul>
  <li>Navigate to: <em>Agent Panel → Users → Add New</em></li>
  <li>Create end users (e.g., Karen, Ken).</li>
  <li>Verify users can submit tickets successfully.</li>
</ul>

---

<h2>6️⃣ Configure Service Level Agreements (SLAs)</h2>
<img width="960" height="666" alt="P2-6-SLAs" src="https://github.com/user-attachments/assets/e0c357c7-4845-4c2a-8e78-718f4992fe75" />

<p>
SLAs define expected response and resolution times based on ticket severity. Proper SLA configuration ensures high-priority incidents receive immediate attention.
</p>

<ul>
  <li>Navigate to: <em>Admin Panel → Manage → SLA</em></li>
  <li>Create the following SLA policies:
    <ul>
      <li><strong>Sev-A:</strong> 1 hour, 24/7 coverage (critical outages)</li>
      <li><strong>Sev-B:</strong> 4 hours, 24/7 coverage (high-priority issues)</li>
      <li><strong>Sev-C:</strong> 8 hours, business hours (standard requests)</li>
    </ul>
  </li>
</ul>

---

<h2>7️⃣ Configure Help Topics</h2>
<img width="959" height="635" alt="P2-7-Help-Topics" src="https://github.com/user-attachments/assets/908c9ffe-b028-4a76-b7d6-ff3b04394e01" />

<p>
Help topics categorize incoming tickets and automate routing to the appropriate department or team.
</p>

<ul>
  <li>Navigate to: <em>Admin Panel → Manage → Help Topics</em></li>
  <li>Create common help topics such as:
    <ul>
      <li>Business Critical Outage</li>
      <li>Personal Computer Issues</li>
      <li>Equipment Request</li>
      <li>Password Reset</li>
    </ul>
  </li>
</ul>

---

<h2>✅ Key Takeaways</h2>

<ul>
  <li>Structured roles and departments improve ticket accountability</li>
  <li>SLAs enforce response discipline and service quality</li>
  <li>Help topics streamline ticket routing and escalation</li>
  <li>Proper configuration mirrors real enterprise ITSM workflows</li>
</ul>

---

<h2>📌 Conclusion</h2>

<p>
This phase completed the transformation of osTicket from a basic installation into a fully operational help desk system. By configuring roles, departments, teams, agents, users, SLAs, and help topics, the platform now supports structured ticket intake, prioritization, and resolution workflows.
</p>

---

<h2>➡️ Next Phase</h2>

<p>
Continue to <strong>Phase 3: Ticket Lifecycle & SLAs</strong>, where the full lifecycle of a ticket—from intake to resolution—is demonstrated using SLAs, escalation, and agent workflows.
</p>

<p>
<a href="https://github.com/adrian-ego-aguirre/ticket-lifecycle">
  ➜ Go to Phase 3: Ticket Lifecycle & SLAs
</a>
</p>
