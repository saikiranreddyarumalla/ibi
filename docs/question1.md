
# What are the differences between cookie, local storage and session storage?

Cookies, local storage, and session storage are three different ways to store data in a web browser. Each of them has distinct characteristics and use cases. Here are the main differences between them:

## Storage Duration:
Cookies: Cookies have an expiration date, meaning they can be set to persist for a specified period or until they are explicitly deleted. They can be set with an expiration time, making them suitable for persistent data across multiple sessions.
Local Storage: Data stored in local storage persists indefinitely until it is explicitly cleared by the user or the web application. It remains available even after the browser is closed and reopened, making it useful for long-term storage.
Session Storage: Data stored in session storage lasts only for the duration of the browser session. It is cleared when the browser is closed, making it suitable for temporary data that should be available within the same session.

## Data Capacity:
Cookies: Cookies have a size limit of typically around 4KB, which is relatively small compared to local storage and session storage.
Local Storage: Local storage provides a larger storage capacity (usually up to 5-10 MB), making it more suitable for storing larger amounts of data.
Session Storage: Like local storage, session storage also provides a larger capacity compared to cookies but is typically limited to the same 5-10 MB range.

## Sending to Server:
Cookies: Cookies are automatically sent to the server with every HTTP request for the specific domain they belong to. This can potentially add extra overhead to each request.
Local Storage: Local storage data is not automatically sent to the server with each request, reducing the potential overhead.
Session Storage: Similar to local storage, session storage data is not sent to the server with each request.

