# Security Audit Report

## 1. Principle of Least Privilege (PoLP)

The Principle of Least Privilege means that users and services should receive only the permissions they need to perform their tasks. This reduces the chance that an account or service can access sensitive resources unnecessarily. In cloud environments, it helps limit the damage caused by compromised accounts.

## 2. Attack Surface

The attack surface of a virtual machine includes all the points where an attacker could attempt to access or affect the system. Examples include open network ports, running services, and exposed applications. Reducing unnecessary services and open ports helps make the server harder to attack.

## 3. Default Deny Policy

A Default Deny policy blocks incoming network traffic unless a specific rule allows it. This is safer than trying to block individual attackers because unknown or unauthorized connections are blocked automatically. Only the services that are genuinely needed should be allowed through the firewall.
