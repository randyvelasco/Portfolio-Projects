This project leverages the power of Apache Kafka as a distributed streaming platform to ingest
and process real-time stock market data. The seamless integration of Python for data
manipulation and AWS services such as Glue, Athena, and SQL for data transformation and
analysis enhances the project's scalability, efficiency, and accessibility. 

<img width="893" alt="image" src="https://github.com/randyvelasco/Portfolio-Projects/assets/124484712/e55ad01f-bce4-4e4e-a54b-68d9093f61d2">


The workflow commences with the generation of a stock market data stream to simulate API
behavior. This process utilizes a CSV file containing stock market data. Subsequently, a Python
script is executed every second to randomly capture a single data row from the CSV. The
captured data is then transmitted to Apache Kafka through a broker and producer, ultimately
being published to a specific topic.

The data is consumed by a consumer and subsequently stored in JSON format on Amazon S3.
Amazon Glue undertakes data cataloging tasks using a crawler, organizing and cataloging the
data before saving it in a database. Amazon Athena is then employed to execute SQL queries,
ensuring the accuracy of the entire workflow process.

Please read the accompanying documentation for the steps undertaken.


Thanks.
