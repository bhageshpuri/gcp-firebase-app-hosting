# gcp-firebase-app-hosting
gcp-firebase-app-hosting

![image](https://github.com/user-attachments/assets/9c2b39c4-5b8d-45f0-bfc9-5cc5f3c9bc3e)

![image](https://github.com/user-attachments/assets/f5316fad-db36-4bd0-b014-770db0cde7f6)

Either choose an existing project or create a new project:

![image](https://github.com/user-attachments/assets/9b72aa22-d5d4-4c20-a2f6-50807f25f852)

![image](https://github.com/user-attachments/assets/d128a0c8-702b-4cf4-a48f-663d5c75d282)

![image](https://github.com/user-attachments/assets/9786c4c4-669a-436d-91fa-69ee04850142)

![image](https://github.com/user-attachments/assets/96e6dcd0-3fa1-4b75-998e-c286d4d3e02e)

![image](https://github.com/user-attachments/assets/5bdf17ca-e7f5-43f3-9e3c-a1b026fde642)


To use the free Spark Plan the GCP project should not have billing enabled.

Once you enable the free plan later to use other GCP services you can enable billing and still stay on the free plan.

Code to deploy using terraform:

https://firebase.google.com/docs/projects/terraform/get-started 

https://firebase.google.com/codelabs/firebase-terraform#0

While creating a new project for Firebase, label the project:
labels = { "firebase" = "enabled" }

Enable services/APIs: 
cloudbilling.googleapis.com cloudresourcemanager.googleapis.com serviceusage.googleapis.com firebase.googleapis.com

Firebase Authentication

Option 1 (Recommended): Set up Firebase Authentication in the console, which doesn't require GCIP. 
• Using this option means that you do not have to associate your new project with a Cloud Billing account.

Option 2: Set up Firebase Authentication via Terraform using Google Cloud Identity Platform (GCIP) APIs. 
• Using this option means that you have to associate your new project with a Cloud Billing account since GCIP requires the project to be on the Blaze pricing plan.

