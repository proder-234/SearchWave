# **SearchWave- Web & Music Search Engine**

## A lightweight, client-side search engine with two modes: live web search powered by DuckDuckGo, and a local lyrics/music search engine backed by a pre-indexed dataset of songs.

**Live demo:** [https://userweb.cs.txstate.edu/\~mkj82/](https://userweb.cs.txstate.edu/~mkj82/)

## **Features**

* **Web Search (Part A)** — Queries DuckDuckGo through public CORS proxies and parses the HTML response to render the top 10 web results, including title, URL, and snippet.  
* **Lyrics Search (Part B)** — Searches a local JSON dataset of songs entirely in the browser. Results are ranked by a scoring model that weighs matches in the song title, artist name, and lyrics. Clicking a result opens a dedicated song page (song.html) displaying the full lyrics.

## **Project Structure**

project mining/  
├── index.html        \# Main page — tabbed interface for both search modes  
├── song.html         \# Full song/lyrics detail page  
├── lyrics.csv        \# Raw lyrics dataset (source data)  
├── js/  
│   └── songs.json    \# Pre-processed, indexed song data loaded at runtime  
└── static/  
    └── style.css     \# Stylesheet 

## **How to Use**

1. Open the live URL above in any modern browser.  
2. **Web Search** is selected by default — type a query and press Enter or click the search button.  
3. Switch to **Lyrics Search** using the tab at the top of the search bar, then search by song name, artist, or any lyric phrase.  
4. Click any lyrics result card to open the full song page.

## **Author**

SAJJA REGMI, mkj82 — Texas State University
