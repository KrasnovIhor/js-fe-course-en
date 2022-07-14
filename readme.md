## Alexandra:

### Basic scope +50/+80

- **Layout, design, UI of the main page of the application: (+10)**
    - [X] all elements specified in the task are present on both the mobile and desktop versions
    - [X] all described application design requirements are met

- **Layout, design, UI of the interactive menu: (+10)**
  - [X] all described application design requirements are met
  - [X] menu links are functional and lead to corresponding categories page of words
  - [x] active link is styled differently
  - [x] the interactive menu is present on all pages of the application
  - [x] smooth animation of the interactive menu
  - [x] the menu is closed by clicking on the cross icon, by clicking on the link in the menu, by clicking anywhere in the application, except the menu itself

- **Layout, design, UI of categories page: (+10)**
    - [x] all the elements specified in the task are present on both mobile and desktop versions
    - [ ] all described application design requirements are met

- **Training Mode: (+20)**
    - [x] when you click on the card, the word is pronounced in English: (+10)
    - [x] each card has a button on the right bottom corner. When you click on that button the card flips over. The back side of the card has a translation of the word. A card is rotated back to the front side when the mouse cursor moves beyond the borders of the card: (+10)

- **Code quality requirements are met (+30)** (evaluated by mentors only)
  - [ ] code duplication is kept to minimum: (+10)
  - [x] js-code is divided into modules: (+10)
  - [x] webpack, eslint, eslint-config-airbnb-base and babel are used: (+10)

### Advanced scope +80

- **Game Mode: (+80)**
    - [x] the game mode is activated by toggling the Train/Play switch button. Features described above for the training mode are disabled for the game mode. The button that flips the card and the text on the card are both hidden. The "Start game" button is displayed. Card size does not change. Only the image remains on the card, which occupies the card's entire area (if this does not contradict your design): (+10)
    - [x] after clicking on the "Start game" button, the random word from those on the page is pronounced. For each page, and for each game, random words are generated anew: (+10)
    - [x] after the first click on the "Start game" button, the button changes to the "Repeat" icon. When you click on the "Repeat" button, the word is pronounced again: (+10)
    - [x] the sound signal "error" is played if the user clicks on the wrong active card: (+10)
    - [x] the sound signal “correct” is played if the user clicks on the correct active card. After that, a new random word from those that have not yet been guessed is pronounced: (+10)
    - [x] a card with correctly guessed word becomes inactive, and its style is changed. Clicks on inactive cards are not accompanied by any sound effects, and they do not affect the game score: (+10)
    - [x] after the start of the game, each click on the active card is displayed in the form of stars (or other symbols). The correct answer is displayed with one colored star and the wrong answer is displayed with a different colored star. If there are too many stars and there is no space, the previous stars are hidden, and the new ones are added: (+10)
    - [x] when the game is over: (+10)
        - if all words are guessed correctly, the “success” signal is played, cards with words are removed, and a joyful emoticon (or another picture) is displayed on the page
        - if there were errors while guessing the words, the “failure” signal is played, cards with words are removed, and a sad emoticon (or other picture) with the number of mistakes is displayed on the page.
        - afterward, the application automatically redirects to the main page with a list of categories

### Hacker scope +40

- **Statistics Page: (+40)**
    - [ ]  statistics page contains a list of all categories, all words in each category, and a translation of each word. The minimum width at which statistics page is displayed correctly is 320 px. The presence of a scrollbar in a table with statistics is not considered to be an error: (+10)
    - [ ] statistics are displayed next to each word - how many times a card with a given word was clicked in training mode, how many times this word was guessed in game mode, how many mistakes were made, the percentage of correct answers for each word in game mode. After restarting the application, statistics are saved: (+10)
    - [ ] it is possible to sort the data alphabetically, for numerical data - by their value. Sorting can occur in ascending and descending order and should cover the entire data range: (+10)
    - [ ] there are "Repeat difficult words" and "Reset" buttons on the statistics page. The "Reset" button resets statistics. Clicking on the "Repeat difficult words" button opens a page similar to the category page with most frequent words guessed wrong. The page "Repeat difficult words" can have from zero to eight words, depending on how many words were guessed wrong in play mode. After clicking on the "Reset" button, the number of words on the "Repeat difficult words" page is set to zero: (+10)
    - [ ] additional functionality outside of the scope of the task is implemented. This part is not evaluated, but if you can do better, then why not.

## Penalty Points
- [ ] less than eight categories, less than eight words in each category, data for the last two categories is copied from the demo, and not prepared independently: -10 points
- [ ] requirements for a pull request, repository, and commit names are not met: -10 points (evaluated by mentors only)
- [ ] source code requirements are not met: -10 points or more (evaluated by mentors only)
