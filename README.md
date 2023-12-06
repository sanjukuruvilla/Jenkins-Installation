# Jenkins-Installation
Jenkins-installation-easy-step

Installing Jenkins on Ubuntu

create an instance in AWS

![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/b04202c6-e84e-41f1-afff-a9b420b1e5f2)

update your instance:
sudo apt-get update

install java: 
sudo apt install openjdk-11-jre

Check Java version:
java --version

![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/5c1c79ff-ca0f-40dd-9f8a-8267e14abf23)

Installing Jenkins:

Step 1: Goto Jenkins official website:
        
- https://www.jenkins.io/doc/book/installing/

Step 2: Choose Linux:
       
![chooselinux](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/d3afcbf8-d429-4689-b7a1-36568529f993)

Step 3: Choose Debian/Ubuntu:
        
![choseubuntu](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/7bbe1f9a-508c-42c7-8270-53fb5e16a0b6)
        
Step 4: Copy the script and paste it on your EC2 terminal:

![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/fe405bff-c2c4-44e1-8a24-ddfd88202dc7)
        
Step 5: Check Jenkins version:

![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/389438e7-8688-40c4-a9a0-e3b004e45d42)
        
Step 6: Allow port 8080 for Jenkins in security group under inbound rules, 

- choose My IP, if you dont want it to expose to all others on Internet
- Choose Anywhere IPv4 if you want anyone to access Jenkins on Internet
        
![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/7a65838c-a99b-4466-a8c1-4c31417e87bf)

Step 7: Start the Jenkins by using the commands below in linux terminal

- sudo systemctl start jenkins.service  // Starts the Jenkins service
- sudo systemctl enable jenkins.service // Prevents Jenkins to stop whenever te instance reboot.
- sudo systemctl status jenkins.service // Check the status of Jenkins service
        
![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/75ec1718-92fb-4a34-af3c-4e483acc44c8)
        
Step 8: Jenkins will be running on port 8080 of your EC2 IP address, open in a web browser

Step 9: Go to your terminal

- sudo cat /var/lib/jenkins/secrets/initialadminpassword
       
![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/1f6bb140-3824-45e0-9160-254cec2437b9)

copy the password and update
        
Step 10: Install the suggested plugins:

![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/91a442e8-2c94-4ff1-b3ed-1f4a8cdfd506)

![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/c77e61ad-6f9a-4bd0-a2ad-34beea24e780)

![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/30ea87fd-0132-45d8-a1a8-5fc72b55491c)
        
Step 11: Update the Details

![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/2bf29f9d-485b-4936-a909-36c55fc2e752)

You have reached the Dashboard page of Jenkins.

![image](https://github.com/sanjukuruvilla/Jenkins-Installation/assets/57086804/ae1f0987-78fd-422c-865b-0869e7edab36)

Now you can start building the pipepline. 
Stay safe and Keep Coding ...




