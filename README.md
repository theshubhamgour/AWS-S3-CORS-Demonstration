# AWS S3 CORS Demonstration

This repository contains a demonstration of how to configure CORS (Cross-Origin Resource Sharing) in AWS S3 to allow web applications to securely interact with resources hosted on S3. The demonstration includes both the HTML and the CORS configuration file used to make requests to an S3 bucket.

## Overview

The project demonstrates the following:
- Setting up an S3 bucket with the appropriate CORS configuration.
- Creating a simple HTML file to fetch data from the S3 bucket.
- Displaying the fetched data on the web page.

### Screenshot

![AWS S3 CORS Demonstration](https://github.com/user-attachments/assets/02eb52a8-b25f-4049-a957-d8a22cb6e795)


## Files Included

- **index.html**: The HTML file that contains the frontend code to fetch data from the S3 bucket using JavaScript.
- **CORS Configuration**: The JSON file containing the CORS rules for the S3 bucket.

## How to Use

1. Clone this repository.
2. Upload the `index.html` to your S3 bucket.
3. Apply the CORS configuration provided in the JSON file to your S3 bucket.
4. Access the `index.html` file via the S3 bucket's public URL to see the CORS demonstration in action.

## CORS Configuration

Here is the sample CORS configuration used in this demonstration:

```json
[
    {
        "AllowedHeaders": [
            "Authorization"
        ],
        "AllowedMethods": [
            "GET"
        ],
        "AllowedOrigins": [
            "<url-of-s3-bucket>"
        ],
        "ExposeHeaders": [],
        "MaxAgeSeconds": 3000
    }
]
```
## Conclusion
This demonstration shows how to configure AWS S3 CORS settings to allow your web applications to securely access resources stored in S3. 
This is a basic setup, but it can be expanded to accommodate more complex requirements.

Feel free to fork and experiment with the code to suit your needs!


You can save this content in a file named `README.md` and include it in your GitHub repository along with the `index.html` and CORS configuration files. 
Make sure to replace the image filename with the correct path if it’s different in your repository.



