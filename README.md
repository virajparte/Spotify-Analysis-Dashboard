# Spotify-Analysis-Dashboard
# 🎧 Spotify Streaming Behavior Analysis

Understanding how listeners interact with music — from what they play to when they skip — can uncover powerful insights about user preferences and content performance.  
This analysis dives deep into **Spotify streaming logs** to decode how people really listen.

---

## 👀 Why This Project?

Music streaming platforms thrive on engagement — but behind every play or skip, there’s a story 🎶

📌 This analysis helps answer:

- Which songs are people loving — and finishing?
- When do listeners lose interest and skip?
- Which artists keep audiences hooked?
- Which platforms do people listen on the most?
- What time do listeners tune in?
- How does shuffle mode change listening behavior?

If the question helps improve **user retention and discovery**, this dashboard **answers it**.

---

## 🧩 Data Domain Overview

| Field               | What It Represents                             | Why It Matters                          |
|--------------------|------------------------------------------------|-----------------------------------------|
| `spotify_track_uri` | Unique track ID                                | Connect data to Spotify catalog         |
| `ts`                | Timestamp when playback stopped                | Session pattern & peak hours            |
| `platform`          | Device used (mobile/desktop/web/smart speaker) | Device-based engagement trends          |
| `ms_played`         | Duration played in milliseconds                | Completion, skips & revenue calculation |
| `track_name`        | Track title                                    | Track popularity                        |
| `artist_name`       | Name of artist                                 | Listener taste & top artists            |
| `album_name`        | Album name                                     | Album-level performance                 |
| `reason_start`      | Why playback started (click, autoplay, etc.)   | User-driven vs passive listening        |
| `reason_end`        | Why playback stopped (finished/skipped/logout) | Drop-off detection                      |
| `shuffle`           | Shuffle mode enabled?                          | Listening style preferences             |
| `skipped`           | Song skipped?                                  | Popularity & engagement score           |

🎯 Ultimate Goal → Help Spotify & artists **boost listener loyalty**.

---

## 🔍 What We Can Discover

### 🎵 Listener Engagement
- Most played songs, artists & albums
- Skip patterns → where interest drops
- True favorites → completed plays

### 📱 Platform Usage
- Mobile usage dominates?
- Desktop for work hours?
- Smart speakers on weekends?

### 🕒 Time-Based Trends
- Peak listening hours
- Best-performing weekdays
- Special spikes (e.g., Friday releases)

---

## 📈 Key Metrics Tracked

| KPI                            | Insight                                     |
|-------------------------------|---------------------------------------------|
| **Skip Rate**                  | Tracks losing listener attention quickly    |
| **Completion Rate**            | True engagement & fan loyalty               |
| **Artist Popularity Index**    | Based on listening time                     |
| **Listening Session Duration** | How long users stay active                  |
| **Shuffle Dependency**         | Listener discovery & exploration patterns   |

💡 Spotify pays artists **based on ms_played** → this metric drives revenue.

---

## 🧠 Example Insights

> Listeners love starting music…  
> but **many tracks stop before finishing**.

Meaning:
- Some songs attract clicks but don’t hook
- Skips tell **exactly when** interest declines
- Autoplay choices reveal **real** favorites

🕔 Evening hours show longest sessions  
📱 Mobile leads streaming  
🎲 Shuffle = more exploration & new discoveries

---

## 🛠 Data Model (Star Schema)

| Type           | Table                                              | Purpose                                              |
|----------------|----------------------------------------------------|------------------------------------------------------|
| **Fact Table** | `streaming_events`                                 | Playback duration, skip status, start/end reasons    |
| **Dimensions** | `tracks`, `artists`, `albums`, `platforms`, `time` | Filtering & drill-down analytics                     |

Optimized for **engagement & performance tracking** ✔

---

## 🎯 Who Benefits?

| Stakeholder              | Benefit                                      |
|------------------------|----------------------------------------------|
| 🎤 Artists              | Know which songs people truly enjoy          |
| 🧠 UX Teams             | Improve player behavior & autoplay           |
| 💸 Business Teams       | Increase payout through retention            |
| 🔊 Recommendations Team | More accurate personalization                 |

---

## 🚀 Future Enhancements

- Skip-time detection → identify weak song sections
- Genre & mood clustering using ML
- Listener persona segmentation
- Predicting which songs are likely to be skipped next

---

