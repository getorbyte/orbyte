
<aside style="width: 200px">

## Transfers
- <a href="./get">GET</a>
- <a href="./set.md">SET</a>
- <a href="./update.md">UPDATE</a>
- <a href="./delete.md">DELETE</a>

</aside>
<main >

# SET - Transfer
Orbyte's transfers allow integrate information from Orbyte to your project.

## Orbyte set
Allows you to set a new Post into Orbyte page.

### Items 
This option only accepts items. Check the items to be filled in when creating your new Post.

## NPM Set

### Call
    orbyte.connect({
        key: "<transfer_key_goes_here>",
        content: ["<content_goes_here>"]
    });

where

    key: String
    content: String[]

- key: Is the transfer key ID
- content: Array of the items you checked in Orbyte transfer

### Responses
#### success
    {
        statusCode: 200,
        message: 'Everything is OK!'
    }

#### Error
    {
        statusCode: 500,
        message: 'There was an error'
    }
</main>
