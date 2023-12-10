# YouTube Data Harvesting and Warehousing
Capstone Project Assigned by Guvi Institute.

 <img src="https://wallsdesk.com/wp-content/uploads/2016/06/YouTube-logo-png.png" width="10%" height="30%">

```
Streamlit application that allows users to access and analyze data from multiple YouTube channels.
```


 ## Features :
- [x] Able to input a YouTube channel ID and retrieve all the relevant data (Channel name, subscribers, total video count, playlist ID, video ID, likes,dislikes, comments of each video) using Google API.
  
- [x] Option avaialable to store the data in a MongoDB database as a data lake.

- [x]  Able to collect data for up to 10 different YouTube channels and store them in the data lake by clicking a upload button.
  
- [x]  Option available to select a channel name and migrate its data from the data lake to a SQL database as tables.

 - [x] Able to search and retrieve data from the SQL database using different search options, including joining tables to get channel details.

## Tools and libraries used for this project :

| Tool/Lib | Purpose |
| --- | --- |
| Python | Scripting,  to make requests to the API for retrieve datas. |
| MongoDB | To store the retrieved datas in a MongoDB data lake |
| MySQL | Migrate to a SQL data warehouse for converting as structured/tabular format. |
| Streamlit | Using Streamlit to create a simple UI where users can enter a YouTube channel ID, view the channel details, and select channels to migrate to the data warehouse. |
| Pandas | For EDA processes. |
| Plotly | Graphing library makes interactive, publication-quality graphs. |

## Approach :
```mermaid
graph TD;
   A[Input YouTube Channel ID] --> B(Get Channel Data)
    B --> C(Store Data in MongoDB)
    C --> D[Upload to MongoDB]
    D --> E(Select Channel for Migration)
    E --> F(Migrate Data to SQL)
    F --> G(Search and Retrieve Data from SQL)
    G --> H(Display Data in Streamlit UI)
```

    A[Input YouTube Channel ID] --> B(Get Channel Data)
    B --> C(Store Data in MongoDB)
    C --> D[Upload to MongoDB]
    D --> E(Select Channel for Migration)
    E --> F(Migrate Data to SQL)
    F --> G(Search and Retrieve Data from SQL)
    G --> H(Display Data in Streamlit UI)


## User Interface 
__Home Page__

> About this Application and benefits of Youtube data harvesting

![Screenshot]()



__Upload Page__

> Upload Youtube channel's Identity Document to retrieve datas and store it in a MongoDB database.

![Screenshot]([https://github.com/Binoth5/YOUTUBE-HARVESTING/blob/main/2023-12-11%20(1).png))



__Migrate Page__

> Insert the retrieved datas into SQL Data Warehouse 

![Screenshot](https://github.com/your-username/repository-name/image-folder/screenshot.png)



__Analysis Page__

> Select the Questions to insights of youtube channels

![Screenshot](https://github.com/your-username/repository-name/image-folder/screenshot.png)




## Conclusion
> This project aims to develop a user-friendly Streamlit application that utilizes the
Google API to extract information on a YouTube channel, stores it in a MongoDB
database, migrates it to a SQL data warehouse, and enables users to search for
channel details and join tables to view data in the Streamlit app.
