# gcp-firebase-app-hosting
gcp-firebase-app-hosting

![image](https://github.com/user-attachments/assets/9c2b39c4-5b8d-45f0-bfc9-5cc5f3c9bc3e)

![image](https://github.com/user-attachments/assets/f5316fad-db36-4bd0-b014-770db0cde7f6)

Either choose an existing project or create a new project:

![image](https://github.com/user-attachments/assets/9b72aa22-d5d4-4c20-a2f6-50807f25f852)

![image](https://github.com/user-attachments/assets/d128a0c8-702b-4cf4-a48f-663d5c75d282)

![image](https://github.com/user-attachments/assets/9786c4c4-669a-436d-91fa-69ee04850142)

![image](https://github.com/user-attachments/assets/96e6dcd0-3fa1-4b75-998e-c286d4d3e02e)

To use the free Spark Plan the GCP project should not have billing enabled.

Code to deploy using terraform:

https://firebase.google.com/codelabs/firebase-terraform#0

While creating a new project for Firebase, label the project:

...

# Create a new Google Cloud project.
resource "google_project" "default" {
  provider = google-beta.no_user_project_override

  name            = "<PROJECT_NAME_OF_YOUR_PROJECT>"
  project_id      = "<PROJECT_ID_OF_YOUR_PROJECT>"

  # Required for the project to display in any list of Firebase projects.
  labels = {
   ** "firebase" = "enabled"**
  }
}
