# BigDataTweetSentimentAnalysis

from pyhive import hive

    import pandas as pd

    #Create Hive connection 

    conn = hive.Connection(host="127.0.0.1", port=10000, username="username")

    # Read Hive table and Create pandas dataframe

    df = pd.read_sql("SELECT * FROM db_Name.table_Name limit 10", conn)

    print(df.head())
