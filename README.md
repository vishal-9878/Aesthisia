Hi I have completed assignment assigned by Aesthisia 
	Below are steps to create the given setup:-
1. Pulled github repository provided by the organisation.
2. Created a Dockerfile.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Create app directory
WORKDIR /usr/src/app
#Copying json packages
COPY aesthisia-demo/package.json ./
#Copying app sources
COPY aesthisia-demo/src/* ./
# Installing and Running npm
RUN npm install
COPY aesthisia-demo ./
RUN npm run

EXPOSE 3000
CMD npm start
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
3. Built Dockerfile to create a Docker Image.
4. Ran a Docker Container.
5. Hit on the repective port.



 						THANKS
