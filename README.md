# GoogleAI-Chatbot
Sample code for GoogleAI-Chatbot.

*How to set up your local environment for connecting Google Vertex AI account*.

*The basic model and its loading*.

Streamlit framework.
##Vertex AI setup 
Install Google Cloud CLI on Windows​

https://cloud.google.com/sdk/docs/install-sdk#windows​
Run below command in power shell:​
gcloud auth application-default login​
gcloud auth application-default set-quota-project  {project_id}

In your program import the following 
   <
   ** import os
    **GOOGLE_APPLICATION_CREDENTIALS** = "C:\\Users\\XXXXX\\AppData\\Roaming\\gcloud\\application_default_credentials.json"
    if not os.path.exists(GOOGLE_APPLICATION_CREDENTIALS):
         print("Warning: The KEY file (JSON) cannot be found. ")
    os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = GOOGLE_APPLICATION_CREDENTIALS
    PROJECT_ID = "<**XXXXX-sandbox**>"  # @param {type:"string"}
    vertexai.init(project=PROJECT_ID, location="us-central1")**
   >
