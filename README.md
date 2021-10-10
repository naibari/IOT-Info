# The Internet of Things (IoT)
Describes physical objects (or groups of such objects) that are embedded with sensors, processing ability, software, and other technologies, and that connect and exchange data with other devices and systems over the Internet or other communications networks.



## Below are some examples of how IoT impacts our daily lives

### 1. Home Security
The Internet of Things is the key driver behind a completely smart and secure home. IoT connects a variety of sensors, alarms, cameras, lights, and microphones to provide 24/7/365 security—all of which can be controlled from a smart phone. For example, the Ring doorbell camera security system allows users to see, hear, and speak to visitors at their door via a computer, tablet, or mobile phone.

### 2. Activity Trackers
These sensor devices are designed to be worn during the day to monitor and transmit key health indicators in real time, such as fatigue, appetite, physical movement, oxygen levels, blood pressure, fall detection, and compliance with taking medicine. At-home health monitoring reduces the number of emergency doctor or hospital visits and helps elderly or disabled people live more independent lives.

### 3. Digital Twins
In the manufacturing world, a digital twin is essentially an identical digital copy of a physical object. Using technologies including IoT, artificial intelligence, and machine learning, the digital twin can update itself as the physical object changes in response to its surrounding conditions. Engineers can use the digital twin, instead of the actual physical object, to make adjustments or test updates. 

### 4. Self-Healing Machines
Relying on arrays of thousands of sensors, artificial intelligence, and machine learning, manufacturing equipment can be designed to recognize variances in its own operation, and correct them, before they turn into problems that require downtime and repair. This saves companies time and money and frees up employees who would normally monitor equipment and undertake maintenance to work on higher-level tasks.

### 5. Motion Detection
Using sensors to detect motion or vibration in large-scale structures such as buildings, bridges, and dams can identify the small disturbances and patterns that could lead to catastrophic failures. Networks of detectors are also used in areas susceptible to landslides, avalanches, and earthquakes.
* If you want to read more please go to [ASME](https://www.asme.org/topics-resources/content/10-best-iot-examples-in-2020).

# How to Install Django on Windows PowerShell:

## Introduction:
The Python ecosystem has a lot of web frameworks. One that has consistently been popular is the Django framework. It’s popular for being robust, secure, and allows developers to develop projects fast.
In this tutorial, you will learn how to install Django on Windows using pip. After that, you will verify the installation, create a project, and start a Django development server.
Before you install Django, you must make sure that Python is installed on your system.

## Step 1 — Opening PowerShell:
First, you need to open PowerShell on your computer. You can do that by searching for PowerShell in the Windows search box.

## Step 2 - Verifying Python Installation:
Before you install Django, first, you need to make sure that you installed Python on your system.
```sh
python -V
```
-V option logs the Python version installed on your system.

After running the command, you should see output like this:
```sh
PS C:\Users\Username> python -V
Python 3.9.7
```
## Step 3 - Upgrading Pip:
Python comes with pip by default. But most of the time, it comes with an old version. it’s always a good practice to upgrade pip to the latest version.

Enter the following command to upgrade pip on your system:
```sh
python -m pip install --upgrade pip
```
Now you’ve upgraded pip, you’ll create the project directory where you’ll install Django.

## Step 4 - Creating a Project Directory:
In this section, you will create a directory that will contain your Django application.
Create the directory using the mkdir command:
```sh
mkdir django_project
```
Move into the django_project directory using the cd command:
```sh
> cd django_project
```
Now that you’ve created the working directory for your project, you’ll create a virtual environment where you’ll install Django.

## Step 5 - Creating the Virtual Environment:
In this step, you’ll create a virtual environment for your project. A virtual environment is an isolated environment in Python where you can install the project dependencies without affecting other Python projects. This lets you create different projects that use different versions of Django.
To create a virtual environment, type the following command and wait for a few seconds:
```sh
> python -m venv venv
```
he command will create a directory called venv inside your project directory.

Next, confirm the venv directory has been created by listing the directory contents using the ls command:
```sh
> ls 
```
Now you’ve created the virtual environment directory, you’ll activate the environment.

## Step 6 - Activating the Virtual Environment:
Run the following command to activate the virtual environment:
```sh
> venv\Scripts\activate
```
After you run the command, you will see

a (venv) at the beginning of the prompt. This shows that the virtual environment is activated:
```sh
(venv) PS C:\Users\Stanley\Desktop\django_project>
```
If you face an error, follow this:
## Solution to “Running Scripts Is Disabled On This System” Error On PowerShell:
o fix the error, you need to change the PowerShell execution policy to remotesigned. This will allow you to run scripts that are on your local computer unsigned, and also remote scripts(from the internet) which have been signed.

Type the following command in the PowerShell admin window to change the execution policy:
```sh
> set-executionpolicy remotesigned
```
You will be prompted to accept the change, type A(Yes to all), and press ENTER on your keyboard to allow the change.

Now that you’ve activated the virtual environment for your project, the moment you’ve been waiting for is here. It’s time to install Django!

## Step 7 - Installing Django:
You will install Django on your system using pip.

Run the following command to install Django using pip install:
```sh
(venv)> pip install django
```
The command will install the latest version of Django. 

Once the installation finishes, you need to verify that Django has been installed. To do that, type the following command:
```sh
(venv)> django-admin --version
```
Now, You’ll begin to create a Django project.

## Step 8 - Creating the Django Project
You create a project by using the command-line utility django-admin that comes with Django. The command generates files where you can configure the settings for your database, add third-party packages for your project to mention a few.

Create the project using the django-admin startproject command:
```sh
(venv)> django-admin startproject test_project
```
Change into the test_project directory:
```sh
(venv)> cd test_project
```
Type the following command to see the contents in the project directory:
```sh
(venv)> ls test_project
```
## Step 9 - Running the Development Server:
Now that the project has been created, we will start the Django development server.

Start the development server using the manage.py runserver command:
```sh
(venv)> python manage.py runserver
```
Next, visit http://127.0.0.1:8000/ in your web browser. You should see the page.

To learn more, click [here](https://www.stanleyulili.com/django/how-to-install-django-on-windows/)
