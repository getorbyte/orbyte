# GET - Transfer
Orbyte's transfers allow integrate information from Orbyte to your project.

## Orbyte Get
Allows you to get information. With this options you can select:

### Items 
Check the items to want to display when reciving the information

### Number of posts
Total posts you want to display

    All posts (display all posts)
    Custom (custom number of posts)

### Filters
Filter your posts. Choose an item into the list and create a conditional rule for the specific item. You can filter by:

    '=' (equal than)
    '>' (greater than) *
    '≥' (equal or greater than) *
    '<' (smaller than) *
    '≤' (equal or smaller than) *
    'D' (Dinamyc content, its an equal comparer that sets the value on your project)

<small>* Only works with integers or floats</small>

## NPM Update

### Call
    orbyte.connect({
        key: "<transfer_key_goes_here>",
        filter: ["<content_goes_here>"]
    });

where

    key: String
    filter: string[]

- key: Is the transfer key ID
- filter: Array of the filter that you checked with D (dynamic) option

### Responses
#### success
    {
        statusCode: 200,
        message: 'Everything is OK!',
        data: Object[]
    }

#### Error
    {
        statusCode: 500,
        message: 'There was an error'
    }

## Transfers
- <a href="./get.md">GET</a>
- <a href="./set.md">SET</a>
- <a href="./update.md">UPDATE</a>
- <a href="./delete.md">DELETE</a>