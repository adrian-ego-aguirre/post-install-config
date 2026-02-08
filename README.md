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

<ul>

  <li>
    <strong>Configure Roles</strong>
    <ul>
      <li>Navigate to: <em>Admin Panel → Agents → Roles</em></li>
      <li>Create an administrative role with full permissions (e.g., <strong>Supreme Admin</strong>).</li>
      <li>Assign permissions to manage tickets, users, and system settings.</li>
    </ul>
  </li>

  <li>
    <strong>Configure Departments</strong>
    <ul>
      <li>Navigate to: <em>Admin Panel → Agents → Departments</em></li>
      <li>Create a department named <strong>System Administrators</strong>.</li>
      <li>Assign department-level visibility and escalation rules.</li>
    </ul>
  </li>

  <li>
    <strong>Configure Teams</strong>
    <ul>
      <li>Navigate to: <em>Admin Panel → Agents → Teams</em></li>
      <li>Create <strong>Level I Support</strong> and <strong>Level II Support</strong> teams.</li>
      <li>Assign agents based on escalation level.</li>
    </ul>
  </li>

  <li>
    <strong>Configure Agents (Support Staff)</strong>
    <ul>
      <li>Navigate to: <em>Admin Panel → Agents → Add New</em></li>
      <li>Create agents (e.g., Jane, John).</li>
      <li>Assign roles, departments, and teams accordingly.</li>
    </ul>
  </li>

  <li>
    <strong>Configure Users (End Customers)</strong>
    <ul>
      <li>Navigate to: <em>Agent Panel → Users → Add New</em></li>
      <li>Create end users (e.g., Karen, Ken).</li>
      <li>Verify users can submit tickets successfully.</li>
    </ul>
  </li>

  <li>
    <strong>Configure Service Level Agreements (SLAs)</strong>
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
  </li>

  <li>
    <strong>Configure Help Topics</strong>
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

<p>
This configuration reflects real-world IT service management practices and prepares the environment for handling live support requests efficiently and securely.
</p>
