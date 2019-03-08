# WEB system
- [ ] Viking The Builder

## Description
- [ ] Little app where user talks with system by picking answers. Reminds branching dialog options in rpg games. Purpose of this site: it's a marketing tool and landing page for upcoming game: Viking The Builder. Because it's landing page as well it has blog and press release pages.

## Entity definition
- [ ] BlogClass - entity, that controls branching options, questions, button clicks or animations, showing text, setting questionns.
- [ ] 3 mandatory attributes:
    - [ ] questions:string[]
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


## API definition
- [ ] API should have at least 4 methods
    - [ ] A method to return entity by ID. Should not have request body
    - [ ] A method to return multiple entities (Array) by ID. This method should support at least one header value to:
        - [ ] Return only entities that match pattern in one of its attributes
        - [ ] Return 10 entities starting provided index
        - [ ] Return sorted entities by one of its attributes (both ascending and descending)
        - [ ] Other (should be approved by Product Owner (PO))
    - [ ] A method to remove entity by ID. Returns removed entity. Should not have request body
    - [ ] A method to update entity by ID. Accepts entity to update and returns updated entity
- [ ] Each method should have HTTP method defined
- [ ] Each method should have URI defined (use {id} as entity ID placeholder)
- [ ] Should return all 4xx errors in unified format. Define format using `joi` language
- [ ] Should return all 5xx errors in unified format. Define format using `joi` language

## UI definition
# UI Structure
- [ ] In main window there will be (home,blog press) buttons followed by newly opened blog post with branching dialog options. It will not only show images and text, but as well will stream gifs.
# Views
- [ ] https://imgur.com/a/lGvhKT1
- [ ] https://imgur.com/a/jSNG3XO


