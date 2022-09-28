# Sending HTTP GET requests asynchronously in Rus

- A The runtime usage is defined on top of the main function of your application
- B We mark the main function as async, so we can use wait inside
- C We are using the crate reqwest here to execute a HTTP GET request, which will return a type Future
- D We use the await keyword to tell the program we want to wait for the Future to be in a finished state before we
  move on in this function
- E We print out the content of our response
- F The keyword Ok returns a Result - an empty one in this case
