Here we are going to create our first VPC along with 2 subnets (public and private) and an internet gateway.

1. Go to AWS console and search for VPC and click on it.
   ![](../assets/search.png)

3. Click on `Create VPC` button and configure it as follows:
   ![](../assets/create-vpc.png)

   Above We configured the VPC to have the following properties:
    - Resources to create: `VPC Only`
    - Name: `my-vpc`
    - IPv4 CIDR block: `manual` and entered `10.1.0.0.16` <br/>
    (which is our IP address range for our VPC.)

5. Then click on `Create VPC` button and wait for it to be created.

6. Now we have our VPC created, let's create our first subnet.

   ![](../assets/subnet1.png)

7. Select the AZ same as your VPC.
   ![](../assets/subnet2.png)

8. Configure 2 subnets as follows:
   ![](../assets/subnet3.png)
    Name: `public` <br/>
    IPv4 CIDR block: `10.1.1.0/24` <br/>
    Availability Zone: Same as your VPC <br/>

    Name: `private` <br/>
    IPv4 CIDR block: `10.1.2.0/24` <br/>
    Availability Zone: Same as your VPC <br/>

9. Click on `Create Subnet` button and wait for it to be created.
   ![](../assets/subnet4.png)

10. Tada! We have our first VPC and subnets created.
   ![](../assets/subnet5.png)

11. Now we need to create an internet gateway.
   ![](../assets/ig1.png)

12. Click on `Create Internet Gateway` button and name it.
   ![](../assets/ig2.png)

13. Go to actions and click on `Attach to VPC` and select your VPC.
    ![](../assets/ig3.png)

14. Choose your VPC and click on `Attach Internet Gateway` button.
    ![](../assets/ig4.png)

That's it! Hope you enjoyed this guide and successfully created your first VPC and subnets along with an internet gateway.
