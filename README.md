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


## User Interface 
__Home Page__

> About this Application and benefits of Youtube data harvesting


![2023-12-11](https://github.com/Binoth5/YOUTUBE-HARVESTING/assets/153276019/f3321c1d-bcbc-444c-b57c-f0819d4b4b0b)

__Upload Page__

> Upload Youtube channel's Identity Document to retrieve datas and store it in a MongoDB database.


![2023-12-11 (1)](https://github.com/Binoth5/YOUTUBE-HARVESTING/assets/153276019/71a247a4-6663-4eb1-a2fd-b0ce940fbd67)



__Migrate Page__

> Insert the retrieved datas into SQL Data Warehouse 



![2023-12-11 (2)](https://github.com/Binoth5/YOUTUBE-HARVESTING/assets/153276019/03dbdbd0-4d5a-44de-808c-4e86b2fca1be)


__Analysis Page__

> Select the Questions to insights of youtube channels



![2023-12-11 (3)](https://github.com/Binoth5/YOUTUBE-HARVESTING/assets/153276019/03a00a6b-3bd4-44df-aaff-c7011e179844)



## Conclusion
> This project aims to develop a user-friendly Streamlit application that utilizes the
Google API to extract information on a YouTube channel, stores it in a MongoDB
database, migrates it to a SQL data warehouse, and enables users to search for
channel details and join tables to view data in the Streamlit app.
