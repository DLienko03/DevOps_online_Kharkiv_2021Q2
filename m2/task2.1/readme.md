# Task 2.1 report

## Part 1. HYPERVISORS
### 1)What are the most popular hypervisors for infrastructure virtualization?
    Type 1 hypervisors are The most popular ones for infrastructure virtualization. They can
    be divide into type 3(monolithic) and 4(microkernel). Example of 3-rd type is VMware ESX,
    example of 4-th - Microsoft Hyper -V.
      
### 2)Briefly describe the main differences of the most popular hypervisors.
    Type 1 hypervisor works above hardware(without host OS between them). Type 2 - inside host OS,
    so it works simultaneously with other applications in host OS (VirtualBox, VMWare). Type 3-4 are 
    subptypes of Type 1. Type 3 (Monolitic) hypervisor (VMware ESX) manages virtual stack and drivers 
    itself, while type 4 (Microkernel) (Microsoft Hyper -V) delegates this tasks to virtual machines.
      
## PART 2. WORK WITH VIRTUALBOX
### 1)First run VirtualBox and Virtual Machine (VM) </br>
   * 1.1-1.5: </br> ![image](https://user-images.githubusercontent.com/80945113/112326642-5a805700-8cbd-11eb-9668-4f9a9eae9d18.png)</br>
                  ![image](https://user-images.githubusercontent.com/80945113/112326712-69ffa000-8cbd-11eb-9a7a-933148953c39.png)</br>
   * 1.6-1.7: </br> ![image](https://user-images.githubusercontent.com/80945113/112327459-1e012b00-8cbe-11eb-8937-c4422c9e9d6a.png)</br>
                  ![image](https://user-images.githubusercontent.com/80945113/112327592-396c3600-8cbe-11eb-922b-179ee43011aa.png)</br>
   * 1.8: </br> ![image](https://user-images.githubusercontent.com/80945113/112327893-7b957780-8cbe-11eb-8ded-633f08de2039.png)</br>
   * 1.9: </br> ![image](https://user-images.githubusercontent.com/80945113/112328133-b7304180-8cbe-11eb-8cf6-5e84b1998073.png)</br>
  
### 2)Configuration of virtual machines</br>
  2.3 shared_folder: </br> ![image](https://user-images.githubusercontent.com/80945113/112328678-3d4c8800-8cbf-11eb-9775-4a9ed557ed9d.png)</br>
  2.4 configure network modes </br>
  * NAT: </br> ![image](https://user-images.githubusercontent.com/80945113/112329454-e2676080-8cbf-11eb-8bf2-8ff35a860503.png)</br>
  * Host-only: </br> ![image](https://user-images.githubusercontent.com/80945113/112329913-44c06100-8cc0-11eb-9f6f-ddde01a816e7.png)</br>
  * Bridged: </br> ![image](https://user-images.githubusercontent.com/80945113/112329575-fca13e80-8cbf-11eb-88ea-d26cd3578c5f.png)</br>
  * Results: </br> ![image](https://user-images.githubusercontent.com/80945113/112332058-19d70c80-8cc2-11eb-99b1-0471f7ac4db8.png)</br>
  
### 3)Work with CLI through VBoxManage.</br>
###  Examples of some commands:
  ![image](https://user-images.githubusercontent.com/80945113/112332465-6de1f100-8cc2-11eb-926a-89d1763c8a8a.png)
  ![image](https://user-images.githubusercontent.com/80945113/112332509-776b5900-8cc2-11eb-8336-832dedf37a1b.png)
  ![image](https://user-images.githubusercontent.com/80945113/112332556-82be8480-8cc2-11eb-9c29-79d3f5bf4ca6.png)
  
## PART 3. WORK WITH VAGRANT
### 1-4(install, init enviroment):</br>
  ![image](https://user-images.githubusercontent.com/80945113/112334194-ed23f480-8cc3-11eb-902e-c2db449ea807.png)</br>

### 5-6(connect via putty):</br>
  ![image](https://user-images.githubusercontent.com/80945113/112334670-44c26000-8cc4-11eb-8775-94d07e4d63e6.png)</br>

### 7(stop and delete VM):</br>
  ![image](https://user-images.githubusercontent.com/80945113/112334950-805d2a00-8cc4-11eb-985f-eb2b7e219050.png)

### 8(create own vagrant box):
  ![image](https://user-images.githubusercontent.com/80945113/112335060-97038100-8cc4-11eb-890b-a13802161405.png)

Thanks for attention!
  
