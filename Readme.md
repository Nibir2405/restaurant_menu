# Restaurant Menu Django Project

This is a Django-based web application for managing and displaying a restaurant's menu. It allows users to view menu items categorized by meal type, see details for each item, and provides an admin interface for managing menu items.

## Features

- List menu items grouped by meal type (Starters, Salads, Main Dishes, Desserts)
- Show item details including description, price, and availability
- Admin interface for adding, editing, and removing menu items
- User authentication for menu item authorship
- Responsive design using Bootstrap

## Project Structure

```
mysite/
    settings.py
    urls.py
restaurant_menu/
    models.py
    views.py
    urls.py
    admin.py
    migrations/
templates/
    base.html
    index.html
    menu_item_detail.html
manage.py
db.sqlite3
```

## Getting Started

### Prerequisites

- Python 3.10+
- Django 5.2.1

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/Nibir2405/restaurant_menu.git
    cd restaurant_menu
    ```

2. Install dependencies:
    ```sh
    pip install django
    ```

3. Apply migrations:
    ```sh
    python manage.py migrate
    ```

4. Create a superuser for admin access:
    ```sh
    python manage.py createsuperuser
    ```

5. Run the development server:
    ```sh
    python manage.py runserver
    ```

6. Access the app at [http://127.0.0.1:8000/](http://127.0.0.1:8000/) and the admin at [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/)

## Usage

- The home page lists menu items by category.
- Click on a menu item to view its details.
- Log in to the admin interface to manage menu items.

## Models

- [`restaurant_menu.models.Item`](restaurant_menu/models.py): Represents a menu item with fields for meal name, description, price, meal type, author, status, and timestamps.

## Templates

- [`templates/base.html`](templates/base.html): Base template with navigation.
- [`templates/index.html`](templates/index.html): Home page listing menu items.
- [`templates/menu_item_detail.html`](templates/menu_item_detail.html): Detail view for a menu item.

## License

This project is for educational purposes.
