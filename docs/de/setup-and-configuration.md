---
layout: default
title: Setup and Configuration 
nav_order: 1
locale: de
---

# [](#header-1)Setup and Configuration

* * *

![](../../../assets/images/header-banner.jpg)

**ADTNG** is a fully hosted secure solution (hosted on Azure), managed and maintained by BCC Ltd.
In order to make use of ADTNG you will need to register the **ADTNG** application against each Office 365 tenant that you would like to manage. This is done through the Azure portal of each [Office 365 tenant](https://portal.azure.com){:target="_blank"}
This application registration will allow the **ADTNG** application to access the O365 objects it needs to maintain.

## [](#header-2)Azure Portal Setup

*	As a **Tenant Administrator** go to [https://portal.azure.com](https://portal.azure.com){:target="_blank"}
*	Access the **Azure Active Directory** section
*	Select **App registrations** and **+New Registration**

{: .mt-lg-5 .mt-md-5 }

![](../../../assets/images/azure-app-reg-1.png)


The application registration form will need to be provided with the following options.

* Click on Register

![](../../../assets/images/azure-app-reg-2.png)

Once the registration is complete you will see a screen similar to the one below:

![](../../../assets/images/azure-app-reg-3.png)

Keep a copy of the Application (client) ID and the Tenant ID as these will be required later on (respectively Client ID and Tenant ID)


We
<h2>here : {{ site.data.navs.docs_list_title }}</h2>
<ul>
   {% for item in site.data.navs.docs %}
      <li><a href="{{ item.url }}">{{ item.title }}</a></li>
   {% endfor %}
</ul>


1. Click on Add a certificate or secret

2. Click on +New client secret

3. Enter the Description for this secret (for example ADTNG Application Secret)

4. Enter a secret duration (Expires) (for example 24 months but do follow your corporate security policy if applicable)

5. Click Add

6. Copy the Value of the key to your clipboard (as per screen below). This will be required later on (Client Secret).

