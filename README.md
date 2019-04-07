# Backpulse

> Headless CMS built with ❤.

[Jump to documentation](#documentation)

## What it is

Backpulse.io is an open source API Based / Headless CMS.  
Manage your site's content through Backpulse's interface and retrieve it with a secure API.

[@backpulse](https://github.com/backpulse) on GitHub.

## Features

- Unlimited sites
- Storage
- API endpoint encrypted with a Cloudflare SSL certificate
- Contribution
- Easy to use
- Dark theme

## Examples

My blog is powered by Backpulse.io. Check it [out](https://blog.aureleoules.com)

[GitHub source](https://github.com/aureleoules/blog)

## Donate

Please consider donating if you think **Backpulse** is helpful to you or that my work is valuable.  
I would be very grateful!  
  
[![Donate](https://img.shields.io/badge/Donate-Crypto-blue.svg)](https://commerce.coinbase.com/checkout/b4d64264-dda8-41d0-9f15-0843f969fa79)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/aureleoules)

## Contribute

All contributions are welcome!  

[backpulse/core](https://github.com/backpulse/core) built with Go  
[backpulse/dashboard](https://github.com/backpulse/dashboard) built with React  
[backpulse/frontpulse](https://github.com/backpulse/frontpulse) built with React  

# Documentation
Welcome to [Backpulse](https://www.backpulse.io)'s documentation!

## Getting started

Your API Endpoint is : `https://api.backpulse.io/:sitename`.  
Where `:sitename` is your site's name.

Exemple of a successful request:
```json
{
    "status": "success",
    "code": 200,
    "message": "success",
    "payload": {}
}
```

Exemple of a 404 (not found) error:
```json
{
    "status": "error",
    "code": 404,
    "message": "not_found",
    "payload": null
}
```

## Routes
List of all available routes for the client api.

### About
Fetch about informations  
> GET `/about`  

Response:
```json
{
    "status": "success",
    "code": 200,
    "message": "success",
    "payload": {About}
}
```

### Contact
Fetch contact informations
> GET `/contact`

Response:
```json
{
    "status": "success",
    "code": 200,
    "message": "success",
    "payload": {Contact}
}
```

### Articles
* Fetch all articles of site. 
    > GET `/articles`  

    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": []Article
    }
    ```

* Fetch specific article.
    > GET `/articles/:shortid`

    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": Article
    }
    ```

### Galleries
* Fetch all galleries of site.
    > GET `/galleries`  
    
    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": []Gallery
    }
    ```

* Fetch specific gallery.
    > GET `/gallery/:shortid`

    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": Gallery
    }
    ```

* Fetch default gallery.
    > GET `/galleries/default`

    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": DefaultGallery
    }
    ```

### Projects
* Fetch all projects of site.
    > GET `/projects`  
    
    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": []Project
    }
    ```

* Fetch specific project.
    > GET `/projects/:shortid`

    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": Project
    }
    ```

### Albums
* Fetch all albums of site.
    > GET `/albums`  
    
    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": []Album
    }
    ```

* Fetch specific album.
    > GET `/albums/:shortid`

    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": Album
    }
    ```

* Fetch specific track.
    > GET `/tracks/:shortid`

    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": Track
    }
    ```

### Video groups
* Fetch all vide groups of site.
    > GET `/videogroups`  
    
    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": []VideoGroup
    }
    ```

* Fetch specific video group.
    > GET `/videogroups/:shortid`

    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": VideoGroup
    }
    ```

* Fetch specific video.
    > GET `/videos/:shortid`

    Response:
    ```json
    {
        "status": "success",
        "code": 200,
        "message": "success",
        "payload": Video
    }
    ```