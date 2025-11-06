# DevOps Intern Final Assessment

**Name:** Ravi sankar Manem  
**Date:** 06/11/2025

## Project Description

This project demonstrates a **DevOps workflow** using open-source tools including **Linux, Docker, CI/CD (GitHub Actions), Nomad, and monitoring (Grafana Loki)**.  
Each step in the workflow produces real, usable output for the next, simulating a small but realistic DevOps pipeline.

---

## Project Steps Overview

1. **Git & GitHub Setup**  
   - Repository initialized with README.md  
   - Sample script `hello.py` prints "Hello, DevOps!"  

2. **Linux & Scripting Basics**  
   - Folder: `scripts/`  
   - Script: `sysinfo.sh` prints:
     - Current user
     - Current date
     - Disk usage  
   - Script made executable and tested

3. **Docker Basics**  
   - `Dockerfile` containerizes `hello.py`  
   - Runs `python hello.py` on container startup  
   - Instructions included to build and run locally

4. **CI/CD with GitHub Actions**  
   - Workflow file: `.github/workflows/ci.yml`  
   - Automatically runs `hello.py` on every push  
   - Status badge included in README

5. **Job Deployment with Nomad**  
   - Nomad job file: `nomad/hello.nomad`  
   - Runs Docker container as a service with minimal resources  
   - Instructions included to run Nomad job

6. **Monitoring with Grafana Loki**  
   - Loki configured (Docker-based)  
   - Logs from containers forwarded to Loki  
   - Instructions and setup notes in `monitoring/loki_setup.txt`

7. **Extra Credit (Optional)**  
   - Optional MLflow tracking or VM deployment for advanced workflow

---

## How to Run

### Linux Script
```bash
cd scripts
./sysinfo.sh
