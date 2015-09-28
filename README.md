# PromiseAndHTTPFactoryInAngularJS
AngularJS: Integration of promises ($q) and $http in factory 

I have integrated promises ($q) with $http services, this will make code more extensible:

This will be shared service which will be consumed by all modules for executing CRUD operation,  Request Type, URL, Parameter Object will be passed to this shared service, so it will make code more maintainable, readable and scalable. If we don't go through this method then we have to use $http.get() or $http.post method, every where in services files of each module, content negotiation issues can be simply handled over here, If you want to append anything with each URL like 'Http:\\mydomain\' then instead of copy it on every service file,  just hard-code this thing in this file and append URL from their respective services. We don't need to mention protocol and host-name now in every URL request.
- It will be json valid.
- It will handle server errors.
- It will automatically display custom error message
- If it enters .then() everything went as planned.​
