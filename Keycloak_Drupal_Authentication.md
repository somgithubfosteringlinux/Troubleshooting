
## Troubleshooting steps for OIDC keycloak authentication in drupal:

* <b>Download the below OIDC module for drupal from below link:</b><br/>
  https://ftp.drupal.org/files/projects/keycloak-8.x-1.5.zip

------

* <b>Login to Drupal main console then select Extend -> modules -> Install New module.</b>
* Upload and Install the downloaded modules.
  
    <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Extend_Install-new-module.png"></p>
    
------

* <b>The downloaded modules will appear as below in installed modules:</b>
  
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Installed_modules.png"></p>
     
 ------
     
* <b>Now, we have to add the OpenID connect button:</b>
* Click on manage -> block layout
 
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Structure_blocl_layout.png"></p>
     
------
     
* <b>Select sidebar first in block layout -> select OpenID connect (at sidebar first) as shown below:</br>
     
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/sidebar_first_OIDC_button.png"></p><br/>
     
     <b>Output on the drupal mainpage:</b><br/>
    
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/oidc_button_homepage.png"></p>
     
------
* <b>Click on manage from drupal navigation bar, and select configuration -> webservices -> OpenId connect:</b>
  
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Configuration_OpenID%20connect.png"></p>
  
     -> <b>Opt for below in changes to OpenID connect:<b><br/>
  
   <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/OpenID%20connect.png"></p>
-------

  * <b>Now select the Configuration -> Account Settings from Drupal navigation bar:</b>
  
  
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Configuration_Account-settings.png"></p>
     
     -> <b>Opt for visitors option in account settings:</b><br/>
     
     <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/Accountsetting_visitors.png"></p>

------
  
 Finally, while cicking on OpenID connect it will redirect to keycloak Authentication server:
   
   <p align="center"><img src="https://raw.githubusercontent.com/somgithubfosteringlinux/images/main/Troubleshoot_keycloak_Drupal_OIDC_Auth/keycloak_Drupal_Auth.gif"></p>
  
------

### Reference links:
1. https://www.drupal.org/project/keycloak
2. https://www.drupal.org/docs/8/modules/keycloak-openid-connect/configuration
