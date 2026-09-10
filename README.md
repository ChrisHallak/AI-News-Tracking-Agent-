# AI News Intelligence Agent

An automated n8n workflow that helps me keep up with the latest AI news and discussions on YouTube.

The workflow runs every day at 9 PM, finds AI-related videos published during the last 24 hours, filters them based on their engagement and relevance, extracts the transcripts, and uses an LLM to generate a daily report.

## Why I built this

AI is moving very quickly, and there are new announcements, models, tools, and discussions almost every day.

I personally like watching videos and podcasts about AI because I don't only want to know what happened. I also want to understand what people are saying about it and what different opinions there are.

The problem is that watching all of this content every day takes a lot of time.

So I built this workflow to automate the first part of that process.

Instead of going through dozens of videos myself, I get a daily report that gives me an overview of the most important things happening in AI and the discussions around them.

## How it works

The workflow runs automatically every day at 9 PM.

```text
Schedule Trigger
       ↓
Find Recent AI Videos
       ↓
Process Each Video
       ↓
Get Video Details
       ↓
Calculate Video Engagement
       ↓
Filter Relevant Videos
       ↓
Get Video Transcript
       ↓
Prepare Transcript
       ↓
Save Transcript
       ↓
Combine All Transcripts
       ↓
Extract Transcript Text
       ↓
Analyze AI News
       ↓
Format News Report
       ↓
Save Daily AI Report
