# Readings: CRUD

## **In your own words, describe what each group of status code represents:**

**100’s** = tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. 

**200’s** = tell the client that its request was accepted.

**300’s** = tell the client that the resource they are requesting isn’t available at the expected location anymore.

**400’s** = These are the client error codes.

**500’s** = These are the server error codes.

## **What is a status code 202?**
    
This code tells the client that the request was valid, but its processing will finish sometime in the future. 

## **What is a status code 308?**

This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

## **What code would you use if an update didn’t return data to a client?**

204 No Content. 

## **What code would you use if a resource used to exist but no longer does?**

410 Gone 

## **What is the ‘Forbidden’ status code?**

403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

----------

**To know more please 
[visit this page](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)**

----------