# How to set up an Amazon Web Services computer (a virtual "instance"):

This page shows you how to create a new "AWS instance", or a running computer
In a web browser, navigate to https://aws.amazon.com/ and log in using your credentials

image:

0. Under "Compute", select EC2

![alt text](~/Desktop/make_aws_instance/aws_images/step0.png)

1. Switch to zone US West (N California)

![alt text](~/Desktop/make_aws_instance/aws_images/step1.png)

2. Click on "Launch Instance"

![alt text](~/Desktop/make_aws_instance/aws_images/step2.png)

3. On the left side of the next page, select "Community AMIs"

![alt text](~/Desktop/make_aws_instance/aws_images/step3.png)

4. Search for ami-c72d7fa7 (2017-01-20-ubuntu-wily-titus-ucdavis-dragon)

5. Click on "select"

![alt text](~/Desktop/make_aws_instance/aws_images/step5.png)

6. Choose t2.micro

![alt text](~/Desktop/make_aws_instance/aws_images/step6.png)

7. Near the top, click "6. Configure Security Group"

![alt text](~/Desktop/make_aws_instance/aws_images/step7.png)

8. Click "Add Rule"

![alt text](~/Desktop/make_aws_instance/aws_images/step8.png)

9. Change the Port Range from 0 to 8000

![alt text](~/Desktop/make_aws_instance/aws_images/step9.png)

10. Click Review and Launch

![alt text](~/Desktop/make_aws_instance/aws_images/step10.png)

11. Click "Launch"

![alt text](~/Desktop/make_aws_instance/aws_images/step11.png)

12. Under the drop down menu, select "Proceed without a key pair" and check the box

![alt text](~/Desktop/make_aws_instance/aws_images/step12.png)

13. Click "Launch Instances"

![alt text](~/Desktop/make_aws_instance/aws_images/step13.png)

14. Click "View Instances"

![alt text](~/Desktop/make_aws_instance/aws_images/step14.png)

15. Copy the IPv4 public IP into a new browser tab and add ":8000" to the end.

![alt text](~/Desktop/make_aws_instance/aws_images/step15.png)

16. You should see a page like this:

![alt text](~/Desktop/make_aws_instance/aws_images/step16.png)

17. Enter the password (note, it will always be city in which UCD is located. No caps.)

18. Click "New", and select "Terminal" from the drop down menu

![alt text](~/Desktop/make_aws_instance/aws_images/step18.png)

19. Type "bash" into the terminal window-looking thing in the new tab. Hit Enter

![alt text](~/Desktop/make_aws_instance/aws_images/step19.png)

20. Do all of the things in your shiny new Linux-based environment

![alt text](~/Desktop/make_aws_instance/aws_images/step20.png)

21. When you're done, terminate the instance.

In the EC2 management console, select the instance, then click Actions and select
Terminate from the drop down menu. When prompted, click "Yes, Terminate"

![alt text](~/Desktop/make_aws_instance/aws_images/step21.png)