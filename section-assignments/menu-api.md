# Section Assignment 2: Restaurant Menu API

## Scenario
Your job is to write the test plan and execute the test cases for an API that mimicks a restaurant menu.
> This endpoint uses mocked data, so while adding and deleting items will return changes in the response payload, there's no database connected, so adding or deleting items won't persist those changes upon subsequent calls. That means if you add an item to the menu or delete an item, it'll work just for that one time. If you get the menu again, it'll be back to its original state.

## Pre-work Guides
- [API Introduction](../guides/api-introduction.md)
- [Using Postman](../guides/postman.md)

## API Information
Here's some basic information about this API:

-   `GET` endpoint: `api/v2/engineeronboarding/menu`
-   `POST` endpoint: `api/v2/engineeronboarding/menu/addItem`
-   `DELETE` endpoint: `api/v2/engineeronboarding/menu/deleteItem/{itemNumber}`
-   Example menu item object:

```json
{ "itemNumber": 1, "name": "Pizza Slice", "price": 4.5, "calories": 350 }
```

## Instructions
- Create a test plan to cover all of the above endpoints
- Execute the test cases in Postman and document the results either in GitHub or a format of your choice
