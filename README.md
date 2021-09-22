# SwiftScore

###Screenshots
<p align="left">
<img src="/images/upcomingmatches.png" width="30%"/> 
<img src="/images/pastscores.png" width="30%"/> 
<img src="/images/leaguetable.png" width="30%"/>
<img src="/images/topscorers.png" width="30%"/>
<img src="https://user-images.githubusercontent.com/72180010/132879117-fa102f6c-8280-45e8-a244-f7d048ccf693.gif" width="30%"/>
</p>

---

### Table of Contents

- [Description](#description)
- [Dependencies](#dependencies)
- [API Reference](#api-reference)
- [Lessons Learnt](#lesssons-learnt)
- [Contributing](#contributing)
- [Roadmap](#roadmap)
- [Google Playstore](google-playstore)
- [License](#license)
- [Author Info](author-info)

---

## Description

* A football stats and live-score app built with Kotlin,MVVM architecture,Retrofit, Coroutines and Navigation Components
* A user can select a league they want to view the league table, top scorers and also be updated on the live-scores in realtime
* User can be able to select to see upcoming matches for a given day
* Project was completed with MVVM architecture and following android app architecture using Retrofit , Coroutines and Navigation components

###Dependencies
* Coroutines
* Retrofit
* Navigation components
* Glide
* GlideVectorYou

### API Reference

#### Get upcoming matches

```https
  GET /api/v1/soccer/matches
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `apiKey` | `string` | **Required**. Your API key |
| `seasonId` | `string` | **Required**.League Id e.g Premier League|
| `dateFrom` | `string` | **Required**.|
| `dateTo` | `string` | **Required**.|

#### Get League Table

```https
  GET /api/v1/json/1/lookuptable.php
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `l`      | `string` | **Required**. League Id e.g 1980 for Premier League |
| `s`      | `string` | **Required**. League Season Id e.g 2021-2022 |

#### Get Top Scorers

```https
  GET /api/v1/soccer/topscorers
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `l`      | `string` | **Required**. League Id e.g 1980 for Premier League |
| `s`      | `string` | **Required**. League Season Id e.g 2021-2022 |



### Lesssons Learnt

- Always perform heavy tasks like local database and network operations on the background thread. This is to prevent blocking the main thread, I used Retrofit for network operation in support of Coroutines to perform the task in the background thread.

- Navigation components made it easy for me to build my app's navigation system. Learnt best practices like having one activity and multiple fragments that can be swaped in and out of the fragment container, this improved app responsiveness since fragments are lightweight

- Learnt how to create UI designs on Figma this really came in handy since without me knowing I was always thinking on the architecture of the app and how the data will flow

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Roadmap
```
  Intergrate offline caching using Room local database​
34
```https
35
  GET /api/v1/soccer/matches
36
```
37
​
38
| Parameter | Type     | Description                |
39
| :-------- | :------- | :------------------------- |
40
| `apiKey` | `string` | **Required**. Your API key |
41
| `seasonId` | `string` | **Required**.League Id e.g Premier League|
42
| `dateFrom` | `string` | **Required**.|
43
| `dateTo` | `string` | **Required**.|
44
​
45
#### Get League Table
46
​
47
```https
48
  GET /api/v1/json/1/lookuptable.php
49
```
50
​
51
| Parameter | Type     | Description                       |
52
| :-------- | :------- | :-------------------------------- |
53
| `l`      | `string` | **Required**. League Id e.g 1980 for Premier League |
54
| `s`      | `string` | **Required**. League Season Id e.g 2021-2022 |
55
​
56
#### Get Top Scorers
57
​
58
```https
59
  GET /api/v1/soccer/topscorers
60
```
61
​
62
| Parameter | Type     | Description                       |
63
| :-------- | :------- | :-------------------------------- |
64
| `l`      | `string` | **Required**. League Id e.g 1980 for Premier League |
65
| `s`      | `string` | **Required**. League Season Id e.g 2021-2022 |
66
​
67
## Lesssons Learnt
68
​
69
- Always perform heavy tasks like local database and network operations on the background thread. This is to prevent blocking the main thread, I used Retrofit for network operation in support of Coroutines to perform the task in the background thread.
70
​
71
- Navigation components made it easy for me to build my app's navigation system. Learnt best practices like having one activity and multiple fragments that can be swaped in and out of the fragment container, this improved app responsiveness since fragments are lightweight
72
​
73
- Learnt how to create UI designs on Figma this really came in handy since without me knowing I was always thinking on the architecture of the app and how the data will flow
74
​
75
## Contributing
76
​
77
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
78
​
79
1. Fork the Project
80
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
81
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
82
4. Push to the Branch (`git push origin feature/AmazingFeature`)
83
5. Open a Pull Request
84
​
85
## Roadmap
```
```
  Add multiple leagues like La Liga, Serie A(Ligue 1 now intergrated in version 1.1.1)
```

## Google Playstore

<p align="left">
    <a href="https://play.google.com/store/apps/details?id=com.swift.swiftscore">
        <img src="/images/googleplaylogo.png" width="40%" height="40%"/>
    </a>
</p>

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Author Info

- Twitter - [@BreensR](https://twitter.com/BreensR)
- Linkedin - [LinkedIn: Breens Mbaka](https://www.linkedin.com/in/breens-mbaka-b447781b9/)

