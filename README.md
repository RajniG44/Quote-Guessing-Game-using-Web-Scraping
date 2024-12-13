# Quote-Guessing-Game-using-Web-Scraping
Quote Guessing Game using Web Scraping
Project Overview
The Quote Guessing Game is a Python-based project that combines web scraping with game development. It scrapes famous quotes and their authors from http://quotes.toscrape.com using the BeautifulSoup library, then creates an interactive guessing game where the user tries to guess the author of a random quote.

Players have four chances to guess the author, with hints provided after each incorrect attempt. The game reveals details such as the author’s birth date, birthplace, and initials to aid in guessing. A success or failure message is displayed at the end.

Features
Scrapes quotes and author details dynamically from the web.
Interactive guessing game with progressive hints.
Provides a fun way to explore famous quotes and learn about their authors.
Easy-to-extend and reusable codebase.
Technologies Used
Python 3.x: Programming language.
BeautifulSoup (bs4): For web scraping.
Requests: For sending HTTP requests to fetch webpage content.
CSV: For optional data storage.
Random: For selecting random quotes.
Time: For adding delays.
Setup Instructions
1. Clone the Repository
bash
Copy code
git clone https://github.com/your_username/quote-guessing-game.git
cd quote-guessing-game
2. Install Dependencies
Ensure you have Python installed. Install the required libraries using pip:

bash
Copy code
pip install beautifulsoup4 requests
3. Run the Script
Execute the script:

bash
Copy code
python quote_guessing_game.py
4. Play the Game
The game will display a random quote. Guess the author and follow the hints provided until you succeed or run out of guesses.

Game Workflow
Scrape Data: The script fetches quotes, authors, and their biography links from http://quotes.toscrape.com.
Select a Random Quote: A random quote is chosen for the user to guess.
User Interaction:
The user gets four chances to guess the author.
After each incorrect guess, hints are provided:
Author's birth date and place.
Author’s first name's initial.
Author’s last name's initial.
A congratulatory or failure message is shown based on the guesses.
Replay Option: Restart the script to play again with a new random quote.
Modules and Key Functions
Module	Purpose
requests	Fetches HTML content of the web pages.
BeautifulSoup	Parses HTML data and extracts elements.
csv	Helps save scraped data for optional storage or future use.
random.choice	Selects random quotes from the scraped data.
time.sleep	Adds delay to prevent rapid requests, avoiding potential blocking from the server.
Performance
Time Complexity: O(N), where N is the number of quotes on the site.
Space Complexity: O(N), as the all_quotes list stores all scraped quotes and their details.
Future Enhancements
Save and load progress between sessions.
Add more detailed hints (e.g., author's famous works or profession).
Store scraped data in a local file to reduce server requests during replays.
Create a graphical version of the game using a Python GUI library like Tkinter or PyQt.
Disclaimer
This project is intended for educational and personal use. Always ensure compliance with website terms of service when web scraping. The author is not responsible for misuse.

License
This project is licensed under the MIT License.

