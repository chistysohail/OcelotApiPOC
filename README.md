# OcelotApiPOC

Imagine you're running a big hotel with several services like a restaurant, gym, and spa. Each service is managed by a different team and located in various parts of the hotel. Now, your guests need an easy way to access these services without having to know where each one is or how they operate. This is where you, as the hotel manager, step in and provide a central information desk. Guests come to you with their requests, and you guide them to the right service, ensuring they have a smooth experience.

In this analogy, your hotel represents a software application made up of many small services (like the restaurant, gym, spa, etc.). These small services are what we call "microservices" in the tech world. They work together to make the whole application function. However, just like guests in a hotel, users of your application need a simple way to access these microservices without worrying about their complexities.

Here's where Ocelot comes into play, acting as the hotel's information desk in our analogy. Ocelot is a tool used in .NET 6 applications (a popular software development framework) to manage access to microservices. When a user wants to perform an action (like booking a spa appointment), they send a request to Ocelot. Ocelot then figures out which microservice (spa, in this case) can handle the request and forwards it accordingly. It can also combine responses from different services (say, if you wanted a package deal that includes both gym and spa) and send them back to the user as one.

So, in layman's terms, Ocelot helps manage and simplify how requests from users are sent to and received from the various microservices in an application, making the whole system work smoothly together, just like a well-run hotel.


Technicaly:
Ocelot API Gateway Project
This project demonstrates how to set up a simple API Gateway using Ocelot in a .NET 6 application. The gateway routes incoming HTTP requests to various backend services based on the configuration defined in ocelot.json.

Getting Started
These instructions will get your copy of the project up and running on your local machine for development and testing purposes.

Prerequisites
.NET 6 SDK
Visual Studio 2019 or later with the ASP.NET and web development workload installed

cd yourproject
Restore NuGet packages


dotnet restore
Build the project


dotnet build

Running the application
Using Visual Studio

Open the solution file in Visual Studio.
Press F5 or click on the "Start" button to run the application.
Using the Command Line


dotnet run
The application will start on http://localhost:5000 and https://localhost:5001 by default unless configured otherwise.

Configuration
The API Gateway's routing configuration is defined in the ocelot.json file. Modify this file to set up routing rules for your backend services.

Testing
To test the API Gateway, send HTTP requests to the paths defined in ocelot.json using a tool like Postman or curl. The gateway will forward your requests to the corresponding backend services.

Built With
.NET 6 - The framework used
Ocelot - API Gateway
Contributing
Please read CONTRIBUTING.md for details on our code of conduct, and the process for submitting pull requests to us.

Versioning
We use SemVer for versioning. For the versions available, see the tags on this repository.

Authors
Your Name - Initial work - YourProfile
See also the list of contributors who participated in this project.

License
This project is licensed under the MIT License - see the LICENSE.md file for details.

Acknowledgments
Hat tip to anyone whose code was used
Inspiration
etc
