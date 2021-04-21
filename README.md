Welcome to Qlik-Slack Birthday bot
Today we'll learn how to make bd bot with qlik and slack.

>This bot was built on some researches on Qlik community site(share to link them)


Our to-do for this quest 
1. Birthdays file, .xlsx in this case, so anyone can add new lines there
2. Config webhook for slack 
3. REST connection from Qlik to Slack
4. Qlik application to shoot everyday for  🎉


- [1. Birthdays file, .xlsx in this case, so anyone can add new lines there](#1-birthdays-file-xlsx-in-this-case-so-anyone-can-add-new-lines-there)
- [2. Config webhook for slack](#2-config-webhook-for-slack)
- [3. Qlik REST API dummy connector](#3-qlik-rest-api-dummy-connector)

Lets go.🚀

---

## 1. Birthdays file, .xlsx in this case, so anyone can add new lines there
Lets assume we have some bds.xlsx on some fileshare with such structure of table\\

| F           | I        | MM             | DD            | AD                         |
|-------------|----------|----------------|---------------|----------------------------|
| *Family name* | *Name*     |* Month of birth* | *Date of birth* | *AD login or Slack username* |
| Baklanov    | Vladimir | 12             | 14            | somefancylogin             |
|             |          |                |               |                            |

## 2. Config webhook for slack 

For this part we need to go to https://slack.com/apps/A0F7XDUAZ-incoming-webhooks and install this app to our slack space.
1. Click `Add to slack`
2. Choose channel to where you want it to post our messages
3. For this manual we'll use `#slack_webhook_test`

After this you'll get: <br id='URL'>
1. URL like `https://hooks.slack.com/services/•••/•••/•••` (• will be numletters)  
2. Ability to customize logo
3. Ability to name it desired way

Done

## 3. Qlik REST API dummy connector

Go to your QlikHub and create empty app(you won't need this one)

- Choose `Add data from files and other sources`<br>
<img src="imgs/rest.png" width="100"/>

- fill URL from [URL](#URL)





```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |


~~The world is flat.~~


- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

