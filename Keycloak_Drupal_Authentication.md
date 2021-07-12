
## Troubleshooting steps for OIDC keycloak authentication in drupal:

* Download the below OIDC module for drupal from below link: <br/>
  https://ftp.drupal.org/files/projects/keycloak-8.x-1.5.zip

------

* Login to Drupal main console then select Extend -> modules -> Install New module.
* Upload and Install the downloaded modules.
  
    <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Extend_Install-new-module.png"></p>
    
------

* The downloaded modules will appear as below in installed modules:
  
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Installed_modules.png"></p>
     
 ------
     
* Now, we have to add the OpenID connect button:
* Click on manage -> block layout
 
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Structure_blocl_layout.png"></p>
     
------
     
* Select sidebar first in block layout -> select OpenID connect (at sidebar first) as shown below:
     
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/sidebar_first_OIDC_button.png"></p><br/>
     
     <b>Output on the drupal mainpage:</b><br/>
    
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/oidc_button_homepage.png"></p>
     
------
* Click on manage from drupal navigation bar, and select configuration -> webservices -> OpenId connect:
  
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Configuration_OpenID%20connect.png"></p>
  
     -> Opt for below in changes to OpenID connect:<br/>
  
   <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/OpenID%20connect.png"></p>
-------

* Now select the Configuration -> Account Settings from Drupal navigation bar:
  
  
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Configuration_Account-settings.png"></p>
     
     -> <b>Opt for visitors option in account settings:<b><br/>
     
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Accountsetting_visitors.png"></p>

------
  
 Finally, while cicking on OpenID connect it will redirect to keycloak Authentication server:
   
   <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/keycloak_Drupal_Auth.gif"></p>
  
------

### Reference links:
1. https://www.drupal.org/project/keycloak
2. https://www.drupal.org/docs/8/modules/keycloak-openid-connect/configuration
