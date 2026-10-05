# Implementing Microsoft Entra PIM Just-In-Time (JIT) Workflow: Security Administrator Role

This guide walks through configuring, requesting, and approving Just-In-Time (JIT) privileged access using Microsoft Entra Privileged Identity Management (PIM) for SC-300 exam preparation and portfolio documentation.

---

## Step 1: PIM Overview & Setup
We start by reviewing the core Privileged Identity Management dashboard to manage access workflows.
* **Dashboard View:** Access the main PIM interface to oversee role assignments and security governance.

![Dashboard](Dashboard.jpg)

---

## Step 2: Assigning Eligible Roles
Next, we select the specific administrative role to restrict under JIT control. Here, we choose the **Security Administrator** role from the directory to make users eligible rather than permanently active[cite: 15].

![Choosing Roles](choosing%20roles.jpg)

---

## Step 3: Auditing Role Assignments
After making the user (`damencruz`) eligible, we verify the action details and transaction logs in the audit history.

![PIM Audit History](PIM%20audit%20History.jpg)

---

## Step 4: Role Activation Stage (JIT Request)
Logged in as the test user (`damencruz`), we navigate to **My roles** where the *Security Administrator* role appears under **Eligible assignments**. Clicking **Activate** begins the JIT escalation process.

![Role Activation Stage](role%20activation%20stage.jpg)

---

## Step 5: Configuring Approval Policies
As a Global Administrator, we update the role settings to require explicit activation approval and designate authorized approvers (such as `maximo dawan`) to govern privilege elevations[cite: 13].

![Approval on Roles](approval%20on%20roles.jpg)

---

## Step 6: Reviewing and Approving Requests
Once the user submits an activation request with a business justification, the designated administrator reviews it in the **Approve requests** queue and grants approval[cite: 14].

![Approving Role Assignment](approving%20role%20assignment.jpg)

---

## Step 7: Verifying Active Elevation
Finally, returning to the user's PIM dashboard under **Active assignments**, we confirm that the *Security Administrator* role is successfully activated with its active session countdown[cite: 16].

![Confirming Role Activated](confirming%20role%20already%20activated.jpg)
