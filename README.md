# ETL_Tik_Tok_Trend

## Team Members:
- Emily Hurst
- Mary Thissen
- Hanna Lakew
- Victor Diaz
- Gus Thanasuwandithee

## Data sets: 
- Tik Tok Trending Tracks: https://www.kaggle.com/yamqwe/tiktok-trending-tracks 
- Tik Tok Trending Videos: https://www.kaggle.com/erikvdven/tiktok-trending-december-2020 
- Billboard Hot 100 Songs: https://www.kaggle.com/dhruvildave/billboard-the-hot-100-songs

## Why we chose these data sets: 
### Tik Tok has become a worldwide sensation and our group was interested in learning more about it's impact on the music industry. We planned to discover a relationship between the video trends and and how it relates to top music charts.

## Proposed Methodology:
### Use Pandas to load in csv files in order to: 
- Join data (our chosen data sets)
- Clean data (drop null rows, etc)
- Filter data (possibly by artist names and song title)

## Data Utilized:
### Data Definitions: 
### Source: https://developer.spotify.com/documentation/web-api/reference/#/operations/get-several-audio-features
- track_id: Tiktok refernce key for the individual songs.
- track_name: Title of the song.
- artist_name: Name of the artist.
- release_date: The day the song was released to the public.
- popularity: Tiktok popularity - The popularity of a Tiktok audio. The value will be between 0 and 100, with 100 being the most popular.
The popularity of a song is a value between 0 and 100, with 100 being the most popular. The popularity is calculated by the sum of likes, comments, shares, and number of views.
- danceibility: Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.
- energy: Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.
- loudness: The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typically range between -60 and 0 db.
- mode: Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0.
- speechiness: Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.
- acousticness: A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.
- instrumentalness: Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.
- liveness: detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.
- valence: a measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
- tempo: the overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.
- duration_mins: How long the song lasted in minutes.
- album: The album the song was on.
- apple_music.isrc: Song code for Apple music streaming platform.
- spotify.id: Song code for Spotify music streaming platform.
- spotify_popularity:The popularity of the track. The value will be between 0 and 100, with 100 being the most popular.The popularity of a track is a value between 0 and 100, with 100 being the most popular. The popularity is calculated by algorithm and is based, in the most part, on the total number of plays the track has had and how recent those plays are.
Generally speaking, songs that are being played a lot now will have a higher popularity than songs that were played a lot in the past. Duplicate tracks (e.g. the same track from a single and an album) are rated independently. Artist and album popularity is derived mathematically from track popularity. Note: the popularity value may lag actual popularity by a few days: the value is not updated in real time.
- explicit: True if the song contained explicit language. False if the song does not contain explicit language.
- peak-rank: Highest spot the song acheived ont he Billboard charts

