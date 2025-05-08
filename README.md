create a database and open mongodb shell
![Screenshot (87)](https://github.com/user-attachments/assets/f460047f-3bc7-42b1-b92c-40bfa6280c19)

use drop collection (for collection)
![Screenshot (88)](https://github.com/user-attachments/assets/ab9b2585-78d6-4207-9724-f2d9ae8b090f)

for collection via shell
![Screenshot (91)](https://github.com/user-attachments/assets/a811c7aa-a3ff-4bde-a39e-3178e7ff6ad8)

refresh
![Screenshot (92)](https://github.com/user-attachments/assets/24681a69-063e-425f-8a39-1504185032d4)

to delete database
![Screenshot (89)](https://github.com/user-attachments/assets/6bb8b71a-df74-4cd3-97c8-939867d0bfde)

refreah
![Screenshot (90)](https://github.com/user-attachments/assets/abf732d5-114f-46c5-9c4b-02fd548f72cf)

insert documents
![Screenshot (93)](https://github.com/user-attachments/assets/c948edfa-ca71-4deb-9269-2ab2c95dd956)
![Screenshot (94)](https://github.com/user-attachments/assets/1c1cbcad-4e2e-4c5c-bec3-85aa39ef5748)
![Screenshot (95)](https://github.com/user-attachments/assets/b6d76f38-f1c7-412c-925d-6ec6e027ba06)
![Screenshot (96)](https://github.com/user-attachments/assets/45922600-2023-4609-b922-227cc2a9be6b)

delete one document
![Screenshot (97)](https://github.com/user-attachments/assets/8059a7d4-cc3e-4aca-be90-ae8660420de8)
![Screenshot (98)](https://github.com/user-attachments/assets/d47a4321-4a7f-4f9f-86eb-a5d1aaad550b)
![Screenshot (99)](https://github.com/user-attachments/assets/1d43a2b7-2975-4243-a601-bc31b0c031a2)

![Screenshot (101)](https://github.com/user-attachments/assets/80b89509-c65d-47ad-bff9-a5d926092156)

delete many documents(duration <=4)
![Screenshot (103)](https://github.com/user-attachments/assets/4f6ce7e1-ff9e-47cf-9832-5e5d8c66724b)
![Screenshot (104)](https://github.com/user-attachments/assets/96af9ea6-1e79-4efd-94d5-103c2d170d42)

update manually
![Screenshot (106)](https://github.com/user-attachments/assets/25ec0cf3-502c-4016-8246-7b02ef0711af)
![Screenshot (107)](https://github.com/user-attachments/assets/dd647760-6c9a-4682-88fd-6d20a27abe6d)

update via shell
![Screenshot (108)](https://github.com/user-attachments/assets/b3367623-b032-4661-8003-e4fb7c332fae)
![Screenshot (109)](https://github.com/user-attachments/assets/8ee5e55a-8a50-475e-a98d-4651b6b951ac)

find
![Screenshot (110)](https://github.com/user-attachments/assets/1dc5a8b8-2a95-4c95-8e74-c19fcd16c2b3)



.....................Questions & Answers......................


create a database bookshop

create a collection books

use bookshop
db.createCollection("books")

insert the following data
{
  "title": "The Hobbit",
  "author": "J.R.R. Tolkien",
  "published_year": 1937,
  "genres": ["Fantasy", "Adventure"],
  "pages": 310,
  "available": true,
  "rating": 4.8
}

  {
    "title": "1984",
    "author": "George Orwell",
    "published_year": 1949,
    "genres": ["Dystopian", "Political Fiction"],
    "pages": 328,
    "available": true,
    "rating": 4.7
  },
  {
    "title": "To Kill a Mockingbird",
    "author": "Harper Lee",
    "published_year": 1960,
    "genres": ["Southern Gothic", "Drama"],
    "pages": 281,
    "available": false,
    "rating": 4.6
  },
  {
    "title": "The Great Gatsby",
    "author": "F. Scott Fitzgerald",
    "published_year": 1925,
    "genres": ["Tragedy"],
    "pages": 180,
    "available": true,
    "rating": 4.4
  },
  {
    "title": "Brave New World",
    "author": "Aldous Huxley",
    "published_year": 1932,
    "genres": ["Science Fiction", "Dystopian"],
    "pages": 311,
    "available": true,
    "rating": 4.2
  }
  Ans:
  db.books.insertMany([
  {
    "title": "The Hobbit",
    "author": "J.R.R. Tolkien",
    "published_year": 1937,
    "genres": ["Fantasy", "Adventure"],
    "pages": 310,
    "available": true,
    "rating": 4.8
  },
  {
    "title": "1984",
    "author": "George Orwell",
    "published_year": 1949,
    "genres": ["Dystopian", "Political Fiction"],
    "pages": 328,
    "available": true,
    "rating": 4.7
  },
  {
    "title": "To Kill a Mockingbird",
    "author": "Harper Lee",
    "published_year": 1960,
    "genres": ["Southern Gothic", "Drama"],
    "pages": 281,
    "available": false,
    "rating": 4.6
  },
  {
    "title": "The Great Gatsby",
    "author": "F. Scott Fitzgerald",
    "published_year": 1925,
    "genres": ["Tragedy"],
    "pages": 180,
    "available": true,
    "rating": 4.4
  },
  {
    "title": "Brave New World",
    "author": "Aldous Huxley",
    "published_year": 1932,
    "genres": ["Science Fiction", "Dystopian"],
    "pages": 311,
    "available": true,
    "rating": 4.2
  }
])
![Screenshot (112)](https://github.com/user-attachments/assets/92f68d46-1b4d-46c2-9a9d-61446b58ccb1)
![Screenshot (113)](https://github.com/user-attachments/assets/e8f89be3-0659-4e1e-ac1c-80fad5fc1337)

  
Find all books
db.books.find()
![Screenshot (114)](https://github.com/user-attachments/assets/07327edc-b1f5-4587-b29e-5dae5cacfeb1)
![Screenshot (115)](https://github.com/user-attachments/assets/af093336-d78d-4170-ac4a-e497a88dbcf8)
![Screenshot (116)](https://github.com/user-attachments/assets/597cb8b7-c70b-4522-a112-5f8802230778)


Find all books published after 1950
db.books.find({published_year:{$gt:1950}})
![Screenshot (117)](https://github.com/user-attachments/assets/89688ef9-7c50-4e43-8561-8bda5a1928b3)

Find the avilable books
db.books.find({available:true})
![Screenshot (117)](https://github.com/user-attachments/assets/c01da6bd-feea-42ee-9e43-619ff20c676d)
![Screenshot (118)](https://github.com/user-attachments/assets/a70e668f-dd6f-486e-80be-20cf80b8a247)
![Screenshot (119)](https://github.com/user-attachments/assets/0f5fe91f-5225-428d-8865-89383d39f95d)

Find all books that belong to the "Dystopian" genre\
db.books.find({genres:"Dystopian"})
![Screenshot (120)](https://github.com/user-attachments/assets/a425abd7-0e99-4f91-a203-3c4f8257429c)
![Screenshot (121)](https://github.com/user-attachments/assets/1ef30301-0283-4c58-912b-29fae25da885)

Find the books which published after 1960 and had rating more than 4.0
db.books.find({published_year:{$gt:1950},rating:{$gt:4.0}})
![Screenshot (121)](https://github.com/user-attachments/assets/4da52e42-2d03-4ebb-b7c9-c0f035d729b0)

Project only title and author fields:
db.books.find({}, { title: 1, author: 1, _id: 0 })
![1](https://github.com/user-attachments/assets/ca725a28-3fce-4c1e-bbb3-684fa41eab77)
![2](https://github.com/user-attachments/assets/5ae62757-35b8-4367-8466-020d72f26eea)

Update the book "1984" to set available: false:
db.books.updateOne(
  { title: "1984" },
  { $set: { available: false } }
)
![2](https://github.com/user-attachments/assets/0ec2201c-1dcd-448d-a55d-c687f84d03fe)

Increase the rating of "Brave New World" by +0.1:
db.books.updateOne(
  { title: "Brave New World" },
  { $inc: { rating: 0.1 } }
)
![3](https://github.com/user-attachments/assets/72c3784b-7cd7-4a48-a0c2-041085bdc48d)

Add a new genre "Classic" to "The Great Gatsby":
db.books.updateOne(
  { title: "The Great Gatsby" },
  { $addToSet: { genres: "Classic" } }
)
![3](https://github.com/user-attachments/assets/47017043-9a63-4afe-9147-8d9f65f6f9b1)

Sort books by published_year ascending:
db.books.find().sort({ published_year: 1 })
![4](https://github.com/user-attachments/assets/24019725-626a-4363-8cc3-b43e56509268)
![5](https://github.com/user-attachments/assets/6797fbb0-b5b5-4be6-87a4-79f56da927f4)

Sort books by rating descending:
db.books.find().sort({ rating: -1 })
![6](https://github.com/user-attachments/assets/8b29c161-d92f-4f27-b872-45d87e569717)
![7](https://github.com/user-attachments/assets/d9e07356-4f7f-4a42-a3bf-155d65c6de95)
![8](https://github.com/user-attachments/assets/d1dd1f05-8bce-42f4-993e-f4cb700b837b)
![9](https://github.com/user-attachments/assets/0bd6a94e-4017-4174-bd81-7c00010e6ba0)

Delete all books with a rating lower than 4.5:
db.books.deleteMany({ rating: { $lt: 4.5 } })
![9](https://github.com/user-attachments/assets/18e83b68-30bc-4fa0-9a57-f21ae918794d)

 




