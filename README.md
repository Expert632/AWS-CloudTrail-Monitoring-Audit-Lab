AWS CloudTrail Monitoring & Audit Lab

### Track, Analyze and Alert on AWS Activity

This hands-on lab demonstrates how to **monitor and audit activity in AWS using CloudTrail**, a key service for **security, compliance, and troubleshooting**.

In cloud environments, it is essential to know:

* who did what
* when actions were performed
* which resources were affected

CloudTrail provides **full visibility of API activity across AWS**, making it a critical tool for **Cloud Security and DevSecOps**.

---

# 🧠 What You Will Learn

This lab introduces the core concepts of **cloud auditing and monitoring**:

| Concept       | Explanation                              |
| ------------- | ---------------------------------------- |
| CloudTrail    | Tracks all AWS API activity              |
| Trail         | Configuration that records events        |
| Event History | View recent account activity             |
| S3 Storage    | Stores logs securely                     |
| CloudWatch    | Monitors logs and triggers alerts        |
| Alerts        | Notifies when suspicious activity occurs |

These are essential for **security monitoring and compliance**.

---

# 🏗 Lab Architecture

The monitoring workflow implemented in this lab:

```id="ct001"
AWS API Activity
        ↓
CloudTrail (Event Tracking)
        ↓
Logs stored in S3
        ↓
CloudWatch Logs
        ↓
Alarm
        ↓
Notification / Action
```

This architecture ensures **full traceability and real-time alerting**.

---

# ⚙️ Lab Steps

## Step 1 — Access AWS CloudTrail

Start by logging into the AWS Console and navigating to **CloudTrail**.

CloudTrail is the service responsible for **tracking all actions performed in your AWS account**.

---

# 🛠 Step 2 — Enable and Create a Trail

Create a **Trail** to start recording activity.

A trail allows you to:

* capture API calls
* track user actions
* monitor resource changes

Once enabled, CloudTrail continuously records **all events in your account**.

---

# 📦 Step 3 — Configure S3 Storage

Configure an **Amazon S3 bucket** to store CloudTrail logs.

Benefits:

* durable storage
* secure access
* long-term audit retention

Logs stored in S3 allow you to **analyze historical activity**.

---

# 🔍 Step 4 — View Events (Event History)

Go to:

```
CloudTrail → Event History
```

Here you can see:

* user activity
* API calls
* timestamps
* affected resources

This provides a **real-time view of AWS account activity**.

---

# 🔎 Step 5 — Filter Logs

Use filters to find specific events.

Examples:

* filter by user
* filter by resource
* filter by event type

Filtering helps quickly **identify suspicious or relevant actions**.

---

# ☁️ Step 6 — Send Logs to CloudWatch

Integrate CloudTrail with **Amazon CloudWatch**.

This allows you to:

* monitor logs in real time
* create metrics
* trigger alerts

CloudWatch enhances **visibility and automation**.

---

# 🚨 Step 7 — Create an Alert

Create a **CloudWatch Alarm** based on specific events.

Example:

```id="ct002"
If unauthorized API call detected → Trigger Alert
```

Alerts help detect:

* suspicious activity
* unauthorized access
* security incidents

---

# 🔔 Step 8 — Notification

Configure notifications (e.g., via SNS).

Workflow:

```id="ct003"
CloudTrail Event → CloudWatch Alarm → Notification
```

This ensures that you are **immediately informed of important events**.

---

# 🛡 Security Best Practices Demonstrated

This lab demonstrates key **cloud security practices**:

✔ Enable full activity logging
✔ Store logs securely in S3
✔ Monitor events in real time
✔ Filter and analyze logs
✔ Create alerts for suspicious activity
✔ Enable automated notifications

These practices are used in **production cloud environments**.

---

# 🎯 Skills Demonstrated

Completing this lab demonstrates knowledge of:

* AWS CloudTrail auditing
* Log management and analysis
* CloudWatch monitoring
* Alerting and notification systems
* Cloud security and compliance

These skills are valuable for:

* Cloud Engineer
* DevOps Engineer
* DevSecOps Engineer
* Security Analyst

---

# 🚀 Why This Lab Matters

Without logging:

* security incidents go unnoticed
* actions cannot be traced
* compliance is impossible

With CloudTrail:

✔ full visibility
✔ better security
✔ faster incident response

This lab demonstrates how to **track, analyze, and respond to cloud activity effectively**.

