## PS: This project was intended for a useFetch Hook and not a useEffect Hook as the project title implies. thanks 

I created a custom useFetch hook that returns an object with the following data:
isLoading - Will be true while the fetch request is loading
isError - Will be true if the fetch request failed
data - Will contain the data from the fetch request

I also added the ability to pass down an options object to the useFetch hook that will set the options for the fetch request.
Added in the proper cleanup functionality for aborting a request if a new request is triggered before the old one finishes.
Added a promise.reject to return an error if the url doesn't exist