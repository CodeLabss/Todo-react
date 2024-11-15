Using context with local storage

Create a folder context and a file inside with .js and 2 things need to be used useContext and createContext

Next a custom hook conaining above context is written to directly import the custom hook anywhere  in the app and use it. 
along with a const provider to wrap the content like <Card />, etc inside of it

Below is the provider and Context:

Context -> export const TodoContext = createContext({

    1. todos array which will have id, msg of todo, and a boolean field for if the  todo is done or not
    2.  addTodo function to add a new todo
    3.  update function to update todo
    4.  deleteTodo function to delete a todo
    5.  toggleTodo function to toggle the todo status
})

export const TodoProvider = TodoContext.Provider

ABOVE IS CONTEXT

BELOW IS APP.JSX

Import everything like hooks, provider from context and display in the div
Wrap entire div in TodoProvider 
Add value attr in value and inside its object write all the functions in the value

