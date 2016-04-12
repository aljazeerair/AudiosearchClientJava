# Audiosearch Java Client for Android

Unofficial Java Android client for [Audiosearch API](https://audiosear.ch/api)

See the [docs](https://www.audiosear.ch/developer/)

OAuth credentials are available [here](https://www.audiosear.ch/oauth/applications)

Work in progress.

# Using the client
```java
Audiosearch client = new Audiosearch()
                    .setApplicationId(YOUR_APPLICATION_ID)
                    .setSecret(YOUR_SECRET_KEY)
                    .build();
```

## Get trending
```java
client.getTrending().execute().body();
```

## Search episodes
```java
client.searchEpisodes(67946).execute().body().getResults();
```

## Get episode details
```java
client.getEpisode(67946).execute().body();
```

# Dependencies
* OKhttp3
* Retrofit2
* Jackson

# Contribute
```shell
git commit -m "your awesome contribution"
```





