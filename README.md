## Marvel Database Character and Comic Count Retrieval through Marvel Comic API

### About Marvel Comic API
The Marvel Comics API is a RESTful service which provides methods for accessing specific resources at canonical URLs and for searching and filtering sets of resources by various criteria. All representations are encoded as JSON objects.
It allows developers everywhere to access information about Marvel's vast library of comics—from what's coming up, to 70 years ago.
The API can be accessed via https://developer.marvel.com/docs

### Accessing Marvel API
To access Marvel API, you have to sign up at the Marvel developer portal https://developer.marvel.com/. This gives you access to an API key that will help consume the data in the Marvel Database.

Upon signing up, You will be given a private key and public key. This is private to you and will be needed to sign requests when API calls are made to the database. The API calls are capped at a limit of 3000calls/day (i.e the max number of calls your application can make per day).

### Marvel Database Resources
You can access six resource types using the API:

    1.Comics: individual print and digital comic issues, collections and graphic novels. For example: Amazing Fantasy #15.
    2.Comic series: sequentially numbered (well, mostly sequentially numbered) groups comics with the same title. For example, Uncanny X-Men.
    3.Comic stories: indivisible, reusable components of comics. For example, the cover from Amazing Fantasy #15 or the origin of Spider-Man story from that comic.
    4.Comic events and crossovers: big, universe-altering storylines. For example, Infinity
    5.Creators: women, men and organizations who create comics. For example, Jack Kirby.
    6.Characters: the women, men, organizations, alien species, deities, animals, non-corporeal entities, trans-dimensional manifestations, abstract personifications, and green amorphous blobs which occupy the Marvel Universe (and various alternate universes, timelines and altered realities therein). For example, Spider-Man.
All the entity types are described in detail here https://developer.marvel.com/documentation/entity_types

### Project Objective

In this project, we aim to retrieve all characters and the quantity of comics in which they appear using the Marvel API key and render our result in and organised table format using python.

The character names and comic information are in Json format and can be accessed at: GET/v1/public/characters and  GET/v1/public/comics repectively

### Illustration on how the task was carried out

The basic steps carried out in this project are outlined as follows:

![Marvel%20datatask%20Story.png](attachment:Marvel%20datatask%20Story.png)

### Using Marvel Wrapper

The Marvel API wrapper https://pypi.org/project/marvel/ was used to render contents on the marvel database in a more user freindly format and it enabled the interaction with database easier using the API keys.

To use the API wrapper in the python application, use *pip* to 
> pip install marvel

### Results

We retrieved a total of 1562 characters from the database and a total of 93753 comics associated with the characters.

### Tools
Python, Marvel API wrapper, Marvel Comic API, exclidraw.



#### References
1. General API Information https://developer.marvel.com/documentation/generalinfo#:~:text=The%20Marvel%20Comics%20API%20is%20a,representations%20are%20encoded%20as%20JSON%20objects.&text=The%20Marvel%20Comics%20API,encoded%20as%20JSON%20objects.&text=Comics%20API%20is%20a,representations%20are%20encoded%20as

2. Tool for rendering image 
https://excalidraw.com

3. Marvel API Wrapper
https://pypi.org/project/marvel/

