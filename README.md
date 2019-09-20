# Head First Python. Paul Berry - Notes

## Functions and Modules - Standard library

Useful links:

- <http://pypi.python.org>
- <https://docs.python.org/3/library/index.html>

### 1. sys module

- sys.platform
- print(sys.version) - Python version

### 2. os module

- os.getcwd() - name of folder where the code is operating
- access system’s environment variables:
  - whole system

    ~~~python
    >>> os.environ
    environ({'ALLUSERSPROFILE': 'C:\\ProgramData', 'APPDATA': 'C:\\Users\\lenka\\AppData\\Roaming',
    'COMMONPROGRAMFILES': 'C:\\Program Files (x86)\\Common Files',
    'COMMONPROGRAMFILES(X86)': 'C:\\Program Files (x86)\\Common Files',
    'COMMONPROGRAMW6432': 'C:\\Program Files\\Common Files', 'COMPUTERNAME': 'ASUS-ZB-UX410UA',
    'COMSPEC': 'C:\\WINDOWS\\system32\\cmd.exe', 'DRIVERDATA': 'C:\\Windows\\System32\\Drivers\\DriverData',
    'FPS_BROWSER_APP_PROFILE_STRING': 'Internet Explorer', 'FPS_BROWSER_USER_PROFILE_STRING': 'Default'
    ~~~

  - individiual location

    ~~~python
    >>> os.getenv('APPDATA')
    'C:\\Users\\lenka\\AppData\\Roaming'
    ~~~

### 3. datetime module

- date.today()

~~~python
>>> import datetime
>>> datetime.date.today()
datetime.date(2019, 5, 29)
~~~

- separetely

~~~python
>>> datetime.date.today().day
29
>>> datetime.date.today().month
5
>>> datetime.date.today().year
2019
~~~

- date.isoformat

~~~python
>>> datetime.date.isoformat(datetime.date.today())
'2019-05-29'
~~~

### 4. time module

- 24-hours format

~~~python
>>> import time
>>> time.strftime("%H:%M")
'22:46'
~~~

- AM vs. PM

~~~python
>>> time.strftime("%A %p")
'Wednesday PM'
~~~

~~~python
>>> time.sleep(5)
takes 5 seconds to reapeare the >>> prompt

## Data Structures

### Lists []

Lists can contain *any* data of *any* type. Types can be even mixed.

## Operators

### Standard operators

such as +, -, *, /, >, <, > =, < =, and so on

### Super operators

in - returns True / False

## for loop

Three different ways of usage:
### 1. iterate over a list of numbers:
for i in [1,2,3]:
    print(i)
### 2. itarate over a string:
for i in'Hello':
    print(i)
### 3. using range:
for i in range(5):
    print('Blablabla')

## using help in prompt
>>>help(random.randint)

