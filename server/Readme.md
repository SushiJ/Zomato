## API Planning

- Auth (Authenticating the user and creating the user in the database)
- Food (Food Items and their details)
- Restaurant (Restaurants and their details)
- Menu (Menu and its details ) Adding new Menu, updating Menu
- Order (Order and its details)
- Payments (Payments and its details)
- Reviews (Reviews and its details)
- User (User and its details)
- Images (Images and its details)
- Mail (Mail and its details)

Hashing and Salting

you enter a password = 123456
first step is Hashing; sdfasd324sdsdvask34h423*&^*743jdngjkk3457i
second step is Salting(10); sdfasd324sdsdvask34h423*&^*743jdngjkk3457i$%^&\*(

## Database Model

### Restaurant 
<pre>[
  "name": "", 
  "city": "",
  "address": "",
  "mapLocation": "",
  "cuisine": ["", ""],
  "restaurantTimings": "",
  "contactNumber": "",
  "website": "",
  "popularDishes": ["", ""],
  "averageCost": 300,
  "amenties": ["", ""],
  "menuImages": referencing => Images Collecion document,
  "menu": references => Menu Collection document,
  "reviews": ["references => Reviews Collection document", "references => Reviews Collection document"],
  "photos": references => Images Collection document
]</pre>

### Menu
<pre>
menus: [
  {
    name: "",
    items: [
       references => Food Collection document,
    ]
  }
],
"recommended": [
  "references => Food Collection document"
]
</pre>


