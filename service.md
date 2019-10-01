## Service File

- Testnet Default : services_test.json  
- Testnet ko      : service_test_ko.json  
- Mainnet Default : services.json
- Mainnet ko      : services_ko.json

<br/>
<br/>

## Service JSON File format
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
				"launch_uri":"{ios_launch_scheme}"
			}
		},
		"key_id":"{key_id_of_did}",
		"vp":{
			"{presentation_name}":["{credential_name}"]
		}
}
```
- service_id : Unique id of service.
- name_of_service : to be shown to keepin.
- description_of_service : to be shown to keepin.
- icon_image_url_of_service : to be shown to keepin.
- web_url : to be linked in keepin.
- android_package_name : to be linked in keepin.
- apple_app_id : to store in keepin.
- ios_launch_scheme : to be linked in keepin.
- key_id : key id of did of service. Need regisger Meta ID. If exists "vp", must have did and key id. Use encrypt to save vp to IdentityHub
- presentation_name : {xxx}Presentation. Must unique
- credential_name : Pre-defined credential
  - EmailCredential
  - NameCredential
  - DateOfBirthCredential
  - GenderCredential
  - NationalityCredential
  - MobileNumberCredential
  
  
