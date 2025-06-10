# UJTweet

**UJTweet** is a Django-based microblogging platform inspired by Twitter. Users can register, log in, create, edit, and delete tweets (with optional photos), and search for tweets by content. Only tweet owners can edit or delete their own tweets.

---

## Features

- User registration and authentication
- Create, edit, and delete tweets (with optional photo upload)
- Search tweets by content
- Only tweet owners can edit/delete their tweets
- Responsive UI with Bootstrap (customizable)
- Media upload support for tweet images

---

## Project Structure

```
ujnews/
├── manage.py
├── db.sqlite3
├── media/
│   └── tweetspic/
├── templates/
│   ├── layout.html
│   └── registration/
│       ├── login.html
│       ├── register.html
│       └── logged_out.html
├── tweet/
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   ├── views.py
│   └── templates/
│       └── tweet/
│           ├── tweet_list.html
│           ├── tweet_form.html
│           └── tweet_confirm_form.html
└── ujnews/
    ├── settings.py
    ├── urls.py
    └── ...
```

---

## Setup Instructions

1. **Clone the repository**

    ```sh
    git clone <your-repo-url>
    cd "Twitter Clone Django/ujnews"
    ```

2. **Create and activate a virtual environment**

    ```sh
    python -m venv .venv
    .venv\Scripts\activate
    ```

3. **Install dependencies**

    ```sh
    pip install django
    ```

4. **Apply migrations**

    ```sh
    python manage.py migrate
    ```

5. **Create a superuser (optional, for admin access)**

    ```sh
    python manage.py createsuperuser
    ```

6. **Run the development server**

    ```sh
    python manage.py runserver
    ```

7. **Access the app**

    - Visit [http://127.0.0.1:8000/tweet/](http://127.0.0.1:8000/tweet/) to use UJTweet.

---

## Usage

- **Register:** Go to `/tweet/register/` to create a new account.
- **Login/Logout:** Use `/accounts/login/` and `/accounts/logout/`.
- **Create Tweet:** Click "Create a tweet" after logging in.
- **Edit/Delete:** Only available for your own tweets.
- **Search:** Use the search box to filter tweets by content.

---

## License

This project is for educational purposes.

---

## Credits

Developed by Ujwal.
