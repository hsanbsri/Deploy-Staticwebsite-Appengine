# Deploy-Staticwebsite-Appengine
Deploy Static Website With App Engine In Google Cloud

### Proyek Deploy Aplikasi Profile


```bash
Here For The First Step
git clone #git link
```

```sh
-> Open Cloud Shell -> Open Editor -> Create Folder www -> Paste All Assets For Website In www also index.html -> Create File app.yaml in your root folder except www 

# Copy and Paste Code Below for app.yaml 
runtime: python27
api_version: 1
threadsafe: true

handlers:
- url: /
  static_files: www/index.html
  upload: www/index.html

- url: /(.*)
  static_files: www/\1
  upload: www/(.*)
  
```

```sh
-> Klik Terminal -> gcloud app deploy -> gcloud app browse -> Click link display in terminal -> Done 
```
