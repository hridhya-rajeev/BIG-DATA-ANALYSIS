# BIG-DATA-ANALYSIS
# COMPANY: CODTECH IT SOLUTIONS
# NAME: HRIDHYA ABHINA RAJEEVAN
# INTERN ID: CT04DH2665
# DOMAIN: DATA ANALYTICS
# DURATION: 1 MONTH
# description: 
The given task focuses on demonstrating the process of working with PySpark to load, explore, and analyze a dataset related to air travel statistics. The primary goal of this implementation is to show how PySpark can efficiently handle structured data, starting from downloading the dataset to performing basic exploration and analysis. The task is divided into a series of well-defined steps to ensure clarity and reproducibility.

The process begins with the installation of the PySpark library. PySpark is the Python API for Apache Spark, which is a powerful open-source framework designed for distributed data processing. By running the command to install PySpark, the environment is prepared to execute Spark commands from within Python. This step ensures that all the necessary dependencies and configurations are in place before any data processing takes place.

Next, a Spark session is created. The SparkSession object serves as the entry point to programming Spark with the Dataset and DataFrame API. In this case, the session is created with the application name "PySparkDataLoad". This step is critical because it initializes the Spark runtime, enabling the program to perform distributed data operations. Without creating a Spark session, no interaction with Spark’s DataFrame API would be possible.

The third step involves downloading the dataset. A CSV file named airtravel.csv is retrieved from a public URL using Python’s urllib.request module. This file contains monthly air travel data, including passenger numbers for different months and years. Storing the file locally ensures that Spark can directly access and read the file without relying on a live network connection after the initial download.

Once the dataset is available locally, it is loaded into a Spark DataFrame using the spark.read.csv() function. The parameters header=True and inferSchema=True are used to make the loading process more efficient and intuitive. header=True ensures that the first row of the CSV file is treated as column names, while inferSchema=True automatically detects the appropriate data types for each column. The use of a DataFrame provides a tabular structure similar to a relational database table, making it easier to manipulate and query the dataset.

After loading the dataset, the program displays the schema using the printSchema() method. This step is crucial for understanding the structure of the dataset, including the names of the columns and their respective data types. Knowing the schema helps in planning the subsequent analysis and transformations.

The next operation is to display the first five rows of the DataFrame using the show(5) method. This gives a quick preview of the data, allowing the user to verify that it has been loaded correctly and that the column headers and values appear as expected. This kind of preview is often the first step in exploratory data analysis.

Following this, summary statistics are generated using the describe() method, which provides basic descriptive analytics such as count, mean, standard deviation, minimum, and maximum for each numerical column. Displaying these statistics is an important step in understanding the distribution, range, and central tendencies of the dataset.

Finally, the Spark session is stopped using the spark.stop() command. Properly stopping the Spark session is a good practice, as it releases the resources used by the application and ensures that the Spark environment is cleanly shut down.

In summary, this task walks through the complete process of working with a dataset in PySpark—from setup and data loading to exploration and analysis. The steps outlined here form a strong foundation for further data processing, transformations, and advanced analytics using Spark’s powerful distributed computing capabilities. The same methodology can be applied to larger and more complex datasets, making PySpark a valuable tool for handling big data in various real-world applications.


# OUTPUT:
![Image](https://github.com/user-attachments/assets/2de809e5-6b75-4d75-9045-0c1ac600685c)
