#Item Catalog Application - Udacity Nanodegree Project 4

## About
This project is a RESTful web application utilizing the Flask framework which accesses a SQL database that populates categories and their items.
OAuth2 provides authentication for further CRUD functionality on the application. Currently OAuth2 is implemented for Google Accounts.

### Pre-Requirements
- Python 2.7
- [Vagrant](https://www.vagrantup.com/)
- [Udacity Vagrantfile](https://github.com/udacity/fullstack-nanodegree-vm)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## Setup
1. Install Vagrant & VirtualBox
2. Clone the Udacity Vagrantfile
3. Go to Vagrant directory and either clone this repo or download and place zip here
4. Launch the Vagrant VM (`vagrant up`)
5. Log into Vagrant VM (`vagrant ssh`)
6. Navigate to `cd/vagrant` as instructed in terminal
7. Setup application database run `python database_setup.py`
8. Insert initial data `python lotsofmenus.py`
9. Run application using `python application.py`
10. Access the application locally using http://localhost:5000


## JSON endpoints
#### Returns JSON of all restaurants

```
/restaurants/JSON
```
#### Returns JSON of specific menu item

```
/restaurants/<int:restaurant_id>/menu/<int:menu_id>/JSON
```
#### Returns JSON of menu

```
/restaurants/<int:restaurant_id>/menu/JSON
```

### To debug:
- If the Login and Gdisconnect doesn't reflect correct login status of the user, empty your web browser's cache and run the application again.
