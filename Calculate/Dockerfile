FROM openjdk:11 
 
RUN apt-get update && apt-get install -y \ 
    xauth \ 
    x11-apps \ 
    libxtst6  
 
ENV DISPLAY=:0 
 
COPY calc.jar /app/ 
 
WORKDIR /app 
 
CMD ["java", "-jar", "calc.jar"]