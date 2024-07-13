# Simple Notes App
This is a simple notes app built with React and Django.
Simply works to note some impt tasks or feedback to work on, however to deploy this application here we implement simple methodology of dockerizing the application to maintain system complexities and using reverse proxy or port forwarding serve the application via Nginx server. 


## Requirements
1. Python 3.9
2. Node.js
3. React

## Installation
1. Clone the repository
```
git clone https://github.com/LondheShubham153/django-notes-app.git
```

2. Build the app
```
docker build -t notes-app .
```

3. Run the app
```
docker run -d -p 8000:8000 notes-app:latest
```

## Nginx

Install Nginx reverse proxy to make this application available

`sudo apt-get update`
`sudo apt install nginx`

Open the nginx sites-enabled directory then in default file change the location using proxy_pass of python app Ip which needs to be access via instance id only instead of directly host id.

### At last the deployment is over and the webpage will be shown below:
![Screenshot 2024-07-13 153627](https://github.com/user-attachments/assets/89c4d382-f22d-461b-91ff-6246ba4b3554)

