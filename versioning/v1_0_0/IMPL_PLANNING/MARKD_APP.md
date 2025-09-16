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

### Additional Settings 

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

```
            | Shortcut         | Action                | 
            | ---------------- | --------------------- | 
            | CMD + O          | Open                  |
            | CMD + S          | Save                  |
            | CMD + shift + S  | Save As               |
            | CMD + W          | Close                 |
            | CMD + Q          | Quit                  |
            | CMD + M          | Minimize              |
            | CMD + H          | Hide                  |
            | CMD + N          | New document          |
            | CMD + shift + N  | New email             |
            | CMD + P          | Print                 |
            | CMD + E          | Export PDF            |
            | CMD + shift + E  | Export HTML           |
            | CMD + return     | Send email            |
            | CMD + R          | Reply                 |
            | CMD + shift + R  | Reply all             |
            | CMD + F          | Forward               |
            | CMD + shift + U  | Mark as unread        |
            | CMD + shift + A  | Attachment            |
            | CMD + Z          | Undo, Undo send       |
            | CMD + shift + Z  | Redo                  |
            | CMD + X          | Cut                   |
            | CMD + C          | Copy                  |
            | CMD + V          | Paste                 |
            | CMD + A          | Select all            |
            | CMD + /          | Toggle shortcut sheet |
            | CMD + ,          | Open settings         |
            | delete           | Archive message       |
            | CMD + delete     | Delete message        |
            | CMD + shift + J  | Message to junk       |
            | CMD + option + J | Empty junk folder     |
            | CMD + R          | Refresh inbox         |
            | CMD + T          | Toggle AI chat        |
            | CMD + shift + T  | AI continue writing   |
```

  * **Advanced shortcuts currently used a lot in Cursor** 

  - Highlight a word and add markdown formatting or punctuation and the word is automatically wrapped 
    - Highlight word, `SHIFT + *` = italics; also works for _
    - Highlight word, `SHIFT + **` = bold; also works for __ 
    - Highlight word, `'` = wrapped single apostrophe 
      - Shift for double 
      - Use ` key for inline code wrap 
      - And ~~ for strikeout 
      - Use $ for whatever it means to wrap a word in two dollar signs 
      - Etc. if you know more standard markdown shortcuts than I do 
  - When you type the first parenthesis both show up and your cursor starts inside them
    - This one has logic that when done you can hit the end parenthesis to move along 
    - Or you can use the arrow key to move out 
    - It works the same for brackets and any-number-of curly brackets 