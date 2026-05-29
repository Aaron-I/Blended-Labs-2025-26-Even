# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**: Aaron I
* **Register Number**: 212223230002
* **Date of Submission**: 12/05/2026

---

## Objective

The objective of this experiment is to understand how Amazon Elastic Block Store (EBS) provides persistent block-level storage for EC2 instances. This lab focuses on creating and attaching an EBS volume, formatting and mounting it on an EC2 instance, storing data, and verifying data persistence after instance reboot.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing EC2 instance (Amazon Linux 2 preferred)
* Basic knowledge of Linux commands

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Amazon EBS
* SSH Client (Terminal / PuTTY)

---

## Tasks Performed

### Task 1: Explore Amazon EBS

Explore the Amazon EBS service through the EC2 dashboard. Observe different volume types such as General Purpose SSD (gp2/gp3), Provisioned IOPS SSD, Throughput Optimized HDD, and Cold HDD.

---

### Task 2: Create an EBS Volume

Create a new EBS volume in the same Availability Zone as the EC2 instance. Choose an appropriate size and volume type.

---

### Task 3: Attach EBS Volume to EC2 Instance

Attach the created EBS volume to the running EC2 instance as an additional block device.

---

### Task 4: Format the EBS Volume

Connect to the EC2 instance using SSH and format the attached volume with a file system (for example, ext4).

---

### Task 5: Mount the EBS Volume

Mount the formatted volume to a directory in the EC2 instance (for example, /data or /mnt/ebs).

---

### Task 6: Store Data in EBS Volume

Create files and directories inside the mounted EBS volume and store sample data.

---

### Task 7: Verify Data Persistence

Reboot the EC2 instance and verify that the data stored in the EBS volume is still available after reboot.

---

## Workflow (Student Explanation)


1. Logged in to the AWS Management Console and explored the Amazon EBS service through the EC2 dashboard to understand different volume types and storage options.
2. Created a new EBS volume of the required size in the same Availability Zone as the running EC2 instance and verified that the volume was available.
3. Attached the EBS volume to the EC2 instance as an additional storage device and connected to the instance using SSH.
4. Identified the attached block device, formatted it with the ext4 file system, created a mount directory, and mounted the volume to the instance.
5. Created sample files and directories in the mounted volume, rebooted the EC2 instance, remounted the volume if necessary, and verified that all stored data remained available, confirming data persistence.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="1911" height="971" alt="Screenshot 2026-05-29 210824" src="https://github.com/user-attachments/assets/26ea254d-abe3-477d-8b17-ef999c436693" />


---

### Screenshot 2: EBS Volume Attached to EC2

<img width="1918" height="959" alt="image" src="https://github.com/user-attachments/assets/0a2f4955-67be-4b01-841a-0e7e7d41c784" />


---

### Screenshot 3: Mounted Volume with Data

<img width="1911" height="964" alt="Screenshot 2026-05-29 212002" src="https://github.com/user-attachments/assets/2373e2fd-f37f-4b2d-8726-75b04c9e9a3d" />


---

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
