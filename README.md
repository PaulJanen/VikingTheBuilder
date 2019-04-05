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
    
- [ ] MailSubscription - entity, that stores mails in the database. 
- [ ] 3 mandatory attributes:
    - [ ] name:string;
    - [ ] surname:string;
    - [ ] mail:string;
- [ ] 5 custom attributes
    - [ ] maxNameCharacterCount:number;
    - [ ] maxSurnameCharacterCount:number;
    - [ ] maxMailCharacterCount:number;
    - [ ] Mailtext:ut.Entity[];
    - [ ] SubscribeToMailbutton:ut.Entity[];

## Entity restriction
- [ ] Question line max length = 46;
- [ ] Answer line max length = 46; These two restrictions exists, so system dynamicaly breaks lines (it can't on its own...)
- [ ] Question line length is 5 lines. If it crosses 5 lines limit scroll options appear.
- [ ] Answer line length is 2 lines. If it crosses 2 lines limit app crashes
- [ ] maxQuestionIndex:number. Restricts scrolling.


## API definition


## UI definition
# UI Structure
- [ ] In main window there will be (home,blog press) buttons followed by newly opened blog post with branching dialog options. It will not only show images and text, but as well will stream gifs.
# Views
- [ ] https://imgur.com/a/lGvhKT1
- [ ] https://imgur.com/a/jSNG3XO


