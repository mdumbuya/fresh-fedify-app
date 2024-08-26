# Fresh Auth Project

## Table of Contents

- [Fresh Auth Project](#fresh-auth-project)
  - [🚀 Overview](#overview)
  - [✨ Features](#features)
  - [🚀 Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
  - [📂 Project Structure](#-project-structure)
  - [Usage](#usage)
  - [Middleware](#middleware)
  - [Deployment](#deployment)
  - [Contributing](#contributing)
  - [📸 Screenshots](#-screenshots)
    - [Home Page](#home-page)
    - [Sign Up](#sign-up)
    - [Login](#login)
    - [Access Restricted Page](#access-restricted-page)
  - [📝 License](#license)
  - [🙌 Acknowledgments](#-acknowledgments)
  - [📬 Contact](#-contact)
    
## Overview

This project is a web application built using [Fresh](https://fresh.deno.dev/), a modern web framework for Deno, designed to be fast and efficient. The application integrates Supabase for user authentication, allowing users to sign up, log in, and access protected routes.

## Features

- **User Authentication:** Allows users to sign up, log in, and log out.
- **Protected Routes:** Certain pages are accessible only to logged-in users.
- **Supabase Integration:** Uses Supabase for authentication and user management.
- **Responsive Design:** Built with Tailwind CSS, ensuring the app looks great on all devices.

## Getting Started

### Prerequisites

- **Deno:** Ensure you have Deno installed. You can download it from [deno.land](https://deno.land/).
- **Supabase Account:** You need a Supabase project. Sign up at [Supabase](https://supabase.com/).

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/fresh-auth-project.git
   cd fresh-auth-project
   ```

2. Set up environment variables:

Create a .env file in the root directory and add your Supabase credentials:

    ```bash
    SUPABASE_URL=https://your-supabase-instance.supabase.co
    SUPABASE_KEY=your-supabase-anon-key
    ```

3. Install dependencies:

Fresh doesn't require a package manager like npm or yarn. However, make sure you have Deno installed.

4. Run the development server:

Start the Deno development server with:

    ```bash
    deno task start
    ```

The app will be available at [http://localhost:8000](http://localhost:8000).

## 📂 Project Structure

```bash
..
├── components
│   ├── Layout.tsx
│   └── Nav.tsx
├── deno.json
├── dev.ts
├── fresh.config.ts
├── fresh.gen.ts
├── islands
├── main.ts
├── README.md
├── routes
│   ├── _404.tsx
│   ├── _app.tsx
│   ├── auth
│   ├── index.tsx
│   ├── login.tsx
│   ├── logout.tsx
│   ├── _middleware.ts
│   └── signup.tsx
├── static
│   ├── favicon.ico
│   ├── logo.svg
│   ├── styles.css
│   └── walking_in_rain.svg
└── tailwind.config.ts
```

## Usage

- **Home Page:** The landing page of the application.
- **Login Page:** Allows users to log in with their credentials.
- **Signup Page:** Allows new users to create an account.
- **Secret Page:** A protected route that only logged-in users can access.

## Middleware

The `_middleware.ts` file handles the authentication logic. It checks if the user is logged in by verifying the presence of a Supabase token in the cookies. If the token is valid, the user can access protected routes.

## Deployment

To deploy the application, you can use Deno Deploy or any other platform that supports Deno. Ensure your environment variables are set up correctly in the deployment environment.

## Contributing

Contributions are welcome! Please fork the repository and use a feature branch. Pull requests are warmly welcome.

## 📸 Screenshots
### Home Page
[Home Page](./screenshots/home.png)

### Sign Up
[Create Account](./screenshots/create_account.png)

### Login
[Login](./screenshots/login.png)
[Successfull Login](./screenshots/logged_in_success.png)


### Access Restricted Page
[Secret](./screenshots/secret.png)

## License

This project is open source and available under the MIT License.

## 🙌 Acknowledgments

    Fresh Framework
    Preact
    Deno
    Tailwind CSS

Thanks to [@learnbydoing993](https://github.com/learnbydoing993) for this [code](https://github.com/learnbydoing993/fresh-auth-supabase).   

## 📬 Contact

Feel free to reach out if you have any questions or suggestions!

[LinkedIn](www.linkedin/in/mdumbu) 

[Mastodon](https://mastodon.social/@backyardcoding)
