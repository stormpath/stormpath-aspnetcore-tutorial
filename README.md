# Build an ASP.NET Core Application With User Authentication
Original post: (link)

## Try it out

1. If you haven't registered for Stormpath, [create a free developer account](https://api.stormpath.com/register).
2. Log in to the [Admin Console](https://api.stormpath.com/) and use the Developer Tools section on the right side of the page to create and download an API key file.
3. Open the `apiKey.properties` file up in Notepad (or your favorite editor). Using the command line (or PowerShell), execute these commands:

 ```
 setx STORMPATH_CLIENT_APIKEY_ID "[value from properties file]"
 setx STORMPATH_CLIENT_APIKEY_SECRET "[value from properties file]"
 ```
 
4. Back in the Stormpath Admin Console, navigate to **Applications** and find the default application that's created for you when you sign up for Stormpath (called "My Application"). Select it and copy the **Href** value (it'll look like ``https://api.stormpath.com/v1/applications/l0ngR4nd0mStringH3r3``).
5. Save the Application URL as another environment variable:

 ```
 setx STORMPATH_APPLICATION_HREF "[your Application href]"
 ```
 
6. Clone this repo!

 ```
 git clone https://github.com/stormpath/stormpath-aspnetcore-tutorial.git
 ```

7. Open `StormpathAspNetCoreTutorial.sln`. Compile and run!
