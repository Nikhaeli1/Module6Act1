Lab Manual 1: Introduction to Docker Containerization

Name: Bradley Sheen Sale
Section: IT3R2

Guide Questions:
1. 	What role does the Dockerfile play in containerization?
A Dockerfile serves as the foundational blueprint for containerization by acting as a plain text recipe for your application. Instead of requiring you to manually configure a server, it uses a sequential list of instructions to automatically assemble the environment, defining everything from the base operating system to the necessary dependencies and the exact command needed to run the application upon startup. 

2. 	Why are Docker containers lighter than virtual machines?
The reason Docker containers are significantly lighter than virtual machines lies in how they interact with the operating system. Virtual machines rely on a hypervisor to boot an entire, isolated guest operating system for every single application, which consumes massive amounts of RAM, CPU, and storage. In contrast, containers bypass this heavy overhead by sharing the host machine's operating system kernel. They only package the application code alongside its specific required binaries and libraries, allowing them to remain incredibly small and start up in mere milliseconds. 
3. 	What happens when the container finishes execution?

When a container finishes its execution, its lifecycle is directly dictated by the primary process running inside it. Once that main task is complete—such as a Python script finishing its final line of code—the container immediately stops running and enters an exited state. While in this dormant state, it consumes absolutely zero active memory or CPU power, but it does not automatically delete itself from your system. The container and its internal file system remain saved on your hard drive so you can review its logs or restart it until you intentionally remove it. 



App.py

<img width="583" height="311" alt="image" src="https://github.com/user-attachments/assets/47b831fd-ce31-4dad-850e-0800606e8dc9" />



Dockerfile

<img width="537" height="293" alt="image" src="https://github.com/user-attachments/assets/96e93696-8fc2-4920-a697-53f1a0c4a404" />



Output

<img width="591" height="334" alt="image" src="https://github.com/user-attachments/assets/ce04bd0e-e0c2-43f9-86a7-4eef958d366d" />



Cleaning

<img width="572" height="158" alt="image" src="https://github.com/user-attachments/assets/e12678af-3fd5-4fd9-af35-e52a3f2aa8d8" />
