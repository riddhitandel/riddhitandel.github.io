# riddhitandel.github.io

Here is what I used for CSS. 

1. The boxes or rather the cards that you see on the page for projects, labs, certs, about, etc.

.card {
    padding: 35px;  --> Adss inner space 
    border: 1px solid rgba(56, 189, 248, .3); --> thin blue border that appears on the page to define their outlines
    border-radius: 12px; --> gives the boxes rounded corners = modern UI
    background: rgba(255, 255, 255, .03);  --> mkaes it semi-transparent
} 

2. What actually makes the card interactive 

.card:hover {
    transform: translateY(-8px);
    box-shadow: 0 0 25px rgba(56, 189, 248, .5);
}

3. How the size is decided for the cards 

grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); 

- Each card is minimum 250px wide 
- But can expand to fill space (1fr)
- auto-fit --> automatically adjusts number of coloums, so 
small screen - 1 coloum 
medium - 2-3 coloumns 
large - fills full row nicely 

4. What creates the Layout (Grid System)

.dashboard {
    display: grid;  --> Turns layout into structured grid 
    gap: 25px;      --> spcaing between boxes 
}
