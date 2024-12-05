# React Todo App Load Todos

The task consists of 3 part:
- (This repo) [Load todos](https://github.com/mate-academy/react_todo-app-loading-todos)
- [Add and Delete](https://github.com/mate-academy/react_todo-app-add-and-delete)
- [Toggle and Rename](https://github.com/mate-academy/react_todo-app-with-api)

In this 1st part:

- implement todos loading
- implement error messages
- implement filtering by status

## General principles

> Keep your logic as simple as possible!

Improve user experience:
- hide or disable elements that can't be used at the moment
- focus text fields, so user could start typing without extra clicks
- prevents users from doing the same action twice accidentally (disable controls when action is in progress)
- show spinners on todos immediately to notify the user that action is in progress
- update todos only after successful save to the API (tests expect such behaviour)
- in case of any error show a notification (and hide it after delay)
- clear input values on `success` and preserve and focus on `error`


## Show Error Messages

In case of any error show the notification with an appropriate message at the bottom

- the notification can be closed with the `close` button (add the `hidden` class, **DON'T** use conditional rendering);
- automatically hide the notification after 3 seconds;
- hide the notification before any next request;

## Filter Todos by Status

Filter todos by status `All` / `Active` / `Completed`:

- all todos should be visible by default
- use the `selected` class to highlight a selected link;

## Demo Links

- [DEMO LINK](https://AndriiZakharenko.github.io/react_todo-app-loading-todos/)
