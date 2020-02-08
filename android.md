## HttpUrlConnection
  * Explicitly handle redirects by inspecting the response code (3xx)
  * Extract the redirect url from response and make another request to it
  * If redirect is to same domain, consider passing the Auth token. Don't pass sensitive data to another domain
  * HttpUrlConnection may utilize a cache and respond to redirects without a network request. Cache can be disabled
  * HttpUrlConnection requests and response can be monitored by Android Studio's Profiler
  * On unauthorized requests, pass refresh token to get a new auth token, then re-try with the new auth token
