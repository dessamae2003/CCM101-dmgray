# Multi-Tier Architecture Documentation

## Definition of Two-Tier Architecture
A **Two-Tier Architecture** is a software design pattern where an application is split into two distinct, physically or logically separated tiers: the **Web/Application Tier** and the **Database Tier**. Instead of bundling everything into a single container or server, each tier handles a specialized responsibility, communicating across a secure internal network.

---

## 1. The Web/Application Tier
* **Role:** The application tier serves the user interface, manages incoming HTTP/HTTPS requests from clients, executes core business logic, and renders the application pages (in this deployment, powered by Nextcloud).

---

## 2. The Database Tier
* **Role:** The database tier is dedicated to storing, retrieving, and managing persistent data securely, including user credentials, configuration settings, and file metadata (in this deployment, powered by MariaDB).

---

## Why Separate Them?
Separating the web server and the database into two distinct containers instead of packing them into a single monolithic package provides critical operational benefits. It enhances security by isolating database access, allows independent scaling of compute versus storage resources, and simplifies troubleshooting and maintenance since each container can be updated or replaced independently.
