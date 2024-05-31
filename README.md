<<<<<<< HEAD
# Covid-19 India

Given two files `app.js` and a database file `covid19India.db` consisting of two tables `state` and `district`.

Write APIs to perform CRUD operations on the tables `state`, `district` containing the following columns,

**State Table**

| Columns    | Type    |
| ---------- | ------- |
| state_id   | INTEGER |
| state_name | TEXT    |
| population | INTEGER |

**District Table**

| Columns       | Type    |
| ------------- | ------- |
| district_id   | INTEGER |
| district_name | TEXT    |
| state_id      | INTEGER |
| cases         | INTEGER |
| cured         | INTEGER |
| active        | INTEGER |
| deaths        | INTEGER |

### API 1

#### Path: `/states/`
=======
<<<<<<< HEAD
# Movies

Given two files `app.js` and a database file `moviesData.db` consisting of two tables `movie` and `director`.

Write APIs to perform CRUD operations on the tables `movie`, `director` containing the following columns,

**Movie Table**

| Columns     | Type    |
| ----------- | ------- |
| movie_id    | INTEGER |
| director_id | INTEGER |
| movie_name  | TEXT    |
| lead_actor  | TEXT    |

**Director Table**

| Columns       | Type    |
| ------------- | ------- |
| director_id   | INTEGER |
| director_name | TEXT    |

### API 1

#### Path: `/movies/`
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Method: `GET`

#### Description:

<<<<<<< HEAD
Returns a list of all states in the state table
=======
Returns a list of all movie names in the movie table
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Response

```
[
  {
<<<<<<< HEAD
    stateId: 1,
    stateName: "Andaman and Nicobar Islands",
    population: 380581
=======
    movieName: "Captain America: The First Avenger",
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e
  },

  ...
]
```

### API 2

<<<<<<< HEAD
#### Path: `/states/:stateId/`

#### Method: `GET`

#### Description:

Returns a state based on the state ID

#### Response

```
{
  stateId: 8,
  stateName: "Delhi",
  population: 16787941
}
```

### API 3

#### Path: `/districts/`
=======
#### Path: `/movies/`
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Method: `POST`

#### Description:

<<<<<<< HEAD
Create a district in the district table, `district_id` is auto-incremented
=======
Creates a new movie in the movie table. `movie_id` is auto-incremented
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Request

```
{
<<<<<<< HEAD
  "districtName": "Bagalkot",
  "stateId": 3,
  "cases": 2323,
  "cured": 2000,
  "active": 315,
  "deaths": 8
=======
  "directorId": 6,
  "movieName": "Jurassic Park",
  "leadActor": "Jeff Goldblum"
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e
}
```

#### Response

```
<<<<<<< HEAD
District Successfully Added
```

### API 4

#### Path: `/districts/:districtId/`
=======
Movie Successfully Added
```

### API 3

#### Path: `/movies/:movieId/`
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Method: `GET`

#### Description:

<<<<<<< HEAD
Returns a district based on the district ID
=======
Returns a movie based on the movie ID
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Response

```
{
<<<<<<< HEAD
  districtId: 322,
  districtName: "Haveri",
  stateId: 36,
  cases: 2816,
  cured: 2424,
  active: 172,
  deaths: 220,
}
```

### API 5

#### Path: `/districts/:districtId/`

#### Method: `DELETE`

#### Description:

Deletes a district from the district table based on the district ID
=======
  movieId: 12,
  directorId: 3,
  movieName: "The Lord of the Rings",
  leadActor: "Elijah Wood",
}
```

### API 4

#### Path: `/movies/:movieId/`

#### Method: `PUT`

#### Description:

Updates the details of a movie in the movie table based on the movie ID

#### Request

```
{
  "directorId": 24,
  "movieName": "Thor",
  "leadActor": "Christopher Hemsworth"
}
```
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Response

```
<<<<<<< HEAD
District Removed

```

### API 6

#### Path: `/districts/:districtId/`

#### Method: `PUT`

#### Description:

Updates the details of a specific district based on the district ID

#### Request

```
{
  "districtName": "Nadia",
  "stateId": 3,
  "cases": 9628,
  "cured": 6524,
  "active": 3000,
  "deaths": 104
}
```
=======
Movie Details Updated

```

### API 5

#### Path: `/movies/:movieId/`

#### Method: `DELETE`

#### Description:

Deletes a movie from the movie table based on the movie ID
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Response

```
<<<<<<< HEAD

District Details Updated

```

### API 7

#### Path: `/states/:stateId/stats/`
=======
Movie Removed
```

### API 6

#### Path: `/directors/`
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Method: `GET`

#### Description:

<<<<<<< HEAD
Returns the statistics of total cases, cured, active, deaths of a specific state based on state ID
=======
Returns a list of all directors in the director table
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Response

```
<<<<<<< HEAD
{
  totalCases: 724355,
  totalCured: 615324,
  totalActive: 99254,
  totalDeaths: 9777
}

```

### API 8

#### Path: `/districts/:districtId/details/`
=======
[
  {
    directorId: 1,
    directorName: "Joe Johnston",
  },

  ...
]
```

### API 7

#### Path: `/directors/:directorId/movies/`
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Method: `GET`

#### Description:

<<<<<<< HEAD
Returns an object containing the state name of a district based on the district ID
=======
Returns a list of all movie names directed by a specific director
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e

#### Response

```
<<<<<<< HEAD

{
  stateName: "Maharashtra"
}

=======
[
  {
    movieName: "Captain Marvel",
  },

  ...
]
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e
```

<br/>

Use `npm install` to install the packages.

**Export the express instance using the default export syntax.**

**Use Common JS module syntax.**
<<<<<<< HEAD
=======
=======
# Node.js-5
Node.js Coding Practice 5 [MOVIES]
>>>>>>> ad78d021bd1509fabcfc9c5845456167e8a5ecd0
>>>>>>> d4993d65fabec7e84ed8e0c43e0e8ebd1f9dc36e
