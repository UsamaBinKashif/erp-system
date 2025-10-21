# Modern Modular ERP System

##  Summary

This repository is a **production-grade** ERP monorepo.  
It uses a **microservice-based architecture**, managed through **Turborepo**, with **shared packages** for consistent typing, validation, and communication between services.

Each service — such as Accounting, HR, Inventory, CRM, and Notifications — runs independently but communicates through **Pub/Sub** and shared ** schemas**.  
Frontend and backend share DTOs and validation logic for a fully type-safe development experience.
