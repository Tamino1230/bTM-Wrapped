# Wrapped for babTomaMusic (btM)

The `wrapped.py` script is a standalone feature inspired by Spotify Wrapped, designed specifically for the **babTomaMusic (btM)** app. It provides users with a personalized summary of their music listening habits, offering insights into their most-played songs, total listening time, and more.

---

## Features

- **Top 10 Songs**: Displays your most-played songs with their total playtime.
- **Total Listening Time**: Summarizes your total listening time in hours and minutes.
- **Songs Played Less Than 5 Minutes**: Highlights songs that were played briefly.
- **Least Played Songs**: Lists the 5 songs with the least playtime.
- **Unique Songs Count**: Shows the total number of unique songs played.

---

## How It Works

The script reads data from the `song_playtimes.json` file, which tracks the playtime of each song in seconds. It processes this data to generate a detailed report and saves it in a file called `wrapped_report.txt`.

---

## Usage

1. Ensure the `song_playtimes.json` file exists in the same directory as `wrapped.py`.
2. Make sure the setting `record_actions` in the `scripts/config.py` file of the **babTomaMusic** app is set to `True` to record playtime data:
   ```python
   record_actions = True
   ```
3. Run the script:
   ```bash
   python wrapped.py
   ```
4. After execution, check the `wrapped_report.txt` file for your personalized music summary.

---

## Example Output

Here’s an example of what the `wrapped_report.txt` might look like:

```
Your Top 10 Songs:
1. Song A - 669 Minuten
2. Song B - 555 Minuten
...

Total Playtime:
112 hours and 9 minutes

Songs Played Less Than 5 Minutes (Top 5):
- Song X (4 Minuten)
...

Your Least Played 5 Songs:
1. Song Y - 0 Minuten

Unique Songs Played:
269 unique songs
```

---

## Integration with babTomaMusic (btM)

This script is designed to work seamlessly with the **babTomaMusic (btM)** app. It uses the playtime data recorded by the app to generate the report. Think of it as your very own "Spotify Wrapped" for btM!

To learn more about the **babTomaMusic** app, visit the [GitHub repository](https://github.com/Tamino1230/babTomaMusic).

---

## License

This script is part of the **babTomaMusic (btM)** project and is licensed under the MIT License. See the main project repository for more details.
