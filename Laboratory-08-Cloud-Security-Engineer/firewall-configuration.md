# Firewall Configuration

## Allow SSH

Command used:

`sudo ufw allow ssh`

This rule permits SSH connections so administrators can manage the server remotely.

## Default Deny Policy

Commands used:

`sudo ufw default deny incoming`

`sudo ufw default allow outgoing`

The default deny incoming policy blocks unsolicited incoming connections unless an explicit firewall rule allows them. The default allow outgoing policy permits outbound connections.

## Allow the Web Application

Command used:

`sudo ufw allow 8080/tcp`

This rule permits TCP traffic on port 8080 for the Nginx web application.

## Firewall Verification

Command used:

`sudo ufw status verbose`

This command verifies that UFW is active and displays the configured default policies.

Command used:

`sudo ufw status numbered`

This command displays the numbered firewall rules.

## Security Note

If `sudo ufw enable` is run before `sudo ufw allow ssh`, SSH access may be blocked by the default deny incoming policy, potentially locking out a remote administrator.
