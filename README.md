<h1 align="center">Bruno Collections for CyberArk Identity Security REST API</h1>

<table>
<tr>
<td>
  
Bruno Collection and Environment files for **CyberArk Identity Security** REST API testing and automation. Over 800 REST API requests are included in the Collections, which cover Self-Hosted PAM, Privilege Cloud - Standard, Privilege Cloud on Identity Security Platform for Shared Services (ISPSS/Shared Services), and many shared services from the SaaS platform.

Each API request includes small optimizations to help get you up and running quickly, for example:
  * Authentication requests test for and store the resulting tokens as Environment variables.
  * Authentication token is automatically populated to request headers where necessary.
  * Documentation links and important notes are stored inside each request's 'Docs' section.
  * Mandatory URI parameters are selected by default and vice-versa.
  * Central Credential Provider 'GetPassword' request included with every Collection.

![Bruno Collection OIDC Authentication](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/blob/main/assets/brunoCollectionOIDCAuth.png)

</td>
</tr>
</table>

## Installation

##### To import from JSON (Easiest method):
1. Download the latest version of both the 'Environment' and 'Collection' JSON files that correspond to your environment:
  * Privilege Cloud and/or Shared Services:
    * [Collection](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/blob/main/Privilege%20Cloud%20and%20Shared%20Services%20REST%20API/Privilege%20Cloud%20and%20Shared%20Services%20REST%20API.json)
    * [Environment](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/blob/main/Privilege%20Cloud%20and%20Shared%20Services%20REST%20API/Privilege%20Cloud%20Shared%20Services%20Environment.json)

  * Self-Hosted PAM:
    * [Collection](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/blob/main/CyberArk%20Self-Hosted%20REST%20API/CyberArk%20Self-Hosted%20REST%20API.json)
    * [Environment](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/blob/main/CyberArk%20Self-Hosted%20REST%20API/Self-Hosted%20Environment.json)
2.  From the Bruno start page, click 'Import Collection' > 'Bruno Collection' and select the Collection JSON file.

> [!IMPORTANT]  
> You must use Bruno v1.19 or later to import JSON files.

3.  Once the Collection is imported, expand the Collection tree down and select any API request. Press 'ctrl'+'e' on the request page to open the Environments menu.

4. Click 'Import' in the lower left then select the Environment JSON file to use with the Collection.

##### To import Bruno Collection natively (Advanced):
1.  Uploading native .bru project files is on the roadmap.

## Collections

#### CyberArk Privilege Cloud and Shared Services REST API:
  This Collection is meant to help CyberArk Privilege Cloud and CyberArk Identity administrators manage and explore the CyberArk Shared Services/SaaS environment with REST API. For ease of use, the Environment JSON file is alphabetized and includes only relevant environment variables. All default services that are part of the Shared Services platform are included:

  * CyberArk Privilege Cloud - Standard
  * CyberArk Privilege Cloud - Shared Services
  * CyberArk Identity - Shared Services
  * Connector Management
  * Dynamic Privileged Access (DPA)
  * Secure Cloud Access (SCA)
  * Remote Access V2
  * EPM SaaS (Select requests for EPM LCD)
  * Secrets Hub
  * Central Credential Provider (CCP)
  * Conjur Cloud

  Current up to Privilege Cloud v14.2 (August 2024)

#### CyberArk Self-Hosted REST API:
  This Collection is meant to help self-hosted CyberArk PAM administrators manage and explore the PAM environment with REST API. For ease of use, the Environment JSON file is alphabetized and includes only relevant environment variables. The following services are included:

  * Self-Hosted PAM
  * Central Credential Provider (CCP)

  Current up to Password Vault Web Access (PVWA) v14.2 (August 2024)

## Roadmap

- [x] Add Privilege Cloud Collections (28 Jul 2024)
- [x] Add Self-Hosted PAM Collection (4 Aug 2024)
- [x] Add Identity and Shared Services to SaaS Collection: (18 Aug 2024)
    - [x] Identity on Shared Services (28 Jul 2024)
    - [x] Dynamic Privileged Access (10 Aug 2024)
    - [x] Connector Management (10 Aug 2024)
    - [x] Remote Access (10 Aug 2024)
    - [x] Endpoint Privilege Manager (For LCD) (10 Aug 2024)
    - [x] Secure Cloud Access (17 Aug 2024)
    - [x] Identity - Workforce Password Management (17 Aug 2024)
    - [x] Identity - SCIM (17 Aug 2024)
    - [x] Secrets Hub (17 Aug 2024)
    - [x] Conjur Cloud (18 Aug 2024)
- [ ] Add additional services to Self-Hosted Collection:
    - [ ] Remote Access
    - [ ] Endpoint Privilege Manager
- [ ] Add usage guide
- [ ] Upload native .bru project files
- [ ] UX enhancements:
    - [ ] Expand documentation
    - [ ] Improve examples for params
    - [ ] Improve examples for bodies
    - [ ] Expand tests and scripts

## Contact

Maintained by Eli Hopkins, [@IAM-Jah](https://github.com/IAM-Jah). Contact information is located in my profile.

## Acknowledgements

This project would not have been possible without the wealth of knowledge made available by Joe Garcia, [@infamousjoeg](https://github.com/infamousjoeg), and others at CyberArk Software.

## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)