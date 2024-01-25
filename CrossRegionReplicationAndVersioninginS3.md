1. Create a Source bucket
![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/3ad09f7a-5938-4d54-9877-35ea0a039fc5)

2. Object ownership: Select ACLs disabled (recommended) option

![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/806afca9-0e9a-411b-a610-0eef56138153)

3. In the option of Bucket settings for Block Public Access, Uncheck the option of Block all public access. And, Acknowledge the same by checking the below option

![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/af8bacc5-102f-411a-8f29-872c82de4fc5)

4. Bucket Versioning Enabled

![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/358a8587-fc01-4826-aefa-f575b225d300)



Target Bucket

![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/66658756-a817-41d2-86d4-b58326f4d28c)



Enable Versioning

Go to Source Bucket and click on Management. Scroll down and select Create replication rule button. 

![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/85f0c5ab-1b4f-45a9-9749-25bc4a6abfb3)


![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/11e6fb14-99bb-4232-a6fa-a7a4d4781782)

Choose a rule scope : Select Apply to all objects in the bucket

![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/6e345aff-f6eb-4bf9-8c54-f61783644618)

Under Destination, select choose a bucket in this account and click on Browse S3. 

![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/ca4156cd-c6bf-4693-9c2e-7874fd4da60f)

Under IAM Role, Select Choose from existing IAM roles and select Create new role

![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/b68902dc-2155-4e15-87a7-86ce7aa09598)

Under the Destination Storage Class, select Change the storage class for the replicated objects and choose One Zone-IA.

![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/49afebdf-a2d5-4f59-aca8-f928040981bd)

 Leave everything as default. Review once and click on Save button. One Pop-up appears Select No, do not replicate existing objects and Click on Submit button.

 ![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/c449f3dd-66b8-437b-8acd-ab367194441e)

 Now navigate to the source bucket and upload an Object(.txt or .png) in the Source bucket by clicking on Add Files. Click on Upload.

 ![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/7205a457-7f11-4bf3-b0c0-bdd439b98d02)


 Navigate to your Target Bucket to see the replication. It may take up to 3-5 minutes for replication.
 
 ![image](https://github.com/Asma09Akram/Cross-Region-Replication-and-Versioning-in-S3/assets/124654068/03ddf275-e997-4627-8d97-336f148a7397)

