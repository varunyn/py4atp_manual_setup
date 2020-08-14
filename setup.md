## Step 1: Create Compartment

1.  Click on left hamburger menu -> Identity -> Compartments

<img src="./images/step1/1.png" alt="Screen_Shot_2020-08-13_at_6.58.44_PM" style="zoom:80%;" />

2. Click on **Create Compartment**

![Screen_Shot_2020-08-13_at_6.59.43_PM](./images/step1/2.png)

3. Give Name and Description and click on **Create Compartment**.

![Screen_Shot_2020-08-13_at_7.00.26_PM](./images/step6/3.png)

## Step 2: Create Instance 

1. Click on left hamburger menu -> Compute -> Instances

![](./images/step2/1.png)

2. Click on **Create Instance** and make sure you are in right compartment.

![](./images/step2/2.png)

3. Give name and click on **Change Image**

![Screen_Shot_2020-08-13_at_8.57.40_PM](./images/step2/3.png)

4. Click on **Oracle Images** tab.

![Screen_Shot_2020-08-13_at_7.02.48_PM](./images/step2/4.png)

5. Select **Oracle Cloud Developer Image**, check the terms and click on **Select Image**

![Screen_Shot_2020-08-13_at_7.02.48_PM](./images/step2/5.png)

![Screen_Shot_2020-08-13_at_7.03.06_PM](./images/step2/6.png)

6. Download the auto-generated keys or you can use your own keys. After filling all the details it should look something like following image. Click on **Create**

![](./images/step2/7.png)

## Step 3: SSH into instance and setup VNC

1. SSH into instance with command 

   `ssh -i <path_to_private_key> opc@<public_ip_address>`

2. After ssh type `vncpasswd` enter password and press `n` when asked for view-only password.

![Screen_Shot_2020-08-13_at_7.13.05_PM](./images/step3/1.png)

3. Type `vncserver` and it should return output similar to following image.

<img src="./images/step3/2.png" alt="Screen_Shot_2020-08-13_at_9.06.31_PM" style="zoom:67%;" />

## Step 4: Accessing a Graphical User Interface (GUI) via VNC

To access a GUI via VNC, do the following:

1. On your local computer, connect to your instance and create an ssh tunnel for port 5901 (for display number 1): `$ ssh -L 5901:localhost:5901 –i id_rsa opc@<IP Address>`

2. On your local computer, start a VNC viewer and establish a VNC connection to` localhost:1`

3. Enter the VNC password you set earlier

## Step 5: Create Autonomous Database

1. Click on left hamburger menu -> Autonomous Transaction Processing

<img src="/images/step5/1.png" alt="Screen_Shot_2020-08-13_at_9.13.09_PM" style="zoom:50%;" />

2. Makes sure you are in right compartment and click on **Create Autonomous Database**

![Screen_Shot_2020-08-13_at_9.31.37_PM](/images/step5/2.png)

3. Enter Display name and Database name and scroll down

![Screen_Shot_2020-08-13_at_9.32.38_PM](/images/step5/3.png)

4. Enter Password and confirm password

![Screen_Shot_2020-08-13_at_9.33.31_PM](/images/step5/4.png)

5. After filling all the details, it should look something like following image. Click on **Create Autonomous Database**

![](/images/step5/5.png)

## Step 6: Create Object Storage

1. Click on left hamburger menu -> Object Storage -> Object Storage

![1](./images/step6/1.png)

2. Make sure you are in right compartment and click on **Create Bucket**

![2](./images/step6/2.png)

3. Enter Bucket name and click on **Create Bucket**

![3](./images/step6/3.png)

