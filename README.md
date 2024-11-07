# Apache Virtual Host Configuration with Ansible

This repository contains an Ansible playbook designed to configure Apache (httpd) with specific settings on a Linux server. It sets up virtual hosts, SELinux rules, IP-based access restrictions, separate logging for each virtual host, and password-protected directories using `.htaccess` and `.htpasswd`.

## Features

- **SELinux Port Configuration**: Configures SELinux to allow Apache to listen on a specified custom port.
- **IP-based Directory Access Restriction**: Limits access to certain directories by allowing only specific IPs.
- **Virtual Host Configuration with Logging**: Sets up virtual hosts with dedicated error and access logs.
- **Password-Protected Directories**: Creates private directories under each virtual host with basic authentication.

## Requirements

- **Ansible**: Make sure Ansible is installed on your control machine. You can install it using:
  ```bash
  sudo apt update
  sudo apt install ansible
