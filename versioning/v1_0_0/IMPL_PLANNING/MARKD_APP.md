# The 'Markd' App 
*Name is used for various businesses so perhaps Markdup or Markd'up or Markd'Up, all of which the phonetic tool pronounced as we'd want; mentioning this now and here because I don't want to change the name of the project directory* 

## Elevator Pitch 

  * **Lightweight, clean-lined, classic, simple UI app for semantic-highlighted markdown text editing where you can exports to PDF or HTML for free and without extensions; a very curated, simple email client is integrated** 

### The Problem  

  * **There is a limited number of tools to use to write semantic highlighted markdown** 

  - I was writing an email in my Apple Mail application and hating it 
    - Set my font to 'JetBrains Mono 12 Regular' 
    - Now you can't differentiate the sections of text because there is no highlighting 

  - My Cursor IDE has perfected semantic highlighting 
    - I used the textMateRules here `./.vscode/textMateRules.md` 
    - It is honestly difficult to even change IDEs because of issues using or recreating my highlighting setup 

  * **Using your markdown is even more of a challenge**

  - IDE markdown 'PREVIEW' is always so typographically beautiful 
    - There is never a print or export as PDF or HTML built in 
    - The extensions are not reliable and oven overly complex  

  - We created an MCP for "Markdown > PDF" 
    - Tried to convert the beautiful VSCode CSS to use 
    - Too much troubleshooting and never got it to look nice 

  - We have researched applications 
    - They are often too over-purposed 
    - Or they charge a subscription fee 
    - The open source options, including email clients, don't have semantic highlighting 

### Intended Solution 

  * **Convey in this document detailed app functioning in normal language to write code files**  

  1. An extremely simple, text input display; very TextEdit-like  
  2. UI container that has no buttons or menus other than the required for MacOS apps 
  3. Very lightweight, fast, modern MacOS build that is simple and classic enough to be timeless 
  4. textMateRule-like color settings; themes; all labels are easy to understand and have visual example 
  5. Saves files with extension .md; exports .pdf and .html that is typographically adequate to start, perfected over time 
  6. Start by including only two fonts: JetBrains Mono Regular 12 & something like Helvetica with headers and styling 
  7. Only can write in plain text markdown that wraps according to the width of the window or print page 
  8. Check spelling as you type, automatically, along with grammar, pulling ideally from Apple's dictionary 
  9. No smart/curved quotes or apostrophes or dashes or even links; even pasted text just pastes as plain text markdown 
  10. Use dark background for windows; can be altered by user 

### Shortcuts and Syntax  

  * **Reviewed TextEdit, Apple Mail, Cursor menus and pulled essential shortcuts** 

  - User can toggle a view of the shortcut list
    - If they have a maximized window, it shows up like a side panel 
    - If they have a window not maximized, it shows up in its own container 

  - AI shortcuts listed below 
    - This is just thinking ahead, I don't want to complicate the first build too much 
    - Eventually though it would be interesting to attempt something like Cursor Tabs, particularly for re-formatting 
    - Even without the tab suggestions, an AI could very easily compose the rest of a half written email 
    - And eventually you can chat the AI to write whatever 

  - Any advanced help with formatting sooner would be cool 
    - Making charts is difficult for example 
    - When I have tab suggestions turned on it straightens them up when you save 

| Shortcut                                      | Action                | 
| --------------------------------------------- | --------------------- | 
| <kbd>CMD</kbd> <kbd>O</kbd>                   | Open                  |
| <kbd>CMD</kbd> <kbd>S</kbd>                   | Save                  |
| <kbd>CMD</kbd> <kbd>shift</kbd> <kbd>S</kbd>  | Save As               |
| <kbd>CMD</kbd> <kbd>W</kbd>                   | Close                 |
| <kbd>CMD</kbd> <kbd>Q</kbd>                   | Quit                  |
| <kbd>CMD</kbd> <kbd>M</kbd>                   | Minimize              |
| <kbd>CMD</kbd> <kbd>H</kbd>                   | Hide                  |
| <kbd>CMD</kbd> <kbd>N</kbd>                   | New document          |
| <kbd>CMD</kbd> <kbd>shift</kbd> <kbd>N</kbd>  | New email             |
| <kbd>CMD</kbd> <kbd>P</kbd>                   | Print                 |
| <kbd>CMD</kbd> <kbd>E</kbd>                   | Export PDF            |
| <kbd>CMD</kbd> <kbd>shift</kbd> <kbd>E</kbd>  | Export HTML           |
| <kbd>CMD</kbd> <kbd>return</kbd>              | Send email            |
| <kbd>CMD</kbd> <kbd>R</kbd>                   | Reply                 |
| <kbd>CMD</kbd> <kbd>shift</kbd> <kbd>R</kbd>  | Reply all             |
| <kbd>CMD</kbd> <kbd>F</kbd>                   | Forward               |
| <kbd>CMD</kbd> <kbd>U</kbd>                   | Mark as unread        |
| <kbd>CMD</kbd> <kbd>shift</kbd> <kbd>A</kbd>  | Attachment            |
| <kbd>CMD</kbd> <kbd>Z</kbd>                   | Undo, Undo send       |
| <kbd>CMD</kbd> <kbd>shift</kbd> <kbd>Z</kbd>  | Redo                  |
| <kbd>CMD</kbd> <kbd>X</kbd>                   | Cut                   |
| <kbd>CMD</kbd> <kbd>C</kbd>                   | Copy                  |
| <kbd>CMD</kbd> <kbd>V</kbd>                   | Paste                 |
| <kbd>CMD</kbd> <kbd>A</kbd>                   | Select all            |
| <kbd>CMD</kbd> <kbd>/</kbd>                   | Toggle shortcut sheet |
| <kbd>CMD</kbd> <kbd>,</kbd>                   | Open settings         |
| <kbd>delete</kbd>                             | Archive message       |
| <kbd>CMD</kbd> <kbd>delete</kbd>              | Delete message        |
| <kbd>CMD</kbd> <kbd>shift</kbd> <kbd>J</kbd>  | Message to junk       |
| <kbd>CMD</kbd> <kbd>option</kbd> <kbd>J</kbd> | Empty junk folder     |
| <kbd>CMD</kbd> <kbd>R</kbd>                   | Refresh inbox         |
| <kbd>CMD</kbd> <kbd>T</kbd>                   | Toggle AI chat        |
| <kbd>CMD</kbd> <kbd>shift</kbd> <kbd>T</kbd>  | AI continue writing   |

  * **Advanced shortcuts currently used a lot in Cursor** 

  - Highlight a word and add markdown formatting or punctuation and the word is automatically wrapped 
    - Highlight word, <kbd>SHIFT</kbd> <kbd>*</kbd> = italics; also works for <kdb>_</kbd>
    - Highlight word, <kbd>SHIFT</kbd> <kdb>**</kbd> = bold; also works for <kbd>__</kdb> 
    - Highlight word, <kbd>'</kbd> = wrapped single apostrophe 
      - Shift for double 
      - Use <kbd>`</kdb> key for inline code wrap 
      - And <kbd>~~</kdb> for strikeout 
      - Etc. if you know more standard markdown shortcuts than I do 
  - When you type the first parenthesis both show up and your cursor starts inside them
    - This one has logic that when done you can hit the end parenthesis to move along 
    - Or you can use the arrow key to move out 
    - It works the same for brackets and any-number-of curly brackets 

  * **List of markdown syntax to save for a help screen** 

    | Markdown Characters Used               | Rendered Result in PDF/HTML/Email       |
    | -------------------------------------- | --------------------------------------- | 
    | [Portfolio](www.portfolio.com)         | Hyperlinked 'Portfolio' displayed only  | 
    | [hey@email.com](mailto:hey@email.com)  | Email opens new email; phone works too  | 
    | [Chapter 2](#chapter-2)                | Anchor-linked 'Chapter 2' displayed     |
    | *italics* or _italics_                 | 'italics' appears in italics only       |
    | **bold** or __bold__                   | 'bold' appears with bold styling only   | 
    | # Title                                | H1 or Title Size Text                   | 
    | ## Section                             | H2 main page sections heading size      | 
    | ### Chapter of Section                 | H3 section chapter's heading size       | 
    | #### Part of Chapter                   | H4 chapter part's heading size          | 
    | ##### and ###### rest of sizes         | H5 and H6, in total H1 to H6            |
    | - Unordered list item                  | Looks like a normal bullet point        | 
    | * or + Unordered list item             | Same bullet; helps when editing only    | 
    | 1. Ordered list item                   | Looks like a normal numbered list       | 
    | `backtick each side`                   | In-line code formatting                 | 
    | ``` above and below code ```           | Write horizontally, creates code embed  |
    | ~~cross something out~~                | Shows as strikeout when rendered        |
    | > Before a series of sequential lines  | Creates a blockquote of that text       |
    | ![alt text](image.jpg)                 | Shows image at URL with alt. text added |
    |  - [ ] or - [x] in a list              | Shows an empty or checked list box      | 
    | | table | content |                    | Renders looking like a formal table     |
    | --- on a line by itself                | Horizontal line page break              | 
    | $inline math$ or $$block math$$        | Script like proper written equations    | 
    | <kbd>shift</kbd>                       | Key text appears on not-functional key  |
