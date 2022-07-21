# Author: Sirui Wu
# Time: 2021-12-5 16:59:01

How to run code:

Fisrtly, unzip the "thsis.zip"
1 Use terminal to enter the folder of ‘2 Code’, run 'pip install -r requirements.txt' to install necessary libraries for python.

2 Modify config.ini in the folder of '2 Code’, project_file_name is the folder containing fnirs, egg and vm.

3 Enter the folder of ‘2.3 DataVault’ to create datavault and tables. Run code:
    python Create_database.py
    python Create_tables_for_userdata.py
    python Create_tables_for_datavault.py

4 Enter the folder of ‘2.2 Staging Area Layer’ to process and insert data into datavualt. Run code:
    python Insert_VFC_into_datavault.py
    python  Insert_MP_into_datavault.py

5 Enter the folder of ‘2.4 Logic Layer(API)’, run following command in terminal:
    python manage.py makemigrations
    python manage.py migrate
    python manage.py runserver
  Then, you can visit website in http://127.0.0.1:8000
  Follow the Data Visualization Documentation in '2.5 technical documentation' to use the web.

6 Information Mart Layer are the files of html, included in the folder of ‘2.4 Logic Layer(API)’.

# For Testing.py, follow the instruction in report


