# UpdateProfile
API for updating user profile information.

## Overview
The UpdateProfile API allows users to update their profile information with ease. This includes modifying personal details, contact information, and preferences.

## Endpoint
- **URL:** `/api/profile/update`
- **Method:** `PUT`
- **Content-Type:** `application/json`

## Request Body
```json
{
  "userId": "string",
  "fullName": "string",
  "email": "string",
  "phoneNumber": "string",
  "address": "string"
}
```

## Response
- **Success:**
  - **Code:** 200 OK
  - **Content:**
    ```json
    {
      "message": "Profile updated successfully."
    }
    ```
- **Error:**
  - **Code:** 400 Bad Request
  - **Content:**
    ```json
    {
      "error": "Error description."
    }
    ```

## Usage
To update a user's profile, send a `PUT` request to the `/api/profile/update` endpoint with the updated profile information in the request body.
