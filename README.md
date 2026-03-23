# Token Usage Checker

A simple web tool to check what percentage of your token quota you have used.

## How to use

1. Open `index.html` in your browser (or host it on any static web server).
2. Enter the number of **tokens you have used** in the first field.
3. Enter your **total token limit** in the second field.
4. Click **Check Usage** (or press **Enter**).

The tool will show you:

- A colour-coded progress bar (green → yellow → red as usage increases)
- The exact percentage used
- Tokens used, tokens remaining, and the total limit
- A status message indicating whether your usage is low, medium, or high

## Usage levels

| Percentage | Status |
|---|---|
| 0 – 49 % | ✅ Low – plenty remaining |
| 50 – 79 % | ⚠️ Medium – consider monitoring |
| 80 – 100 % | 🚨 High – running low |