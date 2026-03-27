# Suspicious Admin Login Detection

## Description

Monitors successful login activity from privileged accounts.

## Threat Scenario

Unauthorized access using compromised admin credentials.

## Detection Logic

* Event ID: 4624 (Successful Login)
* Filter: Admin accounts

## Response Actions

* Validate login source
* Confirm user activity
* Check for privilege escalation
