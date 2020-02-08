## HttpUrlConnection
  * Explicitly handle redirects by inspecting the response code (3xx is redirect)
  * Create another connection for redirects
  * If redirect is to same domain, consider passing the Auth token. Don't pass sensitive data to another domain
  * HttpUrlConnection may utilize a cache and respond to redirects without a network request. Cache can be disabled.
