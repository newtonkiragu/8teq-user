# 8teq User Management System

## Description
A user management system with the following functionalities
 - User registration
 - Login
 - View user details
 - Change password
 - Logout

#### Link to deployed site
To be deployed
## Table of content
1. [Description](#description)
2. [API endpoints](#endpoints)
3. [Setup and installations](#setup-and-installations)
4. [Deployment](#deployment)
5. [Contributing](#contributing)
6. [Bugs](#bugs)
7. [Contact me](#support-and-contact-details)
8. [Licensing](#license)

## endpoints
API Endpoint | Description | Request
---- | :---- | :----- |
http://127.0.0.1:8000/api/signup | Create a new user account | POST
http://127.0.0.1:8000/api/api-auth/login/ | Login a user | POST
http://127.0.0.1:8000/api/user/id | View details of the new user account | GET
http://127.0.0.1:8000/api/change_password/<int:pk>/ | Reset password of a specific user | GET
http://127.0.0.1:8000/api/change_password/<int:pk>/ | Complete resetting password of a user | PUT
http://127.0.0.1:8000/api/api-auth/login/logout | Logout a specific user | DELETE

## Setup and installations

#### Prerequisites
1. [Python3.6](https://www.python.org/downloads/)
3. [virtualenv](https://virtualenv.pypa.io/en/stable/installation/)
4. [Pip](https://pip.pypa.io/en/stable/installing/)
5. [Django](https://www.djangoproject.com/download/)
5. [Django Rest Framework](http://www.django-rest-framework.org/#installation)

#### Technologies used
    - Python 3.6
    - Django, Django Rest Framework

#### Clone the Repo and checkout into the project folder.
```bash
git clone git@github.com:newtonkiragu/8teq-user.git && cd 8teq-user
```

#### Create and activate the virtual environment
```bash
python3.6 -m virtualenv virtual
```

```bash
source virtual/bin/activate
```

#### Setting up environment variables
Create a `.env` file and paste paste the following filling where appropriate:
```
MODE='dev'
DEBUG=True
DISABLE_COLLECTSTATIC=1
```

#### Install dependancies
Install dependancies that will create an environment for the app to run
`pip install -r requirements.txt`

#### Run migrations
```bash
python3.6 manage.py migrate
```

#### Run the app
```bash
python3.6 manage.py runserver
```
Open [localhost:8000](http://127.0.0.1:8000/api/)

## Deployment
To deploy the application, please follow the instructions in [this gist](https://gist.github.com/newtonkiragu/42f2500e56d9c2375a087233587eddd0)

## Contributing
Please read this [comprehensive guide](https://opensource.guide/how-to-contribute/) on how to contribute. Pull requests are welcome :-)

## Bugs
[Create an issue](https://github.com/newtonkiragu/8teq-user/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) mentioning the bug you have found

#### Known bugs
 - none yet

#### Feature request
[Create an issue](https://github.com/newtonkiragu/8teq-user/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) mentioning the feature you would like implemented

## Support and contact details
Contact [Newton Karanu](karanunewton4@gmail.com) for further help/support

### License
MIT

