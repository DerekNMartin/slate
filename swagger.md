--- 

title: API V2 

language_tabs: 
   - shell 

toc_footers: 
   - <a href='#'>Sign Up for a Developer Key</a> 
   - <a href='https://github.com/lavkumarv'>Documentation Powered by lav</a> 

includes: 
   - errors 

search: true 

--- 

# Introduction 

**Version:** v2 

# /V2/AUTHN/ACTIVATE
## ***POST*** 

**Summary:** Activates an authenticator

### HTTP Request 
`***POST*** /v2/authn/activate` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| bcaccesskey | header | Key that identifies the account | No |  |
| authenticator | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | activated the authenticator |
| 404 | fails to activate authenticator given invalid accesskey |

# /V2/CLIENTZ/VERIFY
## ***POST*** 

**Summary:** Selective Modality Verification

### HTTP Request 
`***POST*** /v2/clientz/verify` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| bcaccesskey | header | Key that identifies the account | No |  |
| bcentitykey | header | Key that identifies the client | No |  |
| bcsecrettoken | header | Client secret token | No |  |
| verification | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Create a normal verification |

<!-- Converted with the swagger-to-slate https://github.com/lavkumarv/swagger-to-slate -->
