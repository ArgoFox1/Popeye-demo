# Popeye Installation and Usage Guide

![popeye_logo](https://github.com/user-attachments/assets/c8675a7c-561b-4a04-886c-2d2f807910af)

* Installation for OSX/Unit using Homebrew/LinuxBrew

   ```shell
   brew install popeye
   ```
* Verifying Popeye Installation
  
   ```shell
   popeye version
   ```
* Download and Install Metrics Server for Kubernetes Data and Logs Collection
  
   ```shell
   git clone https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
      
* Editing the Metrics components.yaml File

  Add the code highlighted in red as shown in the image below:
  ![Screenshot from 2025-01-13 14-01-08](https://github.com/user-attachments/assets/e6b80588-323d-4153-9d50-6a12663b44a9)

* Apply Metrics Server to Kubernetes
    
   ```shell
   kubectl apply -f components.yaml
      
* Checking Metrics Server Status
  To verify the status of the Metrics Server, ensure it is running, then proceed to the next step.
   ```shell
   kubectl get pods -n kube-system
   ```
![older  Çalışıyor  - Oracle VM VirtualBox _ 1 13 01 2025 15_11_09](https://github.com/user-attachments/assets/63e141dc-5e0e-430a-a708-a1c9b0d790ea)

* Run Popeye
   ```shell
   popeye
   ```
   ![older  Çalışıyor  - Oracle VM VirtualBox _ 1 2025-01-13 14-33-53 (2)](https://github.com/user-attachments/assets/61239058-e413-4fd1-84b2-90c899686bf7)

