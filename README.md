# URL Shortener in C++

## Overview

This is a simple URL shortener implemented in C++. It uses a basic console-based interface to shorten and retrieve URLs. The code includes a custom `LinkShortener` class that generates unique short codes for original URLs, ensuring no collisions occur. The main application provides an example of using the `LinkShortener` class to shorten and retrieve URLs.

## Implementation Details

### LinkShortener Class

The `LinkShortener` class is the core component responsible for shortening and retrieving URLs. It uses a random code generation algorithm to create unique short codes for each original URL. The `generateRandomCode` method generates a random alphanumeric code of a specified length.

The `shortenLink` method takes an original URL, generates a short code, and creates a shortened link by combining the base URL and the generated code. It ensures the generated link is unique by checking if it already exists in the internal storage.

The `getOriginalLink` method allows retrieving the original link based on a shortened link.

### Main Function

The `main` function demonstrates the usage of the `LinkShortener` class. It initializes a `LinkShortener` object with a base URL and showcases the process of shortening and retrieving URLs.
