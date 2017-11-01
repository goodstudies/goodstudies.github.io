# goodstudies.github.io
This is a simple web app to demonstrate **Progressive Web Apps** and **UWP Hosted Web Apps by Manifoldjs**.


##PWA App
Link : [https://goodstudies.github.io/PWACurrencyConverter/](https://goodstudies.github.io/PWACurrencyConverter/)

This link is simple example for **Progressive Web App (PWA)** to convert the currency rates between various counties.
Key components of this PWA is ServiceWorker, Promise and localStorage.
It will cache the html and needed files locally and store the latest retrieved currency values in localStorage. So it will work offline.
If you are using Chrome you can add this link to Desktop or Home screen (in Andriod mobile) to work link standalone app.


##Hosted Web Apps by Manifoldjs
Link : [https://goodstudies.github.io/PWACurrencyConverterHostedWebApp/](https://goodstudies.github.io/PWACurrencyConverterHostedWebApp/)

In this app we have added some JavaScript methods to interact and use Windows 10 features like Toast and Tiles in start screen. 
So these features are accessable only Windows 10 store apps created by Manifoldjs and will ignore those methods in remaining platforms.

Following are the steps to create Hosted Web Apps by Manifoldjs CLI tool from command prompt.

Step 1 : Open the Command prompt
Step 2 : Install Manifoldjs by npm **npm install -g manifoldjs**
Step 3 : Type the following commands to create project 
         ```sh manifoldjs https://goodstudies.github.io/PWACurrencyConverterHostedWebApp/ -d D:\UWP\ -l debug -p windows10```
Step 4 : Now open the "D:\UWP\PWACC\windows10\source\App.csproj" in Visual Studio 2017
Step 5 : To access Windows 10 features need to give full access to WinRT rules. 
         Open and make change: **package.appxmanifest** -> Content URIs -> WinRT Access -> All 