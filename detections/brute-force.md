# Brute Force Login Detection

## Description

Detects multiple failed login attempts from a single IP address within a short time window.

## Threat Scenario

An attacker attempts to gain access by repeatedly trying different passwords.

## Detection Logic

* Event ID: 4625 (Failed Login)
* Threshold: More than 5 attempts within 5 minutes

## KQL Query

(See queries/brute-force.kql)

## Response Actions

* Investigate source IP address
* Check for successful login attempts
* Block IP if malicious activity confirmed
* Reset affected user credentials

## Severity

Medium to High
