# UPDATE - Transfer
Orbyte's transfers allow integrate information from Orbyte to your project.

## Orbyte Update
Allows you to update information in a Post. With this options you can select:

### Items 
This option only accepts items. Check the items to be updated in your post.

## NPM Update

### Call
    orbyte.connect({
        key: "<transfer_key_goes_here>",
        content: ["<content_goes_here>"],
        postId: "<id_post_goes_here>"
    });

where

    key: String
    content: String[]
    postId: String

- key: Is the transfer key ID
- content: Array of the items you checked in Orbyte transfer
- postId: The post ID that you want to update

### Responses
#### success
    {
        statusCode: 200,
        message: 'Everything is OK!'
    }

#### Post not found
    {
        statusCode: 404,
        message: 'Post not found'
    }
#### Error
    {
        statusCode: 500,
        message: 'There was an error'
    }