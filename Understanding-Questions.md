# Understanding Questions:
1. What are the steps of execution from the pressing of the 1 button to the rendering of our updated value? List what part of the code executes for each step.
* The user presses the 1 button.
* The onClick listener executes the function handleAdd1.
* handleAdd1 executes addOne() which creates the action object, which in this case it just has a property of type and no payload.
* The reducer function is run, and the action property of type is applied to a switch statement as the argument. 
* The case matching the action type ADD_ONE is run and it returns a new state with an added increment of 1 to the total.
* Since state was changed, React re-renders the DOM.
* TotalDisplay shows the total plus 1.
