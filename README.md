## About The Project

This is the final codebase for our [Pusher tutorial](https://pusher.com/tutorials/how-to-build-a-chat-app-with-vue-js-and-laravel/).

### About us

Pusher does Websocket infrastructure so you don't need to. [Check us out](https://pusher.com/).

<!-- GETTING STARTED -->
## Getting Started

If you don't want to follow the tutorial, and just want to get a local copy up and running, follow these steps.

### Prerequisites

You will need PHP, Composer and Node.js. For MacOS I recommend installing them with [Homebrew](https://brew.sh/). For Windows see instructions for [PHP](https://windows.php.net/download/), [Composer](https://getcomposer.org/doc/00-intro.md#installation-windows) and [Node](https://nodejs.org/en/download/).

### Installation

1. Get your free Pusher API Keys at [https://pusher.com](https://pusher.com)
2. Clone this repo
3. Install Composer packages
   ```sh
   composer install
   ```
4. Install NPM packages
   ```sh
   npm install
   ```
5. Create a sqlite database file in the database folder
    ```sh
    touch db.sqlite
    ```
6. Enter your API keys in `.env`
   ```
    PUSHER_APP_ID=
    PUSHER_APP_KEY=
    PUSHER_APP_SECRET=
    PUSHER_APP_CLUSTER=
   ```
7. Enter the path to your database file
    ```
    DB_DATABASE=<Full path to the sqlite file>
    ```
8. Initilise the database
    ```sh
    php artisan migrate
    ```
9. Compile the webpages and run it
    ```sh
    npm run dev
    php artisan serve
    ```

<!-- USAGE EXAMPLES -->
## Usage

Go to http://127.0.0.1:8000/, register a couple of users and start chatting!

<!-- CONTACT -->
## Contact

- Want so ask a Pusher a question? [Contact support here](https://support.pusher.com/hc/).
- If you want to raise an issue with our PHP SDK, [do it here](https://github.com/pusher/pusher-http-php).
 
## Credits

Owned by [Pusher](https://pusher.com).

## License

PusherSwift is released under the MIT license. See [LICENSE](https://github.com/pusher/laravel-chat/blob/master/LICENSE.md) for details.