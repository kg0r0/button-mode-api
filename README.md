# button-mode-api
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)  
:white_square_button: Experimental implementation of Button Mode API  

 This simple implementation provides for developers to try out [Button Mode API](https://developers.google.com/privacy-sandbox/blog/fedcm-chrome-125-updates) in their local environment. 

:construction: **Note: This is not ready for production** :construction:

## Usage

From Chrome 125, the Button Mode API is starting an origin trial on desktop. So now we need to use Chrome Canary to enable ``FedCmButtonMode``.

<img width="1498" alt="image" src="https://github.com/kg0r0/button-mode-api/assets/33596117/ff4419cf-afbc-43d5-98e4-e2afdb8e0431" width=600px>

Run the IdP and RP server with the following commands:

```bash
button-mode-api/rp $ go run main.go

button-mode-api/idp $ go run main.go
```

Access to http://localhost:8081.

![button_mode_api](https://github.com/kg0r0/button-mode-api/assets/33596117/9f75377a-2ab4-4a3c-9e56-19b02f954e7e)


## Sign-in flow

You can see the following authentication flow from the [Federated Credential Management API developer guide](https://developers.google.com/privacy-sandbox/3pcd/fedcm-developer-guide).
<img src="https://developers.google.com/static/privacy-sandbox/assets/images/idp-endpoints-a67327f46da51.png" width= "600px" >

## References
- https://developers.google.com/privacy-sandbox/blog/fedcm-chrome-125-updates
- https://developers.google.com/privacy-sandbox/3pcd/fedcm-developer-guide
- https://developers.google.com/privacy-sandbox/blog/fedcm-chrome-120-updates
