# WEB system
- [ ] Viking The Builder

## Description
- [ ] Little app where user talks with system by picking answers. Reminds branching dialog options in rpg games. Purpose of this site: it's a marketing tool and landing page for upcoming game: Viking The Builder. Because it's landing page as well it has blog and press release pages.

## Entity definition
- [ ] BlogClass - entity, that controls branching options, questions, button clicks or animations, showing text, setting questionns.
- [ ] 3 mandatory attributes:
    - [ ] questions:string[]
    - [ ] questionIndex:number;
    - [ ] contactsChilds:Array<ut.Entity> = [];
- [ ] 5 custom attributes
    - [ ] questionLineMaxLetterCount:number;
    - [ ] answerLineMaxLetterCount:number;
    - [ ] questionControls:Array<ut.Entity> = [];
    - [ ] contactsChilds:Array<ut.Entity> = [];
    - [ ] button1:ut.Entity[];
    
## Entity restriction
- [ ] Question line max length = 46;
- [ ] Answer line max length = 46; These two restrictions exists, so system dynamicaly breaks lines (it can't on its own...)
- [ ] Question line length is 5 lines. If it crosses 5 lines limit scroll options appear.
- [ ] Answer line length is 2 lines. If it crosses 2 lines limit app crashes
- [ ] maxQuestionIndex:number. Restricts scrolling.

##
- [ ] Analytics - entity, that stores login count and press release visit count in the database. 
- [ ] 3 mandatory attributes:
    - [ ] pressReleaseCount:int;
    - [ ] loginCount:int;
    - [ ] query:string;
- [ ] 5 custom attributes
    - [ ] row:number;
    - [ ] result:mysqlQuery;
    - [ ] sql:string;
    - [ ] con:mySqli_connect;
    - [ ] SubscribeToMailbutton:ut.Entity[];




## API definition 

 - [] POST /api/analytics{logincount} - Adds one user login count to the database.
  Error 400: Database is not running.
 - [] POST /api/analytics{pressReleaseCount} - Adds one user press release count to the database.
  Error 400: Database is not running. 
 - [] GET /api/analytics/{logincount} - Gauna kiek varotojų buvo prisijunge prie svetainės
 -Klaida 400: Duomenų bazė neveikia.   
 - [] PUT /api/analytics/{} - Ištrina vartotjo loginą.
 - Klaida 400: Įvestas paštas neegzistuoja. 
 

## UI definition
# UI Structure
- [ ] In main window there will be (home,blog press) buttons followed by newly opened blog post with branching dialog options. It will not only show images and text, but as well will stream gifs.
# Views
- [ ] https://imgur.com/a/lGvhKT1
- [ ] https://imgur.com/a/jSNG3XO


