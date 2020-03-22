
<aside style="width: 200px">

## Transfers
- <a href="./get">GET</a>
- <a href="./set.md">SET</a>
- <a href="./update.md">UPDATE</a>
- <a href="./delete.md">DELETE</a>

</aside>
<main >

# DELETE - Transfer
Orbyte's transfers allow integrate information from Orbyte to your project.

## Orbyte Delete
Allows you to delete a post.

## NPM Delete

### Call
    orbyte.connect({
        key: "<transfer_key_goes_here>",
        postId: "<id_post_goes_here>"
    });

where

    key: String
    postId: String

- key: Is the transfer key ID
- postId: The post ID that you want to delete

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


</main>
