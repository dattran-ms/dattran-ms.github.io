---
layout: post
title:  "Azure Logic Apps"
author: Dat Tran
categories: [ Azure ]
tags: [Azure Basic]
image: assets/images/az-basic-logic-app/azure-logic-app-title.png
beforetoc: "Azure Logic Apps is a cloud service that helps you schedule, automate, and orchestrate tasks, business processes, and workflows when you need to integrate apps, data, systems, and services across enterprises or organizations."
toc: true
---
Azure Logic Apps are Enterprise Integration Service, which means their main purpose is orchestration, integration and scheduling of tasks in a simple way. With easy to use user interface, no coding design and powerful extensibility you can easily integrate services in minutes.

In this video I will cover basics of Logic Apps and show couple of demos.
![all-trigger]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-1.png)

<br>
## Web Trigger
![web-trigger1]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-1.png)
1. Create new Logic App service
![web-trigger2]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-2.png)
2. Full fill required information
![web-trigger3]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-3.png)
3. Access Logic App Designer and create new Blank Logic App
![web-trigger4]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-4.png)
4. Create the Request
![web-trigger5]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-5.png)
![web-trigger6]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-6.png)
5. Edit the Request
+ Choose GET method
![web-trigger7]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-7.png)
6. Create the Response
![web-trigger8]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-8.png)
![web-trigger9]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-9.png)
7. Edit the Response
![web-trigger10]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-10.png)
8. Save and Get the HTTP URL
![web-trigger11]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-11.png)
![web-trigger12]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-12.png)
9. Pass HTTP URL on browser and verify
![web-trigger13]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-13.png)
![web-trigger14]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-14.png)
10. Check Runs history
![web-trigger15]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-15.png)
11. Run HTTP Request with "Relative path"
![web-trigger16]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-16.png)
12. Edit HTTP Response to utilize the relative path parameter
![web-trigger17]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-17.png)
![web-trigger18]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-18.png)
13. Save and test verify
+ Save
![web-trigger19]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-19.png)
+ Replace {name} as "Adam"
![web-trigger20]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-20.png)
![web-trigger21]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-21.png)

<br>
## Web Trigger and create new blob in Storage Account
![web2-trigger1]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-22.png)
1. Create new Storage Account service
![web2-trigger2]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-23.png)
2. In new Storage account, access "Blobs" and create new "Container"
![web2-trigger3]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-24.png)
![web2-trigger4]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-25.png)
![web2-trigger5]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-26.png)
3. Access "a4e-logic-app-demo-http" and insert a new step
![web2-trigger6]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-27.png)
4. Choose "Storage Account" action
![web2-trigger7]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-28.png)
![web2-trigger8]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-29.png)
![web2-trigger9]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-30.png)
5. Full fill required informations
![web2-trigger10]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-31.png)
6. Test and verify
+ Refresh browser and check Login App run history
![web2-trigger11]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-32.png)
![web2-trigger12]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-33.png)
+ Access Storage Account to check new blog is created
![web2-trigger13]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-34.png)

<br>
## Blob Storage Trigger
![blob-trigger1]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-35.png)
1. Create new "Logic App"
![blob-trigger2]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-36.png)
2. Choose "Azure Blob Storage" trigger
![blob-trigger3]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-37.png)
![blob-trigger4]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-38.png)
3. Full fill required information
![blob-trigger5]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-39.png)
4. Choose "Send a mail" action
![blob-trigger6]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-40.png)
5. Sign in and input required informations
![blob-trigger7]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-41.png)
![blob-trigger8]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-42.png)
![blob-trigger9]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-43.png)
6. Save "Logic App"
![blob-trigger10]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-44.png)
7. Test and verify
+ Refresh browser and check mail on inbox
![blob-trigger11]({{ site.baseurl }}/assets/images/az-basic-logic-app/az-basic-logic-app-45.png)

<br>
## Documents
+ MS Docs: [ms-doc](https://docs.microsoft.com/en-us/azure/logic-apps/)
+ Demo: [demo-video](https://www.youtube.com/watch?v=ZvsOzji_8ow&list=PLGjZwEtPN7j96A9JNpA4ouI3bH-uWZ0Ht)
