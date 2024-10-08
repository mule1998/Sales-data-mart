Welcome to the show. This endeavor aims to provide you with insights into the functioning of projects within a real-time environment.

The code has been meticulously crafted with careful consideration for various aspects. It not only nurtures coding skills but also imparts a comprehensive comprehension of project structures.

Let's Start with the requirements to complete the projects:-
1. Require a laptop with a minimum of 4 GB of RAM, i3 and above (Better to have 8GB with i5).
2. Local setup of spark. This is tricky so keep all things intact to work it properly.Download python 3.10.11 instead of python3.6 or python3.9 
3. Install PyCharm in the system. 
4. MySQL workbench should also be installed on the system.
5. You should have an AWS account.

```plaintext
Project structure:-
my_project/
├── docs/
│   └── readme.md
├── resources/
│   ├── __init__.py
│   ├── dev/
│   │    ├── config.py
│   │    └── requirement.txt
│   └── qa/
│   │    ├── config.py
│   │    └── requirement.txt
│   └── prod/
│   │    ├── config.py
│   │    └── requirement.txt
│   ├── sql_scripts/
│   │    └── table_scripts.sql
├── src/
│   ├── main/
│   │    ├── __init__.py
│   │    └── delete/
│   │    │      ├── aws_delete.py
│   │    │      ├── database_delete.py
│   │    │      └── local_file_delete.py
│   │    └── download/
│   │    │      └── aws_file_download.py
│   │    └── move/
│   │    │      └── move_files.py
│   │    └── read/
│   │    │      ├── aws_read.py
│   │    │      └── database_read.py
│   │    └── transformations/
│   │    │      └── jobs/
│   │    │      │     ├── customer_mart_sql_transform_write.py
│   │    │      │     ├── dimension_tables_join.py
│   │    │      │     ├── main.py
│   │    │      │     └──sales_mart_sql_transform_write.py
│   │    └── upload/
│   │    │      └── upload_to_s3.py
│   │    └── utility/
│   │    │      ├── encrypt_decrypt.py
│   │    │      ├── logging_config.py
│   │    │      ├── s3_client_object.py
│   │    │      ├── spark_session.py
│   │    │      └── my_sql_session.py
│   │    └── write/
│   │    │      ├── database_write.py
│   │    │      └── parquet_write.py
│   ├── test/
│   │    ├── scratch_pad.py.py
│   │    └── generate_csv_data.py
```

How to run the program in Pycharm:-
1. Open the pycharm editor.
2. Upload or pull the project from GitHub.
3. Open the terminal from the bottom pane.
4. Goto virtual environment and activate it. Let's say you have Venv as a virtual environment.i) cd venv ii) cd Scripts iii) activate (if activate doesn't work then use ./activate)
5. Need user on AWS, assign S3 full access, and provide the secret key and access key to the config file.
6. Run main.py from the green play button on the top right-hand side.


