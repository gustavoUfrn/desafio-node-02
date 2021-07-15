
# Read me
This project is the base an application to manage tasks. This time focused on working with middlewares.
#### This project is the base an application to manage tasks.
*Middlewares.* 

 - checksExistsUserAccount (checks if user already exist)
 - checksCreateTodosUserAvailability (checks if a new todo can be created)
		- 10 to non-pro accounts,
		- unlimited to pro accounts
- checksTodoExists (checks if the todo exists)
- findUserById (checks if user already exists by the user id)

*Requirements.* 
- Should be able to find user by username in header and pass it to request.user
- Should not be able to find a non existing user by username in header
- Should be able to let user create a new todo when is in free plan and have less than ten todos
- Should not be able to let user create a new todo when is not Pro and already have ten todos
- Should be able to let user create infinite new todos when is in Pro plan
- Should be able to put user and todo in request when both exits
- Should not be able to put user and todo in request when user does not exists
- Should not be able to put user and todo in request when todo id is not uuid
- Should not be able to put user and todo in request when todo does not exists
- Should be able to find user by id route param and pass it to request.user
- Should not be able to pass user to request.user when it does not exists
