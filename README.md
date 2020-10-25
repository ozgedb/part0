# 0.4-new-note
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes
server-->browser: HTML-code
browser->server: execute console open the Elements tab
server-->browser: HTML code 
note over browser: Find div row in the html code and then press the arrow for menu to drop down
server-->browser: Menu opened
browser->server: Choose form
note over browser:
Add a new note and save
end note
browser->
server-->browser: 
browser->server: The input (note) sent to the server
server-->browser: [{ content: "my new note" }, ...]
note over browser:
Now find the Network tab on the list above the page and click on it.
end note
browser->server: Form data is will appear as new_note on the list opened.



0.5: Single page app
browser->server: https://studies.cs.helsinki.fi/exampleapp/spa
server-->browser: HTML-code
browser->server: executes the JavaScript code 
server-->browser: code fetches the notes as JSON-data 

note over browser:
add HTML elements to the page using the DOM-API



0.6: New note

browser->server: https://studies.cs.helsinki.fi/exampleapp/spa
server-->browser: HTML-code
browser->server: https://studies.cs.helsinki.fi/exampleapp/spa
server-->browser: main.css


note over browser:
open the Network tab and clear out by clicking the clear console symbol
end note

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
server-->browser: [{ content: "HTML is easy", date: "2020-10-25" }, ...]
browser->server:  JavaScript code it fetched from the server

note over browser:
event handler creates a new note, the code is added
to the notes list with the command notes.push(note)
end note
