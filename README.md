# Mission
Develop Github user search app for iOS.

# Condition
Pagination.  
Present searched user list.

# Idea
Use GraphQL supported by Github API.  
Use Reactive framework to implement complex search flow.

# Use of API
For using Github API, you have to generate access-token.  
https://github.com/settings/tokens  
Because of the token is private resource,  
i stored as a file and include git-ignore list for preventing distribution.

# Implementation
For using GraphQL,  
create "POST" request by putting query in the request body.  
There is a 3rd party library 'Apollo-ios' but i developed all by myself.  
https://developer.github.com/v4/

For implementing complex search flow,  
i separated reactive parts to 'UI' and 'Data'.  
It helps giving me a clear logic and obeying SRP.

GraphQL Querying is most tricky part to me.  
The format is strict and there is no easy way to manipulate it.  
Perhaps 'Apollo-ios' would helps.
