## Google App Engine
<p>Google App Engine is a cloud computing platform as a service(pas) for developing and hosting web applications in Google-managed data centers. Applications are sandboxed and run across multiple servers. App Engine offers automatic scaling for web applications—as the number of requests increases for an application, App Engine automatically allocates more resources for the web application to handle the additional demand.

# How to Deploy a web App On Google App Engine

Step 1. Create a new project on Google cloud Console

Step 2. From the APIs & Services menu Enable Google App Engine Admin API
![Enable Api](./images/HArVguiohtDtUhiPIWzqNnBfeRlqtNk7dDsZ_6EO13E%3D.png)
![Enable Api](./images/7KsbdDhKec_NXvMTPi7NP0r3ML4Cu7ST4RZjEpaCuYE%3D.png)


Step 3. Clone this Repo:

```
    git clone https://github.com/medendale/Google-App-Engine.git
```
Step 4. From within The app  directory where the app's app.yaml configuration file is located, start the Google Cloud development server with the following command
```
dev_appserver.py app.yaml
```
View the results by clicking the Web preview > Preview on port 8080.
![Test](./images/znqxKObHIzucdgmme4nJP485ReBUAMdG%2BOKJP9XLzes%3D.png)

Step 5. To deploy your app to App Engine, run the following command from within the root directory of your application where the app.yaml file is located:

```
    gcloud app deploy
```

## The Setup Process 

1. Install [`pip` and `virtualenv`][cloud_python_setup] if you do not already have them.

1. Clone this repository:

```
    git clone https://github.com/medendale/Google-App-Engine.git
```

1. Obtain authentication credentials.

    Create local credentials by running the following command and following the
    oauth2 flow (read more about the command [here][auth_command]):

    ```
    gcloud auth application-default login
    ```

    Read more about [Google Cloud Platform Authentication][gcp_auth].
