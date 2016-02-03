# webhooks

Testing webhooks.

Editing this file in the GitHub UI does result in a webhook message.

Changed the header mapping to get the X- headers mapped through

Refactored the packages.

Added in routing on the user agent header for GitHub web hook

Routing didn't work on a wild carded header value.

## headers

```
content-length=5846, 
http_requestMethod=POST, 
x-github-event=push, 
x-github-delivery=3f381c00-ca7e-11e5-8fbe-17989828c7be, 
host=localhost:8080, 
http_requestUrl=http://localhost:8080/hooks/git, 
connection=close, 
id=98ccf1a6-34f1-4c78-2cc3-ca5baa072587, 
contentType=application/json;charset=UTF-8, 
accept=*/*, 
user-agent=GitHub-Hookshot/21f57ba, 
timestamp=1454507929898
```
