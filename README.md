# Udagram Image Filtering Microservice

Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

It is a Node-Express application deployed to AWS Elastic Beanstalk which runs a simple script to process images.

**Link to the endpoint URL for a running elastic beanstalk deployment** - http://image-filter-02012023-dev.us-east-1.elasticbeanstalk.com/

**Tested with** - http://image-filter-02012023-dev.us-east-1.elasticbeanstalk.com/filteredimage?image_url=https://www.akc.org/wp-content/uploads/2017/11/Shih-Tzu-On-White-01.jpg


## Tasks

### Setup Node Environment

1. Initialized a new project with `npm i`
2. run the development server with `npm run dev`
3. Built and compile the application with `npm run build`

### Created a new endpoint in the ./src/server.ts file

The endpoint uses query parameter to download an image from a public URL, filter the image, and return the result.
- tested the endpoint using postman

![Screenshot (422)](https://user-images.githubusercontent.com/58152694/216231461-47586851-717d-434a-a1c2-9f1f2ed12741.png)
  
### Deployed the system using AWS Elastic Beanstalk

After creating an IAM user role with user group policies:
- `eb init` was used to initialize a new application
- `eb create` was used to create a new elastic beanstalk environment to deploy the image-filter service and
![Screenshot (421)](https://user-images.githubusercontent.com/58152694/216231484-f9af11fe-3039-433c-8b06-579c478e858d.png)



### Elastic Beanstalk application dashboard

![eb dash1a](https://user-images.githubusercontent.com/58152694/216232088-ad628318-e52d-490e-8d3f-a48a28be9b10.png)
![eb dash1b](https://user-images.githubusercontent.com/58152694/216232075-01a84143-b1c9-4c07-8f7c-9e875e6b03ba.png)


