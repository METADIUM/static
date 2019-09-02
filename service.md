**Service File**

- Testnet Default : services_test.json  
- Testnet ko      : service_test_ko.json  
- Mainnet Default : services.json
- Mainnet ko      : services_ko.json

<br/>
<br/>

**Service JSON File format**
```json
{
  "{service_id}":{
    "name":"{name_of_service}",
	  "description":"{description_of_service}",
	  "icon":"{icon_image_url_of_service}",
	  "app":{
		  "web":{
        "launch_uri":"{web_url}"
      },
		  "android":{
			  "id":"{android_package_name}"
		  },
		  "ios":{
			  "id":"{apple_app_id}",
			  "launch_uri":"{launch_scheme}"
		  }
	  },
    "vp":{
      "{presentation_name}":["{credential_name}"]
    }
  }
```

- presentation_name : {xxx}Presentation. Must unique
- credential_name : Pre-defined credential
  - EmailCredential
  - NameCredential
  - DateOfBirthCredential
  - GenderCredential
  - NationalityCredential
  - MobileNumberCredential
  
  
