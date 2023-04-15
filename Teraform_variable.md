install terrafom if using new system /ec2 instance

crate file mkdir variable

![image](https://user-images.githubusercontent.com/85178565/232247233-1df0c423-2fc0-4d25-9831-487e706a8eac.png)

main.tf file

![image](https://user-images.githubusercontent.com/85178565/232247282-c05aee72-86bb-4a36-9c69-b3b824199fad.png)


![image](https://user-images.githubusercontent.com/85178565/232247323-b4519d70-cd5a-486f-b98b-55647713ba1a.png)

created a file called variable.tf & call this file in main.tf file

![image](https://user-images.githubusercontent.com/85178565/232247407-aa3571cb-c87b-4586-b6e7-ddcfa415ab6e.png)

vim variable.tf

![image](https://user-images.githubusercontent.com/85178565/232247482-c76f7572-5868-4d23-8ee3-08453bd7892c.png)

calling in main.tf

![image](https://user-images.githubusercontent.com/85178565/232247551-39c748f7-1e9b-46ce-a547-ee6b85dcd093.png)


terraform plan

![image](https://user-images.githubusercontent.com/85178565/232247763-588c5343-0a33-4c9f-8b66-523233f7b768.png)


terraform apply

![image](https://user-images.githubusercontent.com/85178565/232247857-4e860370-9f06-43c7-a8d2-51bd1ecd058e.png)

devops-autoated file generated

![image](https://user-images.githubusercontent.com/85178565/232247937-cdb1999d-62e1-4791-83f8-89a1a6865e2c.png)



adding values to a variable in a different way--keep variable empty & in globally give value

![image](https://user-images.githubusercontent.com/85178565/232248744-a2f5c26c-601b-446b-ab4d-bf88c173fb43.png)

![image](https://user-images.githubusercontent.com/85178565/232248943-b3c2ab06-8dbb-4723-b2fd-c999ebf44c66.png)


in main.tf file create output variable to call variables and then terraform apply

![image](https://user-images.githubusercontent.com/85178565/232249171-e2f72099-753e-4080-bd9c-ac2a71f1db45.png)


you can change variable value with out entering into file &change value you can change through export TF_VAR_<VARIABLE>=<VALUE>
  
  
  ![image](https://user-images.githubusercontent.com/85178565/232249589-621fdd5f-a4e7-4d4d-b8f5-f661f5a07cd5.png)




