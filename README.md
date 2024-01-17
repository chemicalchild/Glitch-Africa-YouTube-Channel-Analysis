# Glitch-Africa-YouTube-Channel-Analysis
This code uses YouTube API to scrape Glitch Africa channel data 

# Glitch Africa YouTube Channel Analysis - Code Documentation

## Overview

This code documentation outlines the steps involved in fetching statistics for the Glitch Africa YouTube channel, obtaining video details, and performing various analyses on the data. The analyses include transforming data types, calculating video duration in seconds, finding the best and least viewed episodes, generating violin plots, scatter plots, word clouds, and creating additional visualizations.

### 1. Channel Statistics

#### 1.1. get_channel_statistics(api_key, channel_id)
Description:
Fetches basic statistics for the Glitch Africa YouTube channel.
Parameters:
- `api_key`: Your YouTube Data API key.
- `channel_id`: Unique identifier for the Glitch Africa YouTube channel.

#### 1.2. `get_video_ids(api_key, channel_id)`
Description:
Retrieves the video IDs of all videos on the Glitch Africa channel.
Parameters:
- `api_key`: Your YouTube Data API key.
- `channel_id`: Unique identifier for the Glitch Africa YouTube channel.

### 2. Video Details
#### 2.1. `get_video_details(api_key, video_ids)`
Description:
Fetches detailed information for each video on the Glitch Africa channel using the provided video IDs.
Parameters:
- `api_key`: Your YouTube Data API key.
- `video_ids`: List of video IDs obtained from `get_video_ids`.

### 3. Data Transformation
#### 3.1. transform_data(data)
Description:
Converts data types for better analysis, e.g., converting timestamps to datetime objects.
Parameters:
- `data`: DataFrame containing video details.

### 4. Video Duration in Seconds
#### 4.1. get_duration_seconds(data)
Description:
Calculates the duration of each video in seconds on the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

### 5. Best and Least Viewed Episodes
#### 5.1. get_best_episode(data)
Description:
Identifies the episode with the highest views on the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

#### 5.2. `get_least_episode(data)`
Description
Identifies the episode with the least views on the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

### 6. Best Episodes by Likes and Comments
#### 6.1. `get_best_episodes_by_likes(data)`
Description:
Identifies the episodes with the highest likes on the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

#### 6.2. `get_best_episodes_by_comments(data)`
Description
Identifies the episodes with the highest comments on the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

### 7. Visualizations
#### 7.1. `plot_violin(data)`
Description:
Generates a violin plot to visualize the distribution of views for videos on the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

#### 7.2. `scatter_plot(data)`
Description:
Creates scatter plots of comments against views and likes against views for the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

#### 7.3. `plot_duration_vs_videos(data)`
Description:
Plots video duration against the number of videos for the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

### 8. Word Cloud
#### 8.1. `generate_word_cloud(data)`
Description:
Generates a word cloud based on video titles for the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

### 9. Most Published Days
#### 9.1. `most_published_days(data)`
Description:
Identifies the days on which Glitch Africa publishes the most episodes.

Parameters:
- `data`: DataFrame containing video details.

### 10. Data Frame of Comments
#### 10.1. `create_comments_dataframe(data)`
Description:
Creates a DataFrame specifically for video comments on the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

### 11. New Data Frame with Separated Episode Titles and Show Titles
#### 11.1. `separate_titles(data)`
Description:
Creates a new DataFrame with separated episode titles and show titles on the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

### 12. Bar Plots
#### 12.1. `bar_plot_videos_vs_comment(data)`
Description:
Generates a bar plot comparing the number of comments for each video on the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

#### 12.2. `bar_plot_videos_vs_views(data)`
Description:
Generates a bar plot comparing the number of views for each video on the Glitch Africa channel.
Parameters:
- `data`: DataFrame containing video details.

#### 12.3. `bar_plot_videos_vs_likes(data)`
Description:
Generates a bar plot comparing the number of likes for each video on the Glitch Africa channel.

Parameters:
- `data`: DataFrame containing video details.

## Conclusion

This code documentation provides a guide for analyzing statistics, obtaining video details, and performing various insightful analyses for the Glitch Africa YouTube channel using Python. Each function serves a specific purpose, allowing for a comprehensive understanding of the channel's content, engagement, and audience interaction.

