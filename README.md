# React Todo App Add and Delete

> Check the [DEMO LINK]()

## Adding a todo

- 
- Submit a new todo with the entered title.
- Input field auto-focuses by default.
- Display a "Title should not be empty" message if submitted with an empty title.
- Trim the title on save.
- Use your userId for the new todo.
- Send a POST request to the API (refer to API documentation).
- Disable the input during the API request.
- Create a temporary todo (tempTodo) with id: 0 and show it separately from the list.
- Display a loader for the temp todo while waiting for the response.
- On success: add the todo from the API response to the list, clear the input, and focus the field.
- On error: show "Unable to add a todo" message and keep the input text.
- Skip animations for adding/removing todos unless time permits.

> Don't try to implement animations for adding or removing Todos (at least until you finish everything else).
> If you really feel confident to try, there is a hint at the end of the description.

## Deleting todos

- Delete a todo on button click, showing a loader while waiting for the API response.
- On success: remove the todo from the list.
- On error: show "Unable to delete a todo" message and keep the todo.
- Clear all completed todos using the "Clear completed" button:
  - Button is enabled if at least one todo is completed.
  - Deletes todos individually.
  - Show error message if any deletion fails, but proceed with successful deletions.

## Testing
- open `cypress/integration/page.spec.js`
- replace `describe.skip` with `describe` for the root `describe`
